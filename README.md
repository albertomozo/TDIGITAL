# 🚀 TDIGITAL — Automatizaciones con IA Generativa y Transformación Digital

**Repositorio educativo y práctico de soluciones, prompts, automatizaciones y recursos para la Transformación Digital**

---

## 📋 Índice rápido

- [Descripción](#descripción)
- [Estructura del repositorio](#estructura-del-repositorio)
- [Cómo usar este repo](#cómo-usar-este-repo)
- [Secciones principales](#secciones-principales)
- [Cómo colaborar](#cómo-colaborar)

---

## 📝 Descripción

Este repositorio es un **hub centralizado** que combina:

1. **Automatizaciones prácticas** — Recetas paso a paso para automatizar tareas cotidianas (calendarios, actas, formularios, webhooks).
2. **Ingeniería de Prompts** — Plantillas, patrones y ejemplos de prompts estructurados para IA generativa.
3. **Guías educativas** — Manuales sobre Markdown, IA, Transformación Digital y mejores prácticas.
4. **Ejemplos funcionales** — Proyectos de demostración (dashboards, itinerarios, gestores de tareas, portfolios).

**Público objetivo:**
- Docentes y estudiantes de Transformación Digital
- Pequeñas empresas buscando automatizar procesos
- Profesionales que desean usar IA de forma efectiva
- Desarrolladores interesados en soluciones no-code y low-code

> ⚠️ **Nota importante**: Siempre valida manualmente los resultados generados por IA antes de usarlos en producción.

---

## 📁 Estructura del repositorio

```
TDIGITAL/
├── PROMPTS/                    # Plantillas y ejemplos de prompts
│   ├── 00-modelo.md           # Estructura base de un prompt efectivo
│   ├── 01-rol.md              # Cómo definir roles para la IA
│   ├── 02-contexto.md         # Inclusión de contexto y datos
│   ├── generales.md           # Colección de prompts genéricos
│   └── ejemplos/              # Prompts aplicados a casos reales
│
├── markdown/                   # Manual completo de Markdown
│   ├── manual.md              # Introducción y filosofía
│   ├── sintaxis.md            # Referencia de sintaxis
│   ├── ejercicios.md          # Ejercicios prácticos
│   ├── soluciones.md          # Soluciones de ejercicios
│   ├── futuro.md              # Tendencias y IA
│   ├── guia_skill.md          # Markdown para "skills" de IA
│   ├── ficheros.md            # Ingeniería modular de prompts
│   └── skills/                # Ejemplos de habilidades estructuradas
│
├── IA/                         # Guías de IA y Transformación Digital
│   ├── chatgpt_usos.md        # Casos prácticos de ChatGPT
│   ├── chatgpt_guia_TD.md     # ChatGPT en Transformación Digital
│   ├── chatgpt_GPT.md         # Introducción a modelos GPT
│   ├── chatgpt_GPT_2.md       # Ejemplos avanzados
│   ├── linea_tiempo_claude.html # Cronología de Claude
│   ├── linea_tiempo_mistral.md  # Cronología de Mistral
│   └── [más ejemplos interactivos]
│
├── PROMPTS/ejemplos/           # Ejemplos prácticos de prompts
│   ├── investigacion.md        # Prompts para investigación
│   ├── soporte.md              # Prompts para atención al cliente
│   ├── educacion.md            # Prompts educativos
│   ├── generacion-documentacion.md
│   └── [más ejemplos por sector]
│
├── calendario/                 # Automatizaciones de eventos y fechas
│   └── pdf-calendario.md       # Extraer eventos de PDFs a CSV/ICS
│
├── actas/                      # Automatizaciones de minutas y actas
│   └── hoja-de-trucos-minutas.md
│
├── automatizacones/            # Integraciones no-code
│   ├── google-forms-sheets-slack.md
│   ├── preguntas-google-forms.md
│   └── [diagramas y recursos]
│
├── API/                        # Integración de APIs y webhooks
│   └── webhook-make-github.md  # Webhooks con Make/Zapier
│
├── PTD/                        # Guías de Programación (Projects/Prompts)
│   ├── guia_Claude_Projects_PTD.md
│   └── guia_PTD_con_prompts_IA.md
│
├── examples/                   # Proyectos de demostración
│   ├── dashboard-cafe/         # Dashboard de ejemplo
│   ├── itinerarios/            # Planificador de viajes (CSV y Markdown)
│   ├── todolist/               # Gestor de tareas y auditoría
│   └── web-portfolio/          # Portfolio web de muestra
│
├── assets/                     # Plantillas y recursos
│   └── [plantillas varias]
│
├── form-jotfor/                # Formularios (JotForm)
│
├── mistackIA/                  # Prompts experimentales/avanzados
│
└── resumen/                    # Hojas de trucos y resúmenes
```

---

## 🎯 Cómo usar este repo

### Opción 1: Copiar prompts listos
1. Ve a `PROMPTS/` y elige un ejemplo que se ajuste a tu caso.
2. Copia el prompt.
3. Personaliza los marcadores `[entre corchetes]`.
4. Pega en ChatGPT, Gemini, Claude o tu IA preferida.

### Opción 2: Automatizar una tarea
1. Identifica la temática en `calendario/`, `actas/`, `automatizacones/` o `API/`.
2. Lee la guía (`.md`) para entender los pasos.
3. Usa los prompts sugeridos o adapta los de `PROMPTS/`.
4. Implementa con las herramientas recomendadas (Make, Zapier, scripts Python, etc.).

### Opción 3: Aprender sobre Markdown y mejores prácticas
1. Estudia `markdown/manual.md` para conceptos.
2. Resuelve los ejercicios en `markdown/ejercicios.md`.
3. Consulta `markdown/futuro.md` para tendencias con IA.

### Opción 4: Explorar ejemplos funcionales
1. Revisa `examples/` para ver dashboards, itinerarios, gestores de tareas.
2. Replica el código o la estructura en tu propio proyecto.

---

## 🔍 Secciones principales

### 📌 **PROMPTS/** — Ingeniería de Prompts
Aprende a estructurar prompts efectivos:
- **00-modelo.md**: Los 5 elementos clave de un buen prompt (rol, contexto, tarea, restricciones, formato).
- **01-rol.md**: Define quién es la IA (profesor, experto en marketing, etc.).
- **02-contexto.md**: Aporta información de fondo para mejores respuestas.
- **generales.md**: 50+ prompts clasificados por uso (escritura, análisis, creatividad, etc.).
- **ejemplos/**: Prompts reales para investigación, soporte, educación, documentación y más.

### 📚 **markdown/** — Manual de Markdown
Guía completa y educativa:
- Teoría y variantes (CommonMark, GFM, Markdown con IA).
- Sintaxis: encabezados, listas, tablas, código, links, imágenes.
- Ejercicios prácticos con soluciones.
- Tendencias: cómo Markdown + IA revoluciona la documentación.
- **Skills**: Cómo estructurar instrucciones para mejorar prompts.

### 🤖 **IA/** — Inteligencia Artificial en Transformación Digital
Casos de uso y guías:
- Cómo usar ChatGPT, Claude y Mistral en procesos empresariales.
- Líneas de tiempo interactivas (evolución de modelos).
- Ejemplos de visualizaciones (ciclo del agua, evolución de especies con IA).
- Guías específicas de Transformación Digital.

### 📅 **calendario/** — Automatización de eventos
Receta para extraer eventos de PDFs:
- Parsear fechas y horarios.
- Generar CSV para importar en Excel.
- Crear archivos ICS para Google Calendar / Outlook.
- Sincronización automática con webhooks.

### 📋 **actas/** — Automatización de minutas
Genera actas profesionales a partir de:
- Transcripciones de reuniones.
- Notas de voz.
- Uso de IA para extraer asuntos clave, decisiones y responsables.

### ⚙️ **automatizacones/** — Flujos no-code
Integraciones entre herramientas populares:
- Google Forms → Google Sheets → Slack (notificaciones automáticas).
- Zapier / Make para orquestar procesos.
- Ejemplos con diagramas visuales.

### 🔌 **API/** — Webhooks e integraciones
Automatizaciones basadas en eventos:
- Webhooks de GitHub hacia Make/Zapier.
- Triggers y acciones en cadena.
- Casos de uso prácticos.

### 🎓 **PTD/** — Claude Projects y Prompts
Guías para usar Claude Projects (Anthropic):
- Cómo estructurar un proyecto.
- Uso de prompts personalizados dentro de Projects.
- Mejores prácticas para equipos.

### 🎨 **examples/** — Proyectos demostración
Ejemplos funcionales listos para copiar:
- **dashboard-cafe/**: Dashboard simple con Markdown.
- **itinerarios/**: Planificador de viajes con CSV y Markdown.
- **todolist/**: Gestor de tareas con auditoría.
- **web-portfolio/**: Portfolio personal con HTML/CSS.

---

## 🤝 Cómo colaborar

**¿Tienes una automatización nueva, un prompt útil o una mejora?**

1. **Abre un issue** si tienes una idea o encuentras un error.
2. **Envía un PR** con:
   - Nuevas recetas o prompts (en la carpeta apropiada).
   - Mejoras en documentación.
   - Ejemplos funcionales.
   - Correcciones o clarificaciones.

**Criterios para PRs:**
- El contenido debe ser práctico y verificable.
- Incluye ejemplos o pasos claros.
- Usa Markdown correctamente (sigue `markdown/sintaxis.md`).
- Actualiza el índice de la sección correspondiente.

---

## 📄 Licencia

MIT — Siéntete libre de usar, modificar y distribuir este contenido.

---

## 📞 Contacto y soporte

- Abre un **issue** en GitHub para preguntas o sugerencias.
- Revisa las **discussions** para conversar sobre temas generales.
- Contribuye con tus propios ejemplos y mejoras.

---

**Última actualización**: Junio 2026  
**Mantenedor**: Alberto Mozo (@albertomozo)  
**Estado**: En desarrollo activo — Se añaden nuevas secciones regularmente.

---

## 🎯 Roadmap futuro

- [ ] Sección de automatizaciones con Python/Node.js
- [ ] Librerías de prompts por industria (ventas, educación, finanzas).
- [ ] Tutoriales en video.
- [ ] Herramientas de evaluación de prompts.
- [ ] Base de datos de casos de éxito.
- [ ] Enlazar otras herramientas.
- [ ] Prototipos alumnos.
