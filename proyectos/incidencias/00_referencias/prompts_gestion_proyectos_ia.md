# Biblioteca de prompts: gestión de proyectos con inteligencia artificial

**Versión:** 1.0  
**Formato:** Markdown portable  
**Ámbito:** proyectos de distintos sectores, tamaños y metodologías  
**Uso:** copiar, sustituir variables entre corchetes, ejecutar, revisar y aprobar resultados.

> Los textos entre corchetes, como `[NOMBRE_PROYECTO]`, son **marcadores de posición** que debes sustituir por tus propios datos. Si un dato no se conoce, indica `PENDIENTE` y solicita a la IA que lo identifique como supuesto, nunca como hecho. Las referencias a las plantillas 02, 05, 07, 10, 13, 16, 22 y 24 son opcionales y pueden adaptarse a tu propia biblioteca.

## 1. Ficha de variables del proyecto

Copia esta ficha al inicio de cada conversación o guárdala como documento de contexto.

| Variable | Qué debes introducir |
|---|---|
| `[NOMBRE_PROYECTO]` | Nombre corto y reconocible |
| `[DESCRIPCION_PROYECTO]` | Qué se quiere hacer y por qué |
| `[PROBLEMA_NECESIDAD]` | Necesidad, oportunidad o problema |
| `[ORGANIZACION_CONTEXTO]` | Empresa, entidad, área y contexto |
| `[DESTINATARIOS_USUARIOS]` | Usuarios, clientes o beneficiarios |
| `[OBJETIVO_PRELIMINAR]` | Resultado deseado, aunque aún no sea SMART |
| `[FECHA_INICIO]` | Fecha de arranque prevista |
| `[FECHA_OBJETIVO]` | Fecha límite o lanzamiento deseado |
| `[FECHA_CIERRE]` | Fecha prevista de cierre o evaluación |
| `[PRESUPUESTO_MAXIMO]` | Presupuesto y moneda, o PENDIENTE |
| `[RECURSOS_DISPONIBLES]` | Personas, dedicación, herramientas y medios |
| `[ROLES_Y_RESPONSABLES]` | Patrocinador, coordinación, equipo y usuarios |
| `[ENTREGABLES_PRELIMINARES]` | Productos, servicios o resultados esperados |
| `[RESTRICCIONES]` | Limitaciones, normas, calendario, tecnología |
| `[EXCLUSIONES]` | Trabajo que no debe incluirse |
| `[CRITERIOS_EXITO]` | Indicadores y requisitos de aceptación |
| `[METODOLOGIA]` | Predictiva, Kanban, Scrum, híbrida u otra |
| `[HERRAMIENTAS]` | Aplicaciones disponibles para gestión y documentación |
| `[DOCUMENTOS_APROBADOS]` | Texto o enlaces verificables de documentos validados |
| `[INCIDENCIA_REAL_O_SIMULADA]` | Descripción del evento, fecha, efectos y estado |
| `[FECHA_INFORME]` | Fecha de corte del seguimiento |
| `[RESULTADOS_VERIFICADOS]` | Resultados y evidencias efectivamente comprobados |
| `[IDIOMA]` | Idioma de la respuesta, por ejemplo español |
| `[FORMATO_SALIDA]` | Markdown, tabla, CSV, etc. |

**Convención común:** la IA debe distinguir `DATO FACILITADO`, `SUPUESTO PENDIENTE DE VALIDAR` y `DECISIÓN APROBADA` y no debe inventar firmas, autorizaciones, mediciones ni resultados.

## 2. Método de uso

1. Ejecuta el **Prompt 00** y comprueba que entiende el proyecto.
2. Sigue el orden de fases. Pega la última versión **revisada** de los documentos que el siguiente prompt necesite.
3. Tras cada respuesta, corrige, valida y guarda el documento con fecha, versión y responsable.
4. En cambios de chat, vuelve a facilitar la ficha y `[DOCUMENTOS_APROBADOS]`; no supongas que la IA conserva ese contexto.
5. El control, la ejecución, las pruebas y la aceptación corresponden siempre a las personas responsables, no al modelo.

---

# Fase 0 · Preparación

## Prompt 00 — Configurar el asistente de gestión del proyecto

**Finalidad:** establecer rol, contexto y reglas. **Salida:** ficha de contexto validable.

```text
Actúa como asistente de gestión de proyectos con experiencia en metodologías predictivas y ágiles. Ayúdame a gestionar el proyecto siguiente:

Nombre: [NOMBRE_PROYECTO]
Organización y contexto: [ORGANIZACION_CONTEXTO]
Descripción: [DESCRIPCION_PROYECTO]
Necesidad: [PROBLEMA_NECESIDAD]
Usuarios o beneficiarios: [DESTINATARIOS_USUARIOS]
Objetivo preliminar: [OBJETIVO_PRELIMINAR]
Inicio: [FECHA_INICIO]
Fecha objetivo: [FECHA_OBJETIVO]
Cierre previsto: [FECHA_CIERRE]
Presupuesto: [PRESUPUESTO_MAXIMO]
Recursos: [RECURSOS_DISPONIBLES]
Roles: [ROLES_Y_RESPONSABLES]
Entregables preliminares: [ENTREGABLES_PRELIMINARES]
Restricciones: [RESTRICCIONES]
Exclusiones: [EXCLUSIONES]
Criterios de éxito: [CRITERIOS_EXITO]
Metodología: [METODOLOGIA]
Herramientas: [HERRAMIENTAS]

Reglas:
1. Trabaja fase por fase. No des por aprobado un documento sin confirmación humana.
2. Responde en [IDIOMA], usando [FORMATO_SALIDA].
3. Diferencia DATO FACILITADO, SUPUESTO PENDIENTE DE VALIDAR y DECISIÓN APROBADA.
4. No inventes presupuestos, fechas, evidencias, resultados, firmas o aprobaciones.
5. Pide solo los datos imprescindibles y señala los demás como pendientes.
6. Mantén trazabilidad entre objetivos, entregables, tareas, riesgos y decisiones.

Devuelve una tabla de contexto y una lista priorizada de datos pendientes. Todavía no generes los documentos de gestión.
```

**Revisión humana:** confirmar los datos y resolver ambigüedades críticas.

---

# Fase 1 · Inicio

## Prompt 01 — Elaborar el acta de constitución (plantilla 02)

**Salida:** acta de constitución en borrador.

```text
A partir del contexto validado del proyecto [NOMBRE_PROYECTO], redacta un acta de constitución.

Incluye: problema y justificación, objetivo SMART, beneficios previstos, alcance preliminar, exclusiones, entregables, hitos, presupuesto [PRESUPUESTO_MAXIMO], roles [ROLES_Y_RESPONSABLES], riesgos iniciales y tres criterios de éxito medibles.

Respeta [FECHA_INICIO], [FECHA_OBJETIVO], [RESTRICCIONES] y [ENTREGABLES_PRELIMINARES].

Entrega:
A) Acta en Markdown, con versión, fecha y estado Borrador.
B) Datos o autorizaciones pendientes.
C) Comprobaciones que debe hacer [ROL_APROBADOR].

Incluye un apartado de aprobación vacío. No generes firmas ficticias ni presentes la propuesta como autorizada.
```

## Prompt 02 — Revisar y validar el inicio (puerta de control)

**Salida:** informe de revisión de acta.

```text
Revisa críticamente el siguiente borrador de acta de constitución del proyecto [NOMBRE_PROYECTO]:

[ACTA_CONSTITUCION_BORRADOR]

Comprueba que el objetivo sea específico, medible, alcanzable según los recursos conocidos, relevante y temporal; que alcance, entregables, presupuesto, fechas y responsables no sean contradictorios; y que los criterios de éxito se puedan verificar.

Devuelve una tabla con: hallazgo, gravedad (alta/media/baja), evidencia textual, corrección propuesta y responsable de validación.

Separa: inconsistencias comprobables, supuestos pendientes y preguntas esenciales. No cambies silenciosamente ninguna decisión ni afirmes que el acta está aprobada.
```

---

# Fase 2 · Planificación

## Prompt 03 — Definir alcance y entregables (plantilla 05)

**Salida:** declaración de alcance.

```text
Actúa como responsable de planificación. A partir del acta aprobada:

[ACTA_CONSTITUCION_APROBADA]

Elabora el documento de alcance del proyecto [NOMBRE_PROYECTO]. Especifica qué incluye, qué excluye, requisitos, supuestos, restricciones y criterios de aceptación.

Crea una tabla: ID del entregable | descripción | responsable propuesto | dependencia | criterio de aceptación verificable.

Distingue claramente alcance del producto y trabajo del proyecto. Identifica solicitudes que podrían producir ampliaciones no autorizadas del alcance.

Entrega el documento en [FORMATO_SALIDA] y añade una lista de puntos que requieren conformidad de [ROL_APROBADOR].
```

## Prompt 04 — Desglosar tareas y crear cronograma (plantilla 07)

**Salida:** tareas, dependencias, hitos y calendario propuesto.

```text
A partir de los documentos aprobados:

Acta: [ACTA_CONSTITUCION_APROBADA]
Alcance: [DOCUMENTO_ALCANCE_APROBADO]
Recursos y dedicación: [RECURSOS_DISPONIBLES]
Fechas y restricciones: [FECHA_INICIO], [FECHA_OBJETIVO], [RESTRICCIONES]

Divide los entregables en tareas concretas, con IDs, responsables, duración estimada, fecha de inicio, fecha de fin, dependencias y criterio de finalización.

Presenta un cronograma en tabla Markdown y señala hitos, secuencia de dependencias, posibles cuellos de botella y tareas paralelizables.

Si no conoces capacidades o dedicaciones, no afirmes que el plazo sea viable: indica la estimación como supuesto y pide validación. Detecta conflictos de calendario y muestra alternativas razonables sin alterar objetivos aprobados.
```

## Prompt 05 — Elaborar la matriz de riesgos (plantilla 10)

**Salida:** registro de riesgos priorizados.

```text
Actúa como analista de riesgos para [NOMBRE_PROYECTO]. Usa el acta, el alcance y el cronograma validados:

[DOCUMENTOS_APROBADOS]

Identifica riesgos específicos técnicos, organizativos, de costes, plazos, calidad, seguridad, cumplimiento y aceptación cuando correspondan al proyecto.

Utiliza probabilidad e impacto en escala 1–5, nivel P×I, y clasifica en alta (15–25), media (6–14), baja (1–5), salvo que [ESCALA_RIESGOS] indique otra cosa.

Tabla: ID | riesgo | causa | probabilidad | impacto | nivel | prevención | contingencia | indicador de alerta | responsable.

Distingue riesgos posibles de incidencias que ya han ocurrido. No atribuyas probabilidades reales a datos no observados: presenta puntuaciones como valoración inicial a validar por el equipo.
```

## Prompt 06 — Auditar la coherencia del plan

**Salida:** lista de inconsistencias y propuesta de corrección.

```text
Realiza una auditoría cruzada del plan del proyecto [NOMBRE_PROYECTO]:

Acta: [ACTA_CONSTITUCION_APROBADA]
Alcance: [DOCUMENTO_ALCANCE_APROBADO]
Cronograma: [CRONOGRAMA_PROPUESTO]
Riesgos: [MATRIZ_RIESGOS]

Comprueba trazabilidad entre objetivos, entregables, tareas, responsables, fechas, presupuesto y criterios de aceptación.

Detecta tareas sin entregable, entregables sin tareas, dependencias imposibles, riesgos sin responsable, hitos incompatibles y decisiones no aprobadas.

Entrega una tabla: documento | inconsistencia | gravedad | corrección sugerida | quién debe aprobarla. Añade una lista de condiciones para autorizar el paso a ejecución. No modifiques los documentos directamente.
```

---

# Fase 3 · Ejecución y organización ágil

## Prompt 07 — Crear un tablero Kanban (plantilla 13)

**Salida:** tablero inicial y reglas de flujo.

```text
Transforma el plan de trabajo del proyecto [NOMBRE_PROYECTO] en un tablero Kanban.

Cronograma aprobado: [CRONOGRAMA_APROBADO]
Equipo: [ROLES_Y_RESPONSABLES]
Herramienta prevista: [HERRAMIENTA_KANBAN]
Límite de trabajo simultáneo: [LIMITE_WIP]

Usa inicialmente las columnas Pendiente, En curso, Revisión y Hecho, salvo que [COLUMNAS_KANBAN] indique otras.

Crea tarjetas con ID, nombre de tarea, entregable asociado, responsable, prioridad, dependencia, criterio de terminado, fecha objetivo y estado inicial.

Define reglas para mover tarjetas, gestionar bloqueos, revisar prioridades y respetar el límite WIP. Ofrece una tabla Markdown que pueda importarse o adaptarse a la herramienta, sin afirmar haber creado un tablero real.
```

## Prompt 08 — Analizar una incidencia y proponer acciones

**Salida:** plan de respuesta y actualización propuesta del Kanban.

```text
Durante la ejecución del proyecto [NOMBRE_PROYECTO] se ha producido la siguiente incidencia:

[INCIDENCIA_REAL_O_SIMULADA]
Fecha: [FECHA_INCIDENCIA]
Evidencias disponibles: [EVIDENCIAS_INCIDENCIA]
Impacto observado: [IMPACTO_OBSERVADO]
Tablero actual: [ESTADO_KANBAN]
Riesgos actuales: [MATRIZ_RIESGOS_ACTUAL]

Analiza causas posibles, impacto en alcance, calidad, fechas, costes y usuarios. Distingue hechos verificados de hipótesis.

Propón medidas de contención, investigación, corrección y comprobación. Incluye responsable, prioridad, fecha propuesta y criterios para considerar resuelta la incidencia.

Indica qué tarjetas mover, cuáles bloquear y qué decisiones necesitan autorización. No afirmes que la incidencia está resuelta ni que las acciones se han ejecutado.
```

---

# Fase 4 · Seguimiento

## Prompt 09 — Generar el informe de estado (plantilla 16)

**Salida:** informe de seguimiento con semáforo.

```text
Elabora un informe de estado del proyecto [NOMBRE_PROYECTO] a fecha [FECHA_INFORME].

Plan aprobado: [DOCUMENTOS_APROBADOS]
Avances verificados: [AVANCES_VERIFICADOS]
Estado de tareas: [ESTADO_KANBAN]
Hitos previstos y reales: [HITOS_PREVISTOS_Y_REALES]
Gasto previsto y real: [DATOS_PRESUPUESTO]
Incidencias y riesgos: [INCIDENCIAS_Y_RIESGOS]

Incluye resumen ejecutivo, semáforo verde/ámbar/rojo con justificación, entregables completados, desviaciones, bloqueos, próximos pasos y decisiones pendientes.

Usa una tabla Previsto | Real | Desviación únicamente para indicadores con datos disponibles. Marca los valores desconocidos como «sin dato». No inventes porcentajes ni avances.
```

---

# Fase 5 · Control y adaptación

## Prompt 10 — Evaluar alternativas y solicitudes de cambio

**Salida:** análisis de impacto y opciones de decisión.

```text
Analiza la siguiente solicitud de cambio o desviación del proyecto [NOMBRE_PROYECTO]:

[CAMBIO_PROPUESTO_O_DESVIACION]
Motivo: [MOTIVO_CAMBIO]
Situación actual: [INFORME_ESTADO]
Línea base aprobada: [DOCUMENTOS_APROBADOS]
Restricciones: [RESTRICCIONES]

Propón al menos tres opciones cuando existan: mantener el plan, ajustar tareas/recursos y modificar alcance o fecha sujeto a aprobación.

Para cada opción compara impacto en alcance, plazo, presupuesto, calidad, riesgos y carga de trabajo. Señala ventajas, inconvenientes, datos necesarios y quién debe decidir.

Recomienda una opción condicionada a los datos disponibles, pero no des por aprobado el cambio ni alteres la línea base.
```

## Prompt 11 — Verificar la coherencia tras los cambios

**Salida:** matriz de actualizaciones y pendientes.

```text
Comprueba cómo afecta la siguiente decisión humana al proyecto [NOMBRE_PROYECTO]:

Decisión y aprobación: [DECISION_APROBADA]
Versión anterior del plan: [DOCUMENTOS_APROBADOS]
Nuevo estado o plan: [PLAN_ACTUALIZADO]

Revisa la consistencia de objetivos, entregables, cronograma, tareas Kanban, matriz de riesgos, presupuesto e informe de estado.

Devuelve: documentos que deben versionarse, cambios exactos recomendados, dependencias alteradas, responsables, puntos aún sin resolver y comprobaciones necesarias.

Separa lo aprobado de lo propuesto. No supongas que una herramienta externa se ha actualizado.
```

---

# Fase 6 · Cierre y aprendizaje

## Prompt 12 — Preparar checklist de cierre y aceptación (plantilla 22)

**Salida:** checklist verificable, aún sin dar el proyecto por cerrado.

```text
Prepara la lista de aceptación y cierre del proyecto [NOMBRE_PROYECTO].

Alcance y entregables aprobados: [DOCUMENTO_ALCANCE_APROBADO]
Criterios de aceptación: [CRITERIOS_ACEPTACION]
Evidencias disponibles: [EVIDENCIAS_VERIFICADAS]
Incidencias pendientes: [INCIDENCIAS_PENDIENTES]
Rol aprobador: [ROL_APROBADOR]

Genera tabla: entregable | criterio de aceptación | prueba o evidencia requerida | estado (cumple/no cumple/pendiente) | responsable | observaciones.

Añade comprobaciones de documentación, seguridad y transferencia a operación cuando resulten aplicables. No marques «cumple» sin evidencia y deja vacía la firma de aceptación.
```

## Prompt 13 — Elaborar cierre de ejemplo con resultados simulados

**Salida:** cierre ficticio útil para enseñanza o ensayo; omitir en proyectos reales.

```text
Estamos realizando exclusivamente una SIMULACIÓN DIDÁCTICA del cierre del proyecto [NOMBRE_PROYECTO].

Resultados simulados proporcionados por la persona docente: [RESULTADOS_SIMULADOS]
Entregables: [DOCUMENTO_ALCANCE_APROBADO]
Checklist preparado: [CHECKLIST_CIERRE]

Elabora un ejemplo cumplimentado de checklist e informe de aceptación. Etiqueta de manera visible cada dato y evidencia como «SIMULADO».

Distingue requisitos técnicos, resultados de negocio, incidencias pendientes y acciones posteriores. Nunca generes firmas aparentemente auténticas ni confundas este ejercicio con una verificación real.
```

## Prompt 14 — Redactar lecciones aprendidas (plantilla 24)

**Salida:** borrador de retrospectiva para contrastar con el equipo.

```text
Ayúdame a preparar las lecciones aprendidas del proyecto [NOMBRE_PROYECTO].

Objetivos: [OBJETIVOS_APROBADOS]
Resultados comprobados: [RESULTADOS_VERIFICADOS]
Incidencias y decisiones: [INCIDENCIAS_Y_DECISIONES]
Opiniones del equipo: [APORTACIONES_EQUIPO]
Metodología y herramientas usadas: [METODOLOGIA] / [HERRAMIENTAS]

Separa lo que funcionó, lo que no funcionó, causas posibles, decisiones acertadas, oportunidades de mejora y acciones concretas para futuros proyectos.

Crea una tabla: situación | evidencia | aprendizaje | acción de mejora | responsable propuesto | comprobación futura.

No atribuyas opiniones a personas que no las hayan expresado. Finaliza con cinco preguntas para contrastar el borrador en una retrospectiva real.
```

---

# Fase 7 · Documentación y archivo

## Prompt 15 — Preparar el expediente final del proyecto

**Salida:** índice del expediente, resumen y control de integridad.

```text
Prepara el expediente documental final del proyecto [NOMBRE_PROYECTO] usando solamente las versiones verificadas de estos documentos:

[DOCUMENTOS_APROBADOS]

Genera:
1. Índice con nombre del documento, código, versión, fecha, responsable, estado y ruta o enlace disponible.
2. Resumen ejecutivo de máximo [LONGITUD_RESUMEN] palabras.
3. Matriz de trazabilidad: objetivo | entregable | tarea o hito | evidencia de aceptación | resultado.
4. Lista de documentos ausentes, discrepancias, incidencias pendientes y autorizaciones que falten.
5. Registro del uso de IA: tareas asistidas, revisión humana y limitaciones conocidas.

No inventes enlaces, archivos existentes, firmas, cifras ni evidencias. Presenta el estado «pendiente» cuando falte alguna validación y no anuncies el expediente como cerrado sin autorización.
```

---

## 3. Índice rápido de prompts

| Fase | IDs | Producto de trabajo |
|---|---|---|
| Preparación | 00 | Contexto de proyecto |
| Inicio | 01–02 | Acta de constitución y validación |
| Planificación | 03–06 | Alcance, cronograma, riesgos y auditoría |
| Ejecución | 07–08 | Kanban y plan de respuesta |
| Seguimiento | 09 | Informe de estado |
| Control | 10–11 | Evaluación de cambios y consistencia |
| Cierre | 12–14 | Aceptación, simulación opcional y lecciones |
| Documentación | 15 | Expediente final |

## 4. Criterios de calidad antes de utilizar las respuestas

- [ ] ¿Los datos utilizados proceden de información facilitada o validada?
- [ ] ¿Se distinguen supuestos, propuestas, decisiones y hechos?
- [ ] ¿Cada entregable tiene responsable y criterio de aceptación?
- [ ] ¿Las fechas, costes y dependencias son coherentes?
- [ ] ¿Se identifica quién aprueba los cambios y el cierre?
- [ ] ¿No se incluyen datos sensibles ni se inventan evidencias?
- [ ] ¿La versión aprobada se conserva antes del siguiente prompt?

## 5. Convención de nombres sugerida para el repositorio

Archivo único: `biblioteca-prompts-gestion-proyectos-ia.md`. Si la biblioteca crece, dividir por fases en `prompts/gestion-proyectos/00-preparacion.md`, `01-inicio.md`, etc., manteniendo esta ficha de variables como referencia central.
