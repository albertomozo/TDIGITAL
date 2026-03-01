# Generación de documentación — Prompts de ejemplo

Este archivo reúne ejemplos de prompts en español para pedir a un modelo que genere distintos tipos de documentación: manuales, guías, fichas técnicas, tutoriales y resúmenes.

Formato recomendado:
- Rol del asistente: "Eres un redactor técnico experto en [tema]".
- Longitud: especificar (p. ej. "800–1200 palabras" o "ficha de 1 página").
- Estilo: formal/informal, dirigido a usuario final/administrador.
- Formato de salida: Markdown, HTML, o texto plano.

Ejemplos de prompts

1) Manual de usuario completo
Prompt: "Eres un redactor técnico experto en {producto}. Escribe un manual de usuario completo para {audiencia} que incluya: índice, requisitos, instalación paso a paso, ejemplos de uso, resolución de problemas y FAQ. Usa lenguaje claro, añade comandos y bloques de código donde haga falta y entrega en formato Markdown. Longitud aproximada: {longitud}."

2) Guía rápida (one-pager)
Prompt: "Genera una guía rápida de una página para {tarea} dirigida a {audiencia}. Debe incluir pasos numerados, notas de seguridad, y consejos prácticos. Formato: Markdown con encabezados y una sección "Atajos" al final."

3) Ficha técnica (spec sheet)
Prompt: "Escribe una ficha técnica para {producto/componente} con campos: descripción breve, especificaciones técnicas, compatibilidades, límites operativos, diagrama ASCII opcional y tabla de parámetros. Formato: Markdown, incluir una tabla con columnas: 'Parámetro', 'Valor', 'Unidad', 'Notas'."

4) Tutorial paso a paso con ejemplos
Prompt: "Crea un tutorial paso a paso para realizar {tarea} usando {herramienta}. Incluye pre-requisitos, comandos exactos a ejecutar, ejemplos de entrada/salida y una sección de 'Qué verificar' al final. Genera también un pequeño conjunto de pruebas para validar cada paso."

5) Índice y estructura de documentación extensa
Prompt: "Propón un índice detallado para la documentación de {proyecto} con capítulos y secciones (máx. 2 niveles). Para cada sección, añade una oración que describa su objetivo y dos bullets con ejemplos de contenido. Devuélvelo en formato de lista numerada Markdown."

6) Resumen ejecutivo de documentación técnica
Prompt: "Resume en 4–6 párrafos (no más de 350 palabras) la documentación técnica de {sistema}, enfocado a directivos: objetivos, beneficios, riesgos y próximos pasos sugeridos. Mantén un tono no técnico."

7) Convertir documentación a estilo corporativo/plantilla
Prompt: "Reescribe el siguiente texto [PON_TEXTO_AQUI] para que siga la guía de estilo corporativa: tono profesional, voz activa, sin jerga. Conserva la información técnica y mantén encabezados adecuados para exportar a PDF."

8) Checklist de revisión antes de publicar
Prompt: "Genera un checklist de revisión para publicar la documentación de {proyecto}. Incluir items sobre verificación de comandos, consistencia de versión, enlaces rotos, estilo y accesibilidad. Formato: lista de verificación con casillas."

Sugerencias de uso
- Sustituir las variables entre llaves por datos concretos.
- Indicar el formato de salida preferido (Markdown para edición, HTML para web, texto plano para emails).
- Si necesitas resultados en varios idiomas, pedir la traducción al final: "Devuélvelo en español y en inglés".

Ejemplo rápido de prompt final (lista para copiar):
"Eres un redactor técnico experto en plataformas SaaS. Escribe un manual de usuario en formato Markdown para administradores de 'Acme CRM' que incluya índice, instalación, configuración inicial, flujo de trabajo típico y resolución de problemas. Longitud: 1200–1500 palabras. Usa ejemplos reales y bloques de comandos."

---
Pulsa en el enlace desde el índice de ejemplos para usar estas plantillas.
