# PTD — Plan de Transformación Digital

Esta carpeta contiene los modelos, guías y documentos base para crear casos concretos de Planes de Transformación Digital (PTD).

## Índice rápido

- 📌 [Objetivo](#objetivo)
- 📁 [Contenido de la carpeta](#contenido-de-la-carpeta)
  - 🧩 [Plantillas](#plantillas)
  - 📚 [Guías](#guías)
  - 🗂️ [Documentación de artefactos](#documentación-de-artefactos)
- ✅ [Recomendación de uso](#recomendación-de-uso)
- 🧭 [Propuesta de estructura de repositorio](#propuesta-de-estructura-de-repositorio)
- 💡 [Conceptos clave](#conceptos-clave)
- 🛠️ [Sugerencias prácticas](#sugerencias-prácticas)
- 🚀 [Flujo recomendado](#flujo-recomendado)

## Objetivo

- `PTD_01_plantilla.md` y `PTD_02-plantilla.md` son los modelos principales para generar planes reales.
- `PTD_02-plantilla.md` es la versión más completa y se recomienda usarla como **documento fuente de verdad**.
- Las guías `guia_PTD_con_prompts_IA.md` y `guia_Claude_Projects_PTD.md` explican cómo usar IA para generar contenidos y gestionar el proyecto.
- `documentos.md` describe los artefactos derivados que se pueden extraer del PTD.

## Contenido de la carpeta

### Plantillas
- `PTD_01_plantilla.md`
  - Plantilla base para un PTD más sencillo.
- `PTD_02-plantilla.md`
  - Plantilla ampliada y estructurada como fuente de verdad.
- `PTD_02-plantilla.docx`
  - Versión en Word compatible con edición offline y revisión colaborativa.

### Guías
- `guia_PTD_con_prompts_IA.md`
  - Lista de prompts para generar cada sección del PTD con IA.
- `guia_Claude_Projects_PTD.md`
  - Guía para usar Claude Projects o proyectos similares como espacio de trabajo persistente.

### Documentación de artefactos
- `documentos.md`
  - Explica los diferentes documentos y artefactos que pueden salir del PTD como entregables.
- `documentos.png`
  - Representación visual de las categorías de artefactos derivados del PTD.

## Recomendación de uso

1. Usa `PTD_02-plantilla.md` como documento principal de trabajo.
2. Completa los apartados con información real del caso concreto.
3. Genera los artefactos derivados a partir de la información del PTD.
4. Utiliza las guías de prompts para pedir a la IA los contenidos necesarios.
5. Conserva el PTD original como única fuente de verdad y actualiza los artefactos con base en él.

## Propuesta de estructura de repositorio

Se sugiere una organización más clara si el proyecto crece con casos reales y entregables:

```
PTD/
  README.md
  templates/
    PTD_01_plantilla.md
    PTD_02-plantilla.md
    PTD_02-plantilla.docx
  guides/
    guia_PTD_con_prompts_IA.md
    guia_Claude_Projects_PTD.md
  catalog/
    documentos.md
    documentos.png
  casos/
    [cliente]_PTD.md
    [cliente]_artefacto_folleto.md
    [cliente]_informe_ejecutivo.md
```

## Conceptos clave

- **PTD**: Plan de Transformación Digital.
- **Fuente de verdad**: el documento completo que recopila la información estratégica y operativa del proyecto.
- **Documento particular**: un PTD específico para un cliente o caso concreto.
- **Artefacto**: entregable derivado, como folleto, nota de prensa, propuesta de inversión, slide deck, infografía o plan de formación.
- **Guía de prompts**: manual para solicitar a la IA los contenidos que alimentan las plantillas.

## Sugerencias prácticas

- Mantén las plantillas (`PTD_01`, `PTD_02`) limpias y sin datos de caso específico.
- Crea un nuevo archivo en `casos/` para cada cliente o proyecto real.
- Extrae los artefactos en una carpeta separada para mantener la trazabilidad.
- Usa nombres claros y consistentes: por ejemplo `2026-empresaX_PTD.md` y `2026-empresaX_folleto.md`.

## Flujo recomendado

1. Crear caso real usando `PTD_02-plantilla.md`.
2. Completar diagnóstico estratégico y mapeo de herramientas.
3. Extraer artefactos según `documentos.md`.
4. Revisar y validar con el equipo o cliente.
5. Guardar versiones y referencias en la estructura propuesta.
