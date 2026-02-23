# 📋 ¿Qué es un *prompt* con contexto?

En este epígrafe combinamos dos elementos clave: el **rol** que debe asumir el modelo y el **contexto** que rodea a la solicitud. El rol define la voz o posición (por ejemplo, "eres un profesor"), mientras que el contexto aporta información de fondo que ayuda a orientar la respuesta.

Un **prompt que hace referencia al contexto** incluye datos adicionales —como antecedentes, escenario actual o información del usuario— para que el modelo pueda responder de forma más adecuada. El patrón es:

```text
[Contexto: descripción breve de lo relevante].
[Eres un/a ...] [Instrucciones específicas].
```

> El contexto puede ser un párrafo, una lista de puntos o datos concretos. Se coloca al principio para que el modelo lo asimile antes de ejecutar la tarea.

---

## 🧩 Tipos de contextos frecuentes

- **Antecedentes del proyecto**: descripción de la empresa, público objetivo, objetivos previos.
- **Escenario específico**: "Estamos en una campaña navideña", "año fiscal 2025".
- **Historial de conversación**: "El cliente ya preguntó sobre precios".
- **Datos del usuario**: edad, ubicación, rol, intereses.
- **Restricciones o recursos**: presupuesto disponible, herramientas usadas.

---

## ✍️ Ejemplos listos para copiar y pegar

### 🎯 Marketing con antecedentes
```text
Contexto: La marca "EcoBotellas" vende botellas reutilizables y quiere aumentar ventas online en mayo.
Eres un experto en marketing digital. Propón una campaña de email marketing con títulos, segmentación y calendario.
```

### 🎓 Educación con escenario
```text
Contexto: Clase de biología para 3.° de ESO, unidad sobre células animales.
Eres profesora de secundaria. Explica la diferencia entre mitocondrias y cloroplastos con ejemplos cotidianos.
```

### 🤝 Soporte con historial de conversación
```text
Contexto: El cliente ya ha intentado restablecer su contraseña sin éxito.
Eres un agente de soporte técnico. Indica pasos adicionales y cómo ponerse en contacto si falla de nuevo.
```

### 💼 Ventas con datos de usuario
```text
Contexto: El prospecto es director de recursos humanos en una pyme de 50 empleados.
Eres un vendedor de software de nómina. Redacta un mensaje destacando facilidad de uso y ahorro de tiempo.
```

### 🏥 Salud con restricciones
```text
Contexto: Paciente vegetariano, sin alergias, quiere plan de comidas con 1.800 kcal diarias.
Eres nutricionista. Diseña un menú semanal equilibrado respetando las calorías.
```

> 🔁 Ajusta el contexto y la instrucción según necesites. Incluye elementos clave antes de pedir la tarea para obtener respuestas más precisas.
