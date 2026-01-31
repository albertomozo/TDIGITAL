# TDIGITAL — Automatizaciones prácticas para pequeñas empresas 💡

**Objetivo**

Este repositorio reúne soluciones sencillas y reproducibles para automatizar tareas cotidianas en pequeñas empresas. Las soluciones están organizadas por temática y dificultad, con ejemplos, prompts para IA generativa y plantillas para acelerar la implementación. El foco principal es eficiencia práctica: soluciones que puedan implementarse con pocos recursos y herramientas accesibles (scripts, APIs, o integraciones no-code).

---

## Contenido y cómo usar este repo ✅
- /recipes/ : guías y scripts por temática y dificultad
- /templates/ : prompts y plantillas (.ics, .csv, requests)
- /examples/ : scripts de ejemplo (Python, Bash) para tareas concretas

Clona el repo y busca la temática que necesites; cada receta tendrá:
- Descripción breve
- Herramientas recomendadas
- Prompt(s) de IA sugeridos
- Pasos concretos y script mínimo viable

---

## Temáticas y automatizaciones (hoja de trucos) 🔧

### Calendarios y agendas 📅
- Fácil — Extraer eventos de un PDF y exportar a CSV/ICS
  - Descripción: extraer texto (OCR si hace falta), parsear fechas y generar .ics para importar en Google/Outlook.
  - Herramientas: `pdfplumber` o `pytesseract` + `dateparser` + `icalendar` (Python) o Zapier/Make.
  - Tiempo estimado: 1–3 horas.
- Medio — Sincronizar cambios de un calendario PDF con Google Calendar automáticamente
  - Descripción: detectar cambios, actualizar eventos mediante API de Google Calendar.
  - Herramientas: Google Calendar API, script de comparación, webhook.
  - Tiempo estimado: 1–2 días.

### Documentos y datos 📄
- Fácil — Resumir un PDF en 3–5 puntos (IA generativa)
  - Herramientas: OpenAI / local LLM + extracción de texto.
- Medio — Extraer tablas y guardarlas en Excel/Google Sheets
  - Herramientas: `tabula-py`, `camelot`, Google Sheets API.

### Comunicación y clientes ✉️
- Fácil — Generar respuestas automáticas personalizadas para consultas comunes
  - Herramientas: prompts con IA, plantillas, integración con correo (IMAP/SMTP) o WhatsApp Business.
- Medio — Chatbot FAQ para web
  - Herramientas: small LLM, embeddings (vector DB) para respuestas.

### Facturación y contabilidad 💰
- Fácil — Generar factura simple en PDF a partir de plantilla y datos
  - Herramientas: Jinja2 + WeasyPrint/ReportLab.
- Medio — Detectar facturas por correo e ingresar datos a hoja de cálculo
  - Herramientas: IMAP scraper, extracción con IA, Google Sheets API.

### Operaciones y métricas 📊
- Fácil — Generar resumen diario de ventas a partir de CSVs
  - Herramientas: Pandas + script programado (cron/Task Scheduler).
- Medio — Alertas por desviaciones en KPI (Slack / Email)
  - Herramientas: monitoring script + webhook.

---

## Caso práctico: convertir un calendario PDF a otra aplicación (guía rápida) 🛠️

1. **Extraer texto**
   - Si el PDF está como imagen: convierte páginas a imágenes y usa OCR (`pytesseract`).
   - Si es texto: usa `pdfplumber` o `PyPDF2` para extraer texto.

2. **Normalizar y parsear fechas y eventos**
   - Usa `dateparser` o expresiones regulares para detectar fechas, horas y títulos.
   - Ejemplo de prompt (para limpiar/estructurar con IA):

     "Extrae todos los eventos del siguiente texto y devuelve una lista en formato CSV con columnas: start, end, title, description, location. Usa fechas ISO (YYYY-MM-DD HH:MM). Texto: <INCRUSTAR_TEXTO_DE_PDF>"

3. **Generar salida**
   - CSV para importar a muchas apps, o ICS para calendarios.
   - En Python, usa `icalendar` para crear .ics o escribe CSV con `csv`/`pandas`.

4. **Importar / Sincronizar**
   - Importación manual: Google Calendar / Outlook admiten .ics/.csv.
   - Automatizada: usa Google Calendar API o Zapier/Make para crear eventos automáticamente.

5. **Automatizar y programar**
   - Programa un job (cron / Windows Task Scheduler) para chequeos periódicos.

---

## Prompt templates y ejemplos ✍️

- Prompt para extracción a tabla:

  "Del siguiente texto, extrae una tabla con columnas: fecha_inicio (YYYY-MM-DD HH:MM), fecha_fin (opcional), título, descripción, ubicación. Devuelve JSON array." 

- Prompt para limpiar OCR ruidoso:

  "Limpia y corrige este texto generado por OCR, corrige reconocimientos obvios y deja solo el texto legible sin marcar errores." 

---

## Recomendaciones sobre IA generativa ⚖️
- Verifica siempre la salida (especialmente fechas y montos).
- Para datos sensibles, prefiera soluciones on-prem o LLMs locales si es posible.
- Registre cambios y proporcione una revisión humana para las primeras ejecuciones.

---

## Estructura sugerida de carpetas

- recipes/
  - calendario/
    - easy-extract-pdf-to-ics/
      - README.md (pasos y prompt)
      - extract_pdf.py (script mínimo)
      - example.pdf
  - comunicaciones/
  - facturacion/
- templates/
- examples/

---

## Contribuir 🤝
1. Abre un issue con tu idea o problema.
2. Propón una receta completa (README + script + tests si aplica).
3. Sigue el estilo: claridad, reproducibilidad, privacidad y bajo coste de entrada.

---

## Licencia
MIT — ver `LICENSE`.

---

