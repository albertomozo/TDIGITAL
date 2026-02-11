# Prompts generales para IA generativa ✅

Este archivo reúne **plantillas de prompts** y una **clasificación por temáticas** para uso cotidiano. Copia y pega las plantillas entre backticks (`) para usarlas tal cual.

---

## 💡 Tipos de prompts (plantillas)

1. **Instrucción de rol** — Define rol y contexto
```
Eres un/a [rol] experto/a en [tema]. Ayúdame a [tarea] con [restricciones] y entrega [formato].
```

2. **Tarea específica** — Ejecutar acción concreta
```
Realiza: [acción]. Datos: [entrada]. Salida: [longitud/estilo].
```

3. **Transformación de texto** — Parafrasear, resumir, traducir
```
Parafrasea/Resume/Traduce el siguiente texto al [idioma] con tono [tono] y longitud [breve/media/extendida]:
[texto]
```

4. **Generación creativa** — Ideas, títulos, guiones
```
Genera N ideas de [tema] en formato [lista/tabla] con [restricciones/ejemplos].
```

5. **Explicación / enseñanza** — Paso a paso y analogías
```
Explica [concepto] para alguien con nivel [básico/medio/avanzado], usando ejemplos y una analogía simple.
```

6. **Depuración / revisión técnica**
```
Revisa y corrige el siguiente código en [lenguaje]:
[código]
Incluye: cambios, por qué y casos de prueba sugeridos.
```

7. **Análisis de datos / SQL**
```
Escribe una consulta SQL para [objetivo] sobre la tabla [nombre] y explica la lógica en 3 bullets.
```

8. **Planificación / roadmap**
```
Crea un plan en [X] pasos para [objetivo] con hitos, entregables y tiempos estimados.
```

9. **QA / casos de prueba**
```
Genera casos de prueba para [funcionalidad] (entrada válida, entrada inválida, resultados esperados).
```

10. **Meta-prompt / optimización**
```
Optimiza este prompt para mayor claridad y brevedad: [prompt]. Devuelve versión mejorada y 2 variantes.
```

---

## 🗂️ Clasificación por temática

- **Productividad / Oficina**
  - Ejemplos: resumen de reuniones, agendas, correos.
  - Plantilla: `Resume esta reunión en 5 bullets con acciones y responsables: [texto]`

- **Escritura & Contenido**
  - Ejemplos: títulos SEO, estructura de artículos, CTA.
  - Plantilla: 
  ```Escribe un título SEO <70 caracteres para: [tema]``` 

- **Programación & DevOps**
  - Ejemplos: snippets, explicación de algoritmos, revisión de PR.
  - Plantilla: `Genera un ejemplo en [lenguaje] que muestre cómo [patrón]`

- **Datos & Analítica**
  - Ejemplos: consultas SQL, interpretación de KPIs.
  - Plantilla: `Interpreta estos resultados y sugiere 3 métricas de seguimiento: [datos]`

- **Marketing & Social**
  - Ejemplos: captions, campañas, ideas virales.
  - Plantilla: `Genera 10 captions para Instagram sobre [producto] en tono [tono]`

- **Atención al cliente & Soporte**
  - Ejemplos: respuestas estandarizadas, escalado.
  - Plantilla: `Redacta una respuesta profesional a un cliente que reclama: [problema]`

- **Educación & Formación**
  - Ejemplos: ejercicios, quizzes, adaptaciones por nivel.
  - Plantilla: `Crea 5 preguntas de opción múltiple sobre [tema] con respuestas correctas`

- **Legal / Seguridad / Compliance**
  - Ejemplos: checklist de cumplimiento, evaluación de riesgos.
  - Plantilla: `Enumera riesgos de privacidad para una app que hace: [uso de datos]`

- **Creatividad & Diseño**
  - Ejemplos: prompts para imágenes, moodboards, escenarios UX.
  - Plantilla: `Describe un moodboard para una marca con valores [x,y,z] en 6 bullets`

---

## ✅ Buenas prácticas (breve)
- Sé específico: incluye formato de salida (lista, tabla, número de items).
- Añade restricciones: longitud, tono, público objetivo.
- Pide ejemplos y un pequeño checklist o pasos a seguir.
- Itera con meta-prompts para refinar resultados.

---

## 📁 Sugerencia de uso
- Guarda este archivo en `prompts/generales.md` y referencia las plantillas en tus workflows.
- Si quieres, puedo añadir más plantillas por tema o traducirlas a otros idiomas.

---

*Creado automáticamente para facilitar el uso diario de IA generativa.*
