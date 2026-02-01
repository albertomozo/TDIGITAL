# Hoja de Trucos — Actas / Minutas a partir de transcripciones 📝

**Propósito**

Guía mínima para usar IA generativa y transformar una transcripción o apuntes en una minuta útil: resumen ejecutivo, decisiones, y lista de acciones con responsables y fechas.

---

## Prompts listos (copia y pega) ✍️

- **Prompt básico (subiendo la transcripción):**

  "Actúa como un secretario ejecutivo. Lee la transcripción adjunta y genera una minuta clara con las secciones: `Fecha`, `Asistentes`, `Resumen ejecutivo` (3–5 puntos), `Decisiones` (lista), `Acciones` (lista con responsable y fecha límite), `Próxima reunión`. Devuélvelo en texto plano sin explicaciones adicionales."

- **Prompt pegando texto (rápido):**

  "Actúa como un secretario y resume el siguiente texto en una minuta con: 1) Resumen ejecutivo (máx. 5 puntos), 2) Decisiones, 3) Acciones con responsable y fecha límite. Devuélvelo como texto con encabezados claros. Texto: <PEGA_AQUI>"

- **Prompt para salida estructurada (JSON):**

  "Convierte la transcripción en un objeto JSON con campos: `date`, `attendees` (array), `summary` (array de strings), `decisions` (array), `actions` (array de {task,responsible,due_date}), `next_meeting` (string/null). Devuélvelo SOLO como JSON." 

- **Prompt para extraer solo acciones:**

  "Extrae únicamente las acciones de la transcripción en formato CSV con columnas: task,responsible,due_date. Si falta responsable o fecha, deja el campo vacío." 

---

## Pasos rápidos (2–5 minutos) ⏱️

1. Obtén la transcripción (archivo de texto o copia del chat/voz → texto).
2. Limpia ruidos básicos (correcciones de nombres, marcas de tiempo si quieres).
3. Ejecuta el prompt apropiado en tu modelo de IA.
4. Revisa y confirma **responsables y fechas**; corrige manualmente si hace falta.
5. Distribuye la minuta por email o canal (Slack/Teams) y guarda en el repositorio.

---

## Plantilla de minuta (ejemplo)

Fecha: 2026-01-31

Asistentes: Ana, Carlos, María

Resumen ejecutivo:
1. Aumentar stock de productos críticos para febrero.
2. Revisar los contratos con proveedor X.
3. Implementar control semanal de entregas y KPI.

Decisiones:
- Aprobar presupuesto extra de 5k para stock.
- Cambiar proveedor opcional si no mejora comunicación.

Acciones:
- Revisar proveedores (Carlos) — 2026-02-05
- Preparar orden de compra (Ana) — 2026-02-03
- Crear dashboard de entregas (María) — 2026-02-07

Próxima reunión: 2026-02-10, 10:00

---

## JSON schema de ejemplo

{
  "date": "YYYY-MM-DD",
  "attendees": ["Ana","Carlos"],
  "summary": ["Punto 1","Punto 2"],
  "decisions": ["Decisión A"],
  "actions": [{"task":"Tarea","responsible":"Nombre","due_date":"YYYY-MM-DD"}],
  "next_meeting": "YYYY-MM-DD HH:MM" || null
}

---

## Checklist de validación ✅

- ¿Los nombres y cargos son correctos?
- ¿Todas las acciones tienen responsable y fecha (o se marcó como pendiente)?
- ¿Las decisiones están claramente identificadas y sin ambigüedad?
- ¿El resumen refleja las prioridades (3–5 puntos)?
- ¿Hay consenso sobre los próximos pasos antes de distribuir?

---

## Consejos prácticos 💡

- Si la transcripción incluye marcas de tiempo, pide al modelo que las incluya junto a cada acción o decisión.
- Para reuniones sensibles, evita subir la transcripción a servicios externos; usa modelos locales o pide al asistente que resuma offline si es posible.
- Pide al modelo generar también un `Email listo para enviar` con el asunto y cuerpo breve para distribuir la minuta.

---

## Ubicación sugerida

Guarda esta hoja en `actas/` y añade el prompt preferido a `templates/prompts.md` para reutilizarlo.

---

¿Quieres que añada un ejemplo real (transcripción + minuta esperada) en `examples/actas/` y un pequeño script que convierta la salida JSON a un correo listo para enviar? ✉️