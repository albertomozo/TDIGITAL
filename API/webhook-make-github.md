Para ilustrar cómo funcionan los webhooks en un entorno real, analizaremos el diseño paso a paso de una integración muy común: **notificar a tu equipo (por ejemplo, en Slack o por correo electrónico) cada vez que un desarrollador realiza un envío (*push*) o una actualización en un repositorio de GitHub**.

Este flujo se basa en una comunicación reactiva: en lugar de que Make consulte a GitHub cada 5 minutos (polling), GitHub "empujará" un paquete de datos (payload JSON) a Make en el milisegundo exacto en que ocurra el evento.

---

### Paso 1: Crear y configurar el Webhook en Make.com

Para este ejemplo, utilizaremos un **Custom Webhook** (Webhook personalizado) en Make, lo que te dará un control total de la estructura de datos.

1. Entra a tu cuenta de **Make.com**, crea un escenario nuevo desde cero y agrega como primer módulo el disparador **Webhooks > Custom webhook**.


2. Haz clic en **Add** para crear una nueva configuración.


3. Dale un nombre descriptivo, como `GitHub-Repo-Updates`, y haz clic en **Save**.


4. Make generará inmediatamente una dirección URL única (por ejemplo: `[https://hook.eu2.make.com/abc123xyz456def](https://hook.eu2.make.com/abc123xyz456def)`).


5. Haz clic en **Copy address to clipboard** para copiar esta URL (mantenla en secreto, ya que cualquiera con acceso a ella podría activar tu escenario).


6. Deja la ventana de Make abierta; verás que el módulo se queda en estado de escucha activa ("Waiting for data").



---

### Paso 2: Configurar el Webhook en tu repositorio de GitHub

Ahora debes indicarle a GitHub a dónde enviar la información de los eventos.

1. Ve a tu cuenta de **GitHub**, entra al repositorio que deseas monitorear y haz clic en la pestaña **Settings** (Configuración) en la barra superior.
2. En el menú lateral izquierdo, selecciona **Webhooks** y luego haz clic en el botón **Add webhook** (Agregar webhook).
3. En el campo **Payload URL**, pega la dirección URL que copiaste de Make.com.


4. En **Content type**, asegúrate de seleccionar **`application/json`** (es fundamental para que Make pueda descomponer las variables fácilmente).


5. En el campo **Secret**, escribe una clave secreta inventada por ti (por ejemplo: `MiClaveSeguraGitHub123`). Esto te servirá para verificar criptográficamente que las peticiones que reciba Make provengan realmente de tu cuenta de GitHub.


6. En la sección **Which events would you like to trigger this webhook?** (¿Qué eventos deben activar este webhook?), puedes elegir:
* **Just the push event:** Se activará solo cuando alguien suba código a las ramas.


* **Let me select individual events:** Te permite elegir eventos específicos como *Pull Requests*, *Releases*, creación de *Issues*, etc.




7. Asegúrate de que la casilla **Active** esté marcada y haz clic en **Add webhook**.

---

### Paso 3: Realizar un envío de prueba y determinar la estructura en Make

Para que puedas mapear y usar las variables de GitHub en Make (como el nombre del autor, el mensaje del commit, etc.), Make necesita "aprender" cómo vienen estructurados esos datos.

1. En tu computadora, realiza una pequeña modificación en tu repositorio de GitHub y haz un *push* hacia la plataforma (o crea un commit directamente desde la interfaz web de GitHub).


2. GitHub enviará de inmediato un paquete JSON a la URL de Make.


3. Regresa a la pestaña de Make. Verás que el módulo de Webhook ha cambiado de estado y ahora muestra un mensaje de éxito como **"Successfully determined"**.


4. A partir de este momento, Make ha parseado la estructura del payload.



---

### Paso 4: Conectar y mapear los datos hacia otros módulos

Una vez que el webhook ha aprendido la estructura de datos, puedes conectar los siguientes módulos de tu flujo de trabajo:

1. Conecta un segundo módulo a la derecha del webhook (por ejemplo, **Slack > Create a Message** o **Gmail > Send an Email**).


2. Al hacer clic en los campos de configuración del nuevo módulo (como el cuerpo del mensaje), verás que el panel de variables de Make te permite arrastrar los datos exactos del envío de GitHub:


* `repository:name` (El nombre de tu repositorio)


* `pusher:name` (El usuario que hizo la actualización)
* `head_commit:message` (El mensaje que escribió el desarrollador al guardar sus cambios)
* `head_commit:url` (Un enlace directo para revisar el código en GitHub)


3. Diseña el cuerpo de tu notificación de forma dinámica:
> *"¡Hola equipo! **{{1.pusher.name}}** acaba de subir una actualización al repositorio **{{1.repository.name}}**. Mensaje del cambio: '{{1.head_commit.message}}'. Puedes revisarlo aquí: {{1.head_commit.url}}"*
> 



---

### Paso 5: Buenas prácticas y Seguridad Avanzada (Filtro HMAC)

Cualquiera que descubra la URL de tu webhook de Make podría enviar datos falsos para activar alertas ficticias. Para evitarlo, utilizaremos el **Secret** criptográfico que configuramos en GitHub mediante un filtro de validación de firmas.

GitHub envía en la cabecera HTTP de cada petición un parámetro llamado `X-Hub-Signature-256`, el cual contiene la firma digital de los datos. La validación matemática de esta firma responde a la siguiente ecuación:

$$S_{\text{computed\_github}}=\text{HMAC-SHA256}(K_{\text{secret\_github}},B_{\text{raw}})$$

Donde $K_{\text{secret\_github}}$ es la clave secreta que configuraste en GitHub, y $B_{\text{raw}}$ es el contenido crudo del payload sin procesar.

Para configurar este filtro de seguridad en Make:

1. Haz clic en el engranaje del módulo **Custom Webhook** de Make, ve a la configuración avanzada y asegúrate de cambiar la opción **Get request headers** a **Yes**.


2. Haz clic en la línea de conexión (el canal intermedio) que une el Webhook con tu módulo de Slack/Gmail para crear un **Filtro**.


3. Configura las condiciones del filtro de la siguiente manera:
* **Condición (Lado izquierdo):** Usa la función criptográfica nativa de Make para calcular el hash HMAC en tiempo real con tu clave secreta:
{{hmac(1.body; "sha256"; "LaMismaClaveSecretaQuePusisteEnGitHub"; "hex")}}
* **Operador:** Selecciona la comparación de igualdad de texto **`Equal to`**.


* **Valor (Lado derecho):** Extrae la firma enviada por GitHub en las cabeceras HTTP y quítale el prefijo de texto `"sha256="` usando la función `replace`:
{{replace(1.headers["x-hub-signature-256"]; "sha256="; "")}}





Si un atacante intenta enviar datos falsos, la firma calculada de manera local no coincidirá con la cabecera recibida, por lo que el filtro bloqueará la ejecución de inmediato. Si la firma es correcta, el flujo continuará su ejecución y enviará la notificación en tiempo real a tu equipo.