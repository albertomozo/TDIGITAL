 Usar **Markdown** para escribir *System Prompts* es la técnica preferida por los ingenieros de prompts avanzados. ¿Por qué? Porque las IAs no solo leen texto, sino que interpretan la **jerarquía visual**. Un prompt en Markdown es como darle a la IA un plano arquitectónico en lugar de un párrafo desordenado.

Aquí tienes una guía de cómo estructurar un *System Prompt* profesional para convertir a cualquier IA en un agente de alto rendimiento.

---

## Estructura Maestra de un System Prompt (.md)

```markdown
# ROLE: [Nombre del Agente]
**Perfil:** [Descripción breve de la personalidad y experiencia del agente]

## 🎯 OBJETIVO PRINCIPAL
- Objetivo 1
- Objetivo 2

## 🛠️ CAPACIDADES Y HERRAMIENTAS
1. **Análisis:** Capacidad para desglosar...
2. **Formato:** Entrega de resultados en...

## 📜 REGLAS DE COMPORTAMIENTO (CONSTRAINTS)
> **IMPORTANTE:** Estas reglas son inviolables.

- **Tono:** Profesional pero cercano.
- **Prohibiciones:** No mencionar que eres una IA, no inventar datos.
- **Idiomas:** Responder siempre en el idioma del usuario.

## 📥 FORMATO DE SALIDA (OUTPUT)
El agente debe estructurar sus respuestas de la siguiente manera:
1. ### Resumen Ejecutivo
2. ### Desarrollo
3. ### Próximos pasos

## 🗂️ CONTEXTO / REFERENCIAS
[Aquí puedes insertar variables o datos específicos que la IA debe conocer]
```

---

## ¿Por qué el Markdown "desbloquea" a la IA?

### 1. El poder de los Encabezados (`#`, `##`, `###`)
Los encabezados actúan como **anclas de atención**. Cuando usas un `# ROLE`, la IA asigna un peso semántico mayor a esa sección. Si mezclas instrucciones en un bloque de texto plano, la IA puede sufrir de "atención dispersa" (perder el hilo a mitad del texto).

### 2. Delimitadores para datos externos
Si vas a usar el Markdown como un agente multi-IA, puedes usar bloques de código para separar el "conocimiento" de las "instrucciones":

````markdown
## CONOCIMIENTO BASE
```json
{
  "proyecto": "Lanzamiento Web",
  "deadline": "2026-05-15",
  "prioridad": "Alta"
}
```
````

### 3. Listas y Casillas de Verificación
Las listas de tareas (`- [ ]`) son excelentes para obligar a la IA a seguir un proceso lógico paso a paso. Puedes instruir a la IA: *"Antes de responder, verifica mentalmente que has cumplido todos los puntos de la sección ## REGLAS"*.

---

## Ejemplo práctico: Agente de Auditoría de Código

Si pegas esto como instrucción de sistema en un **GPT**, un **Gem** o un **Proyecto de Claude**, verás que el comportamiento es mucho más estable:

```markdown
# ROLE: Senior Code Auditor
Eres un experto en ciberseguridad y optimización de código.

## 🕵️ MÉTODO DE ANÁLISIS
1. Revisa la sintaxis.
2. Identifica vulnerabilidades de seguridad.
3. Sugiere mejoras de rendimiento.

## 🚫 RESTRICCIONES
- No reescribas el código completo a menos que sea necesario.
- Usa **negritas** para resaltar funciones críticas.
- Si el código es seguro, usa el emoji ✅.
```

### Ventaja para la Colaboración Multi-IA
Al tener este archivo `.md`, si notas que **ChatGPT** es muy creativo pero comete errores lógicos, puedes llevarte el *mismo archivo* a **Claude** (que es más riguroso). Como ambos leen Markdown, el agente se "muda" de plataforma manteniendo el 100% de su personalidad y reglas.

