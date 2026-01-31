# TDIGITAL — Automatizaciones básicas con IA generativa 🤖

**Propósito (muy sencillo)**

Este repositorio ofrece soluciones prácticas y mínimas, basadas únicamente en IA generativa, para automatizar tareas cotidianas de oficina. Cada receta incluye: un prompt listo para usar, pasos claros y una comprobación mínima que haga falta.

---

## Cómo usar este repositorio ✅
- Abre la carpeta de la temática que necesites.
- Copia el *prompt* y el texto (o archivo) que quieras procesar en tu chat de IA preferido (ChatGPT, Gemini, etc.).
- Revisa y valida manualmente los resultados antes de importarlos o compartirlos.

---

## Automatizaciones sencillas (hoja de trucos) 🔧
- **Calendarios / Agendas** 📅 — Extraer eventos de un PDF y generar CSV/ICS.
- **Resúmenes** 📄 — Resumir un informe o PDF en 3–5 puntos.
- **Emails** ✉️ — Redactar respuestas o plantillas personalizadas a partir de párrafos y datos.
- **Actas / Minutas** 📝 — Generar minuta de reunión a partir de una transcripción o apuntes.
- **Tablas a CSV** 📊 — Extraer tablas copypasteadas y convertir a CSV.
- **Textos comerciales** 💬 — Crear 3 variantes de un post o anuncio a partir de una sola idea.

---

## Ejemplo práctico (extraer eventos de un calendario PDF) 🛠️

Basado en `calendario/pdf-calendario.md`.

1. Extrae el texto del PDF (si tu IA acepta archivos, súbelo; si no, copia el texto extraído con OCR).
2. Usa este prompt (pega el texto o sube el PDF junto con el prompt):

   "Actúa como un experto en gestión de datos. Lee este calendario y extrae todos los eventos. Devuélvelos como **CSV** con columnas exactas: Subject, Start Date (DD/MM/AAAA), Start Time (HH:MM AM/PM), End Date, End Time, Description. No añadas texto extra fuera del CSV."

3. Copia el CSV generado, guárdalo como `micurso.csv` y **valida las fechas/horas**.
4. Importa en Google Calendar/Outlook o conviértelo a ICS si prefieres.

> Nota: siempre revisa los resultados de la IA para fechas y horas; la revisión humana es obligatoria en esta etapa.

---

## Estructura sugerida (simple)
- `calendario/` — prompts y ejemplo (`pdf-calendario.md` ya contiene el prompt).
- `templates/` — prompts comunes y plantillas de salida (CSV, ICS, email).
- `examples/` — ejemplos de entrada y salida (pueden ser solo textos y archivos de ejemplo).

---

## Contribuir
- Abre un *issue* con tu idea o con un prompt mejorado.
- Envía un *pull request* con un `README` y un ejemplo (texto + prompt).

---


Licencia: MIT
