

Cuando pasas de usar un solo prompt a gestionar archivos Markdown, estás haciendo **Ingeniería de Prompts Modular**. Aquí tienes los otros 3 usos avanzados que transforman a una IA genérica en una herramienta de nivel industrial:

---

## 1. El "Library.md" (Biblioteca de Conocimiento)
A diferencia del `skill.md` (que dice *cómo* actuar), el archivo de biblioteca le da a la IA la **materia prima**.
* **Uso:** Guardas aquí glosarios técnicos, datos específicos de tu empresa, histórico de proyectos o normativas legales.
* **Por qué funciona:** Evitas que la IA alucine. En lugar de decir "inventa una solución", le dices: *"Usa la solución basada en los estándares del archivo `library_normativas.md`"*.

## 2. El "Style_Voice.md" (Manual de Identidad)
Este es vital si generas contenido para redes, blogs o correos corporativos.
* **Contenido:** Define el tono (¿satírico?, ¿sobrio?), la longitud media de las frases, palabras prohibidas y el uso de emojis.
* **Uso avanzado:** Puedes incluir un **"Golden Example"**, un texto que tú escribiste y que es perfecto, para que la IA extraiga el ADN de tu escritura mediante *Few-shot prompting*.

## 3. El "Master_Orchestrator.md" (El Director de Orquesta)
Este es el nivel más alto. Es un archivo que no tiene una habilidad, sino que **gestiona a otras IAs**.
* **Cómo funciona:** Si tienes un proyecto complejo, el Orquestador decide qué "Skill" debe activarse en cada paso.
* **Ejemplo de flujo:**
    1.  El Orquestador lee tu petición.
    2.  Llama a `analista_datos.md` para procesar un CSV.
    3.  Llama a `redactor_creativo.md` para presentar los resultados en un post de LinkedIn.
    4.  Llama a `traductor.md` para pasarlo a inglés.

---

## 📊 Comparativa de Archivos de Configuración

| Archivo | Función Principal | Analogía Real |
| :--- | :--- | :--- |
| **`skill.md`** | Definir capacidades y reglas. | El CV y contrato del empleado. |
| **`context.md`** | Dar información sobre el proyecto actual. | El briefing de la reunión. |
| **`style.md`** | Definir la personalidad y estética. | El manual de marca. |
| **`workflow.md`** | Definir pasos lógicos obligatorios. | El protocolo de actuación (SOP). |

---

## 💡 El Truco Maestro: Variables en Markdown
Puedes dejar huecos en tus archivos `.md` para rellenarlos sobre la marcha. Por ejemplo, en tu archivo de transformación digital, podrías poner:

`[SECTOR_CLIENTE]: {{Insertar sector aquí}}`

Así, cuando pegas el prompt, solo tienes que rellenar la variable y la IA adapta toda su "habilidad" a ese sector específico de forma instantánea.

**¿Te interesa que diseñemos un archivo de "Style_Voice" para que la IA escriba exactamente como tú, o prefieres profundizar en cómo crear un "Orquestador"?**  