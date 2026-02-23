# 🔧 Modelo de prompt completo

Un prompt efectivo combina distintos elementos para guiar al modelo hacia la respuesta deseada. Estos componentes, cuando se usan en conjunto, permiten obtener salidas más precisas y ajustadas al caso de uso.

## ✅ Elementos clave de un buen prompt

1. **Contexto y rol**
   - El rol define la voz, posición o especialización que el modelo debe adoptar ("eres un profesor", "actúa como agente de soporte").
   - El contexto aporta información de fondo (antecedentes, datos del usuario, escenario, historial de conversación, restricciones) que orienta la respuesta.

2. **Objetivo claro**
   - Indica qué necesitas que haga el modelo: redactar, explicar, resumir, generar código, etc.
   - Ejemplo: "Genera un plan de contenidos" o "Redacta un correo breve".

3. **Audiencia**
   - Especifica para quién va dirigida la respuesta. Ej: "para alumnos de 12 años", "para un cliente potencial", "para un público técnico".

4. **Tono y estilo**
   - Formal, informal, persuasivo, empático, técnico, coloquial, etc. Esto moldea la voz.

5. **Formato y estructura**
   - Lista, tabla, pasos numerados, párrafos, esquema, código, etc. Puedes pedir ejemplos o plantillas.

6. **Restricciones y límites**
   - Longitud máxima, idioma, fecha del escenario, evitar ciertas palabras, usar solo datos públicos, etc.

7. **Ejemplos o plantillas**
   - Proporciona un mini‑ejemplo para que el modelo siga un patrón.

8. **Criterios de éxito (opcional)**
   - Define condiciones que debe cumplir la respuesta (mencionar X beneficios, terminar con CTA, incluir referencias, etc.).

## 🛠️ Ejemplo de estructura completa

```text
Contexto: [breve resumen del escenario relevante].

Eres un/a [rol] especializado/a en [área]. [Instrucciones del objetivo].

- Audiencia: [persona o grupo].
- Tono: [formal/amistoso/etc.].
- Formato: [lista, tabla, párrafos…].
- Restricciones: [longitud, idioma, fecha…].

[Opcional: ejemplo o plantilla].

[Opcional: criterios de éxito].
```

💡 **Consejo:** comienza con un enunciado corto y añade elementos adicionales según sea necesario. Cuanto más específico, más enfocada será la respuesta.
