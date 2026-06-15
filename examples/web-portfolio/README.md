 # UNA WEB SENCILLa 
 El ecosistema actual de la IA generativa y los frameworks modernos (como Next.js, Nuxt o SvelteKit) a veces se siente como intentar matar una mosca con un cañón. Para un portfolio personal, **menos es más**.

Usar **JavaScript Vanilla (puro)** con un archivo **JSON** como base de datos y desplegarlo en un **servidor serverless moderno** (como GitHub Pages, Vercel o Netlify) es la combinación perfecta: es ultra rápido, gratis y no requiere instalaciones complejas en tu ordenador.

Aquí tienes la guía definitiva paso a paso para armar tu portfolio sin dolor de cabeza.

---

## 🛠️ Paso 1: La estructura de tu proyecto

En tu ordenador, crea una carpeta llamada `mi-portfolio` con estos tres únicos archivos. No necesitas `npm`, ni `webpack`, ni configuraciones raras.

```text
mi-portfolio/
├── index.html
├── datos.json
└── app.js

```

---

## 📄 Paso 2: El archivo de datos (`datos.json`)

Aquí guardarás toda tu información. Si el día de mañana quieres cambiar un proyecto o tu biografía, solo editas este archivo.

```json
{
  "nombre": "Tu Nombre",
  "titulo": "Desarrollador Full Stack",
  "proyectos": [
    {
      "titulo": "Chatbot con IA",
      "descripcion": "Un clon de ChatGPT usando Vanilla JS.",
      "enlace": "https://github.com"
    },
    {
      "titulo": "E-commerce Serverless",
      "descripcion": "Tienda online rápida y segura sin servidores.",
      "enlace": "https://github.com"
    }
  ]
}

```

---

## 🌐 Paso 3: El diseño (`index.html`)

El HTML será el "esqueleto". Dejaremos contenedores vacíos con `id` para que JavaScript inyecte la información.

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Portfolio Serverless</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@exampledev/new.css@1.1.2/new.min.css">
</head>
<body>
    <header>
        <h1 id="nombre">Cargando...</h1>
        <p id="titulo"></p>
    </header>

    <main>
        <h2>Mis Proyectos</h2>
        <section id="contenedor-proyectos">
            </section>
    </main>

    <script src="app.js"></script>
</body>
</html>

```

---

## 🧠 Paso 4: La lógica en JavaScript (`app.js`)

Usaremos la función moderna `fetch()` para leer el JSON e inyectar el contenido en el HTML de forma automática.

```javascript
// Esperar a que el HTML esté cargado completamente
document.addEventListener("DOMContentLoaded", () => {
    
    // 1. Consumir el archivo JSON local
    fetch('datos.json')
        .then(response => response.json())
        .then(data => {
            // 2. Inyectar los datos básicos
            document.getElementById('nombre').textContent = data.nombre;
            document.getElementById('titulo').textContent = data.titulo;

            // 3. Recorrer los proyectos y maquetarlos
            const contenedor = document.getElementById('contenedor-proyectos');
            data.proyectos.forEach(proyecto => {
                const tarjeta = document.createElement('div');
                tarjeta.style.border = "1px solid #ccc";
                tarjeta.style.padding = "10px";
                tarjeta.style.marginBottom = "10px";

                tarjeta.innerHTML = `
                    <h3>${proyecto.titulo}</h3>
                    <p>${proyecto.descripcion}</p>
                    <a href="${proyecto.enlace}" target="_blank">Ver proyecto →</a>
                `;
                contenedor.appendChild(tarjeta);
            });
        })
        .catch(error => console.error("Error cargando los datos del portfolio:", error));
});

```

---

## 🚀 Paso 5: Alojarlo gratis en la nube (Serverless con GitHub)

Para alojar esto de forma moderna y gratuita, usaremos **GitHub Pages**. Convierte tu carpeta en un servidor web global en 3 minutos:

1. **Sube tu código a GitHub:**
* Ve a [GitHub](https://github.com) y crea un repositorio nuevo (ej. `mi-portfolio`).
* Sube tus 3 archivos (`index.html`, `app.js`, `datos.json`) directamente arrastrándolos a la web de GitHub o mediante la terminal.


2. **Activa el servidor (GitHub Pages):**
* Dentro de tu repositorio en GitHub, ve a la pestaña **Settings** (Configuración) en el menú superior.
* En la barra lateral izquierda, busca la sección **Pages**.
* En el apartado *Build and deployment -> Source*, asegúrate de que esté seleccionado **Deploy from a branch**.
* Abajo, en *Branch*, cambia `None` por **`main`** (o `master`) y la carpeta `/root`. Haz clic en **Save**.



¡Listo! Espera un minuto, refresca la página de *Settings -> Pages* y verás un enlace azul arriba (tipo `https://tu-usuario.github.io/mi-portfolio/`).

### 💡 ¿Por qué es esto "Serverless"?

Porque tú no administras ningún servidor, no pagas mantenimiento, no hay bases de datos SQL complejas corriendo en segundo plano ni configuraciones de Node.js. GitHub funciona como una infraestructura estática global (CDN): cada vez que un usuario entra a tu enlace, GitHub le sirve tu HTML, JS y JSON de forma inmediata, segura y capaz de soportar miles de visitas simultáneas a coste cero.