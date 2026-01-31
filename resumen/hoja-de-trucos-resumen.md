# Hoja de Trucos — Resúmenes de informes/PDFs (3–5 puntos) 📄✂️

**Propósito**

Guía mínima para usar IA generativa y transformar un informe o PDF en un resumen claro de 3–5 puntos accionables. Ideal para minutas, emails y decisiones rápidas.

---

## Prompts listos (copia y pega) ✍️

- **Prompt (subiendo PDF al chat):**
```prompt
  "Actúa como un editor ejecutivo. Lee el archivo PDF adjunto y resume el documento en **3–5 puntos** claros y accionables. Cada punto debe tener máximo 20 palabras. Al final, añade una línea `Clave:` con la idea principal (6–8 palabras). Devuélvelo únicamente como lista numerada y la línea `Clave:`. No añadas texto adicional."
```
- **Prompt (pegando texto):**
```prompt

  "Actúa como un editor ejecutivo. Del siguiente texto extrae **3–5 puntos** accionables y una línea `Clave:` que resuma la idea principal. Limita cada punto a 1 frase. Texto: <PEGA_AQUI_EL_TEXTO>"
  ```

- **Variación (nivel técnico):**
```prompt

  "Resume en 3–5 puntos; por cada punto, añade una sub-línea `Riesgos/Acción` (máx. 10 palabras) si aplica. Devuelve JSON con `summary` (array) y `key` (string)."
```
---

## Pasos rápidos (2 minutos) ⏱️

1. Si es PDF, súbelo al chat de la IA o extrae texto con OCR.
2. Pega el prompt apropiado y ejecuta.
3. Revisa números, fechas y nombres (validación humana obligatoria).
4. Copia el resumen al email, minuta o nota de reunión.

---

## Ejemplo

Entrada (extracto breve):

"El informe muestra un crecimiento del 8% en ventas Q1, pero retrasos en logística incrementan tiempos de entrega. Se propone aumentar stock crítico y mejorar comunicación con proveedores."

Salida esperada:

1. Aumentar stock crítico para productos con alta rotación.
2. Mejorar comunicación con proveedores para reducir retrasos.
3. Monitorizar tiempos de entrega semanalmente y reportar a gerencia.

Clave: Priorizar stock y coordinación logística.

---

## Checklist de validación ✅

- ¿Las cifras y fechas son correctas?
- ¿Faltan secciones importantes (metodología, conclusiones)?
- ¿El tono es apropiado para el destinatario?
- ¿Es accionable cada punto? (si no, pedir reescritura con "hazlo más accionable")

---

## Consejos prácticos 💡

- Sé explícito en el prompt sobre longitud, formato y lenguaje (formal/informal).
- Para capturas rápidas, pide salida en `CSV` o `JSON` si quieres procesarla automáticamente.
- Si el documento es sensible, evita subirlo a servicios públicos; usa modelos locales si es posible.

---

## Ubicación sugerida

Guarda este fichero en `resumen/` y copia el prompt a `templates/prompts.md` para reutilizarlo.

---

¿Quieres que añada un ejemplo real (archivo de entrada y respuesta de IA) en `examples/resumen/` para que puedas probar directamente? 🔧