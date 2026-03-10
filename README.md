# TDIGITAL — Automatizaciones básicas con IA generativa 🤖

**Propósito**

Este repositorio reúne recetas prácticas y minimalistas para automatizar tareas de oficina usando **IA generativa**. Cada receta incluye:

- Un **prompt listo para usar**
- Pasos claros para ejecutar la receta
- Una **comprobación mínima** para validar resultados

> ⚠️ Siempre revisa manualmente los resultados de la IA antes de usarlos en producción.

---

## 🚀 Cómo usar este repositorio

1. Navega a la carpeta de la temática que quieras automatizar.
2. Copia el prompt y el texto/archivo de entrada en tu IA preferida (ChatGPT, Gemini, etc.).
3. Ejecuta el prompt y valida los resultados.

---

## 🔎 Contenido principal

- `calendario/` — Prompts y ejemplos para extraer eventos de PDFs y generar CSV/ICS.
- `actas/` — Plantillas y prompts para generar actas/minutas a partir de transcripciones o notas.
- `prompts/` — Colección de prompts generales y plantillas reutilizables.
- `examples/` — Ejemplos de entrada/salida que ayudan a entender cómo usar cada receta.

---

## 🧩 Ejemplo rápido: extraer eventos de un calendario PDF

Basado en `calendario/pdf-calendario.md`.

1. Extrae el texto del PDF (si tu IA admite carga de archivos, súbelo; si no, usa OCR).
2. Usa este prompt:

   > "Actúa como un experto en gestión de datos. Lee este calendario y extrae todos los eventos. Devuélvelos como **CSV** con columnas exactas: Subject, Start Date (DD/MM/AAAA), Start Time (HH:MM AM/PM), End Date, End Time, Description. No añadas texto extra fuera del CSV."

3. Copia el CSV generado y guárdalo como `micurso.csv`.
4. Verifica las fechas y horas antes de importarlo en Google Calendar/Outlook.

---

## 🛠️ Cómo colaborar

- Abre un *issue* con ideas o mejoras de prompts.
- Envía un *pull request* con nuevas recetas, ejemplos o mejoras de documentación.

---

## 📄 Licencia

MIT
