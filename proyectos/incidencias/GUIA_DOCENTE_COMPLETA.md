# AULA-INC · Implantar un sistema de gestión de incidencias

Kit de simulación didáctica · Versión 1.0 · Preparado el 08/11/2026.

**Todo el caso, las personas, las decisiones, las horas y los resultados son SIMULADOS.** No se ha configurado ninguna herramienta externa ni se ha implantado un sistema real.

## Qué se aprende

Seguir un proyecto pequeño desde la necesidad hasta la transferencia a operación; utilizar los prompts 00–15; completar las plantillas 02, 05, 07, 10, 13, 16, 22 y 24; revisar respuestas de IA; tomar decisiones y conservar versiones.

El proyecto es **implantar** el sistema. Registrar y resolver las incidencias después es la **operación**. Las tareas T01–T09 del proyecto no son los tickets INC-001–INC-010 del servicio. El fallo IP-01 sucede durante la implantación y se gestiona como incidencia del proyecto.

## Por dónde empezar

1. Docente: leer [guion de clase](01_docente/guion_clase.md) y [sistema de trabajo](01_docente/sistema_documentacion.md).
2. Distribuir solo `02_alumnado/` y las plantillas vacías de `00_referencias/`. Mantener `03_solucion/` y las escenas futuras fuera de la carpeta compartida.
3. Facilitar `04_prompts/00_contexto.md` y revelar los archivos de `05_escenas/` cuando lo indique el guion.
4. Ejecutar los prompts en orden usando `04_prompts/guion_prompts.md` y la biblioteca original en `00_referencias/`.
5. Comparar cada resultado con su solución y guardar la decisión humana antes de continuar.
6. Revisar [expediente y trazabilidad](03_solucion/expediente.md).

## Carpetas

| Carpeta | Uso |
|---|---|
| 00_referencias | Copias de la guía y de las ocho plantillas consultadas |
| 01_docente | Organización de clase, herramientas y evaluación |
| 02_alumnado | Enunciado y registro de trabajo rellenable |
| 03_solucion | Ocho plantillas resueltas, revisiones y expediente |
| 04_prompts | Contexto común y fichas de ejecución 00–15 |
| 05_escenas | Sobres de información que se revelan progresivamente |
| 06_producto | Especificación del sistema, procedimiento, pruebas y datos ficticios |

Markdown es la fuente de verdad; CSV sirve para copiar tablas a una hoja o adaptar tarjetas a un tablero. Los CSV no implican una importación automática específica.

## Fuentes y adaptación

Consultadas el 08/11/2026:

- [Guía de prompts de IA](https://github.com/albertomozo/TDIGITAL/blob/main/PROMPTS/ejemplos/prompts_gestion_proyectos_ia.md).
- [Índice de plantillas](https://github.com/albertomozo/metologias-agiles-con-ia-25/blob/main/plantillas_gestion_proyectos/README.md).

La solución conserva los apartados principales de las ocho plantillas y añade evidencias, trazabilidad y control de versiones. Se usa Kanban, sin imponer roles o ceremonias de Scrum. El calendario y la duración de clase son una propuesta didáctica, independiente del calendario ficticio del proyecto.


---

# Sistema aconsejado para documentar y simular

Recomendación: **Markdown en VS Code + repositorio GitHub + un tablero Kanban**. Usa la IA para preparar y revisar borradores; la decisión y la versión de referencia corresponden al equipo.

Para este grupo inicial, el docente puede gestionar GitHub y el alumnado editar copias Markdown en carpetas. No es necesario enseñar Git para aprender gestión de proyectos.

## Una función por herramienta

| Necesidad | Sistema propuesto | Regla |
|---|---|---|
| Documentación de gestión | Markdown | Un archivo vigente por documento |
| Versiones y consulta | GitHub | Conservar hitos; evitar sobreescribir el plan original |
| Trabajo del proyecto | Un tablero físico o digital | T01–T09; no duplicarlo en varias aplicaciones |
| Sistema de incidencias que se implanta | Hoja de cálculo compartida en el ejercicio | INC-001…; no mezclar con las tareas de implantación |
| Distribución a clase | Carpeta compartida o aula virtual | Solo materiales ya revelados |
| DOCX/PDF/diapositivas | Exportación posterior | No mantener una segunda fuente manual |

La recomendación responde al material ya disponible en tus repositorios y a tu preferencia por Markdown. No depende de una función concreta de pago o de una importación automática. El tablero puede ser Trello, GitHub Projects o una pizarra; comprobar disponibilidad en el entorno de clase antes de elegir.

## Flujo documental por paso

1. Abrir el contexto, el prompt original y la plantilla de destino.
2. Proporcionar a la IA los textos completos de las versiones necesarias; un enlace no garantiza su lectura.
3. Guardar la respuesta como `borradores/02-acta_v0.1.md`.
4. Revisar datos, alcance, tareas, fechas, cálculos y supuestos.
5. Registrar en la bitácora qué se acepta, corrige o deja pendiente.
6. Guardar la versión de referencia en `vigente/02-acta.md`; conservar la anterior en `historico/` o en Git.
7. Adjuntar esa versión revisada al siguiente prompt. Una respuesta de IA no actualiza el tablero ni los documentos externos.

## Estructura de trabajo de cada equipo

Crear una copia nueva para cada edición del ejercicio: `equipo-01/`, con carpetas `contexto/`, `borradores/`, `vigente/`, `historico/`, `evidencias/` y `bitacora/`. No editar las soluciones maestras.

En `vigente/` mantener exactamente ocho documentos: 02, 05, 07, 10, 13, 16, 22 y 24. Las revisiones de IA y decisiones pueden ir en una única bitácora para no aumentar burocracia. Los archivos adicionales de este kit son apoyo didáctico o producto del proyecto, no nuevas plantillas obligatorias.

## Metadatos mínimos

Código, versión, fecha, responsable, estado y referencia a la decisión. Estados recomendados: Borrador, Revisado, Aprobado para simulación y Sustituido. La aprobación real sigue pendiente; no producir firmas ficticias.

## Puntos de guardado

| Punto | Documentos que se conservan | Nombre sugerido del hito |
|---|---|---|
| Inicio validado | 02 | H1-inicio |
| Plan validado | 02,05,07,10 | H2-plan |
| Ejecución inicial | 13 y plan | H3-ejecucion |
| Desviación detectada | 16 y captura/tablas del tablero | H4-desviacion |
| Decisión de cambio | Bitácora y documentos afectados | H5-decision |
| Cierre simulado | Los ocho documentos y evidencias | H6-cierre |

Si usas Git, un commit por hito permite mostrar el antes y el después. Si no, copia esos documentos en una carpeta de hito con fecha. No mezcles las dos técnicas sin necesidad.

## Reiniciar la simulación

Crear otra copia de las plantillas vacías, borrar los datos de la hoja del equipo y repartir solo la escena inicial. Conservar la solución docente. Reiniciar también las tarjetas a Pendiente. Cada nuevo chat recibe el contexto y las versiones revisadas; no confiar en memoria implícita.


---

# Guion docente: mostrar cómo se construye la solución

Propuesta: dos sesiones de cinco horas de presencia, cada una con 30 minutos de descanso y 270 minutos de actividad. Se comprimen diez días ficticios en dos sesiones. No es la duración real estimada de implantación. Para una demostración corta, el docente ejecuta los prompts y el grupo revisa; para taller, cada equipo guarda sus documentos.

## Antes de empezar

Preparar una copia por equipo y una hoja vacía con el esquema del producto. No repartir la solución. Proyectar solo el paso activo. Explicar roles y distinguir T, INC e IP. Las escenas están predeterminadas para la demostración; si el alumnado decide otra opción, deberá documentar otra solución coherente.

## Sesión 1: del problema al tablero

| Minutos de actividad | Acción | Prompts | Salida y revisión |
|---|---|---|---|
| 0–25 | Presentar reto, roles y contexto | 00 | Preguntas pendientes; confirmar horas y límites |
| 25–65 | Redactar y revisar acta | 01–02 | 02-acta; no inventar reducción de tiempos |
| 65–110 | Revelar escena 01 y definir alcance | 03 | 05-alcance; criterios medibles para E01–E04 |
| 110–155 | Construir calendario y calcular capacidad | 04 | 07-cronograma; 31 h base y 9 h reserva |
| 155–185 | Identificar riesgos | 05 | 10-riesgos; no llamar riesgo a un hecho ocurrido |
| 185–220 | Auditar plan y emitir D-02 simulada | 06 | Correcciones y punto de guardado H2 |
| 220–255 | Crear tablero de proyecto | 07 | 13-kanban; dependencias y WIP |
| 255–270 | Comparar criterios y explicar siguiente escena | — | Bitácora y archivos revisados |

Insertar descanso tras unos 135 minutos de actividad. La tabla contabiliza actividad, no hora de reloj.

## Sesión 2: probar, adaptar y cerrar

| Minutos de actividad | Acción | Prompts | Salida y revisión |
|---|---|---|---|
| 0–30 | Configurar hoja y ensayar registro/estados | — | Producto mínimo y contraste con procedimiento |
| 30–65 | Revelar escena 02: IP-01 | 08 | Contención, hipótesis y repetición; no declarar resuelto |
| 65–95 | Informe al 16/11 | 09 | 16-informe; corte temporal sin datos futuros |
| 95–140 | Revelar escena 03: C-01; comparar opciones | 10 | Decisión D-03: aplazar correo automático |
| 140–170 | Revelar repetición de prueba y actualizar | 11 | 07 y10 v1.1; tablero, previsión y bitácora |
| 170–210 | Revelar escena 04; verificar evidencias y cerrar | 12–13 | 22-checklist: antes pendiente, después cumple SIMULADO |
| 210–240 | Retrospectiva | 14 | 24-lecciones y acciones |
| 240–270 | Expediente, trazabilidad y explicación del equipo | 15 | Integridad de ocho documentos y registro de IA |

Insertar descanso cerca de mitad de sesión. Si la configuración real tarda más, usar los CSV como material de mesa y conservar el foco en gestión.

## Rutina repetida en cada paso

Mostrar entrada → ejecutar prompt → examinar borrador → detectar un supuesto/error → decidir → guardar versión → enseñar qué entrada necesita el siguiente paso. No mostrar todo el solucionario al inicio.

## Tres momentos que conviene representar

1. Acta v0.1 dice «mejorar mucho la atención». El grupo lo sustituye por C1–C3 verificables. La aprobación del ejercicio la da Dirección, no la IA.
2. P02 falla. El ensayo T06 puede terminar y el producto seguir sin aceptación. La tarjeta T08 permanece bloqueada.
3. Se pide correo automático. El grupo compara opciones y protege la línea base. La alternativa predeterminada lo aplaza; no se borra de la bitácora.

## Rúbrica, 10 puntos

| Criterio | Puntos | Evidencia |
|---|---:|---|
| Contexto, objetivo y límites coherentes | 2 | 02 y05 |
| Plan viable según hipótesis y capacidad | 2 | 07,10 y cálculo de horas |
| Seguimiento, bloqueo y cambio justificados | 2 | 13,16 y bitácora |
| Cierre trazable y transferencia | 2 | 22 y evidencias |
| Revisión crítica de IA y aprendizaje | 2 | Bitácora y24 |

En cada criterio: 0 ausente/incoherente; 1 parcial con lagunas; 2 completo y justificado. La calidad de la revisión cuenta más que imitar literalmente la solución.


---

# Ficha de contexto · Datos facilitados para la simulación

Todos los datos siguientes son ficticios, fijados por el caso docente. El contexto no equivale a una aprobación real.

| Variable | Valor |
|---|---|
| NOMBRE_PROYECTO | AULA-INC: implantación de un sistema de incidencias |
| DESCRIPCION_PROYECTO | Diseñar, configurar y probar un registro central con un procedimiento de atención |
| PROBLEMA_NECESIDAD | Los avisos de equipos y aplicaciones llegan por canales dispersos; no hay seguimiento uniforme. No hay medición inicial de pérdidas o tiempos |
| ORGANIZACION_CONTEXTO | Centro formativo ficticio Aula Norte, dos aulas, 20 equipos |
| DESTINATARIOS_USUARIOS | Docentes y personal de administración; coordinación registra los avisos en el piloto |
| OBJETIVO_PRELIMINAR | Tener un canal y registro único operativo el 19/11/2026 |
| FECHA_INICIO | 09/11/2026 |
| FECHA_OBJETIVO | 19/11/2026: sistema preparado y usuarios informados |
| FECHA_CIERRE | 20/11/2026: aceptación y archivo |
| PRESUPUESTO_MAXIMO | 40 horas internas a coste convencional de 20 €/h = 800 €; sin compras ni licencias nuevas |
| RECURSOS_DISPONIBLES | Coordinación 12 h; técnico 20 h; usuario representante 8 h. Dirección autoriza dentro de las 12 h de coordinación |
| ROLES_Y_RESPONSABLES | Dirección: patrocinador/aprobador; coordinación: dirige y atiende el registro; técnico: configura y corrige; usuario representante: prueba y valida comprensión. En clase el docente representa Dirección |
| ENTREGABLES_PRELIMINARES | E01 registro y vistas; E02 procedimiento; E03 pruebas y ajustes; E04 formación, transferencia y expediente |
| RESTRICCIONES | Solo datos ficticios, horario laboral lunes a viernes, sin compras; usar una hoja compartida ya disponible y copias locales; sin programación obligatoria |
| EXCLUSIONES | App propia, correo automático, WhatsApp, IA que resuelva averías, migración histórica y servicio 24/7 |
| CRITERIOS_EXITO | Registrar 10/10 avisos del piloto; 10/10 tickets con responsable y prioridad; 6/6 pruebas de aceptación superadas al cierre |
| METODOLOGIA | Planificación mínima e iteraciones con Kanban; revisión diaria de 5 minutos |
| HERRAMIENTAS | Markdown, hoja de cálculo, tablero Kanban físico o digital, IA para borradores y revisión |
| DOCUMENTOS_APROBADOS | Ninguno al empezar; las decisiones de cada escena habilitan el siguiente paso solo en la simulación |
| IDIOMA | Español |
| FORMATO_SALIDA | Markdown; CSV complementario |

Variables adicionales: ROL_APROBADOR = Dirección; HERRAMIENTA_KANBAN = tablero elegido por la clase; LIMITE_WIP = 2 En curso y 2 Revisión; LONGITUD_RESUMEN = 150 palabras. No hay una línea base de tiempos de atención; no inventar mejoras porcentuales.

## Reglas para cualquier prompt del ejercicio

SIMULACIÓN DIDÁCTICA. Usa solo contexto y escenas ya reveladas. Distingue dato facilitado, supuesto y decisión simulada. No anticipes resultados de futuras escenas. Mantén los IDs E01–E04, T01–T09, R01–R04, IP-01 y C-01. No generes firmas ni afirmes que una acción se ha ejecutado fuera del caso. Las evidencias de cierre se etiquetan SIMULADO.


---

# Prompts paso a paso

No se afirma que estos prompts se hayan ejecutado en una herramienta externa. La solución docente es una respuesta de referencia redactada para este caso. Cada ejecución en clase puede producir otra redacción.

Usar el texto original completo de cada prompt en `00_referencias/prompts_gestion_proyectos_ia.md`. Las fichas siguientes explican qué aportar y qué guardar. Adjuntar archivos o pegar contenido, no dejar solo las rutas. No alimentar toda la solución al principio: revelaría el desenlace.

## Mensaje de trabajo que puedes usar en cada paso

```text
Estamos en una SIMULACIÓN DIDÁCTICA de AULA-INC. Trabaja únicamente el prompt que indico, con la plantilla y documentos que adjunto. Usa solo los datos de las escenas ya reveladas. Conserva sus IDs y fechas; separa datos facilitados, supuestos y decisiones simuladas. No inventes aprobaciones, evidencias ni acciones externas. Devuelve el documento en Markdown, una lista de pendientes y qué debe revisar el equipo antes de avanzar.
```

## Paso 00 · Preparar contexto

**Prompt original:** 00. **Entradas:** 04_prompts/00_contexto.md.  
**Guardar:** Ficha de contexto; pendientes por confirmar.  
**Revisión/puerta:** Confirmar datos y distinguir simulación de hecho real.

```text
Ejecuta ahora el Prompt 00 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: 04_prompts/00_contexto.md.
No continúes a otro paso. Antes de finalizar, comprueba: Confirmar datos y distinguir simulación de hecho real.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 01 · Redactar acta

**Prompt original:** 01. **Entradas:** Contexto validado; plantilla02.  
**Guardar:** 02-acta v0.1.  
**Revisión/puerta:** No aprobar automáticamente.

```text
Ejecuta ahora el Prompt 01 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Contexto validado; plantilla02.
No continúes a otro paso. Antes de finalizar, comprueba: No aprobar automáticamente.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 02 · Revisar acta

**Prompt original:** 02. **Entradas:** Borrador02.  
**Guardar:** Tabla de hallazgos; 02 corregida.  
**Revisión/puerta:** Dirección emite D-01 al revelar escena01.

```text
Ejecuta ahora el Prompt 02 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Borrador02.
No continúes a otro paso. Antes de finalizar, comprueba: Dirección emite D-01 al revelar escena01.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 03 · Definir alcance

**Prompt original:** 03. **Entradas:** 02 revisada y D-01; plantilla05.  
**Guardar:** 05-alcance.  
**Revisión/puerta:** E01–E04 medibles; exclusiones explícitas.

```text
Ejecuta ahora el Prompt 03 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: 02 revisada y D-01; plantilla05.
No continúes a otro paso. Antes de finalizar, comprueba: E01–E04 medibles; exclusiones explícitas.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 04 · Planificar tareas

**Prompt original:** 04. **Entradas:** 02 y05 revisadas; plantilla07; recursos del contexto.  
**Guardar:** 07-cronograma.  
**Revisión/puerta:** 31 h y nueve tareas; no ocupar toda la reserva.

```text
Ejecuta ahora el Prompt 04 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: 02 y05 revisadas; plantilla07; recursos del contexto.
No continúes a otro paso. Antes de finalizar, comprueba: 31 h y nueve tareas; no ocupar toda la reserva.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 05 · Valorar riesgos

**Prompt original:** 05. **Entradas:** 02,05,07 revisadas; plantilla10.  
**Guardar:** 10-riesgos.  
**Revisión/puerta:** P×I; cada riesgo tiene responsable y alerta.

```text
Ejecuta ahora el Prompt 05 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: 02,05,07 revisadas; plantilla10.
No continúes a otro paso. Antes de finalizar, comprueba: P×I; cada riesgo tiene responsable y alerta.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 06 · Auditar plan

**Prompt original:** 06. **Entradas:** 02,05,07,10 vigentes.  
**Guardar:** Informe de coherencia.  
**Revisión/puerta:** Comprobar dependencias y capacidad; después D-02.

```text
Ejecuta ahora el Prompt 06 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: 02,05,07,10 vigentes.
No continúes a otro paso. Antes de finalizar, comprueba: Comprobar dependencias y capacidad; después D-02.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 07 · Preparar Kanban

**Prompt original:** 07. **Entradas:** 07 y D-02; plantilla13.  
**Guardar:** 13-kanban inicial.  
**Revisión/puerta:** Tarjetas T01–T09; no mezclar INC.

```text
Ejecuta ahora el Prompt 07 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: 07 y D-02; plantilla13.
No continúes a otro paso. Antes de finalizar, comprueba: Tarjetas T01–T09; no mezclar INC.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 08 · Responder al fallo

**Prompt original:** 08. **Entradas:** Escena02; tablero al16 y riesgos iniciales.  
**Guardar:** Respuesta a IP-01.  
**Revisión/puerta:** Hipótesis no son causas confirmadas; T08 bloqueada.

```text
Ejecuta ahora el Prompt 08 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Escena02; tablero al16 y riesgos iniciales.
No continúes a otro paso. Antes de finalizar, comprueba: Hipótesis no son causas confirmadas; T08 bloqueada.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 09 · Informar estado

**Prompt original:** 09. **Entradas:** Escena02, plan y tablero al16; plantilla16.  
**Guardar:** 16-informe al16.  
**Revisión/puerta:** 20 h y5/6 pruebas; sin datos futuros.

```text
Ejecuta ahora el Prompt 09 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Escena02, plan y tablero al16; plantilla16.
No continúes a otro paso. Antes de finalizar, comprueba: 20 h y5/6 pruebas; sin datos futuros.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 10 · Comparar alternativas

**Prompt original:** 10. **Entradas:** Escena03 solo petición C-01; informe16 y línea base.  
**Guardar:** Análisis de C-01.  
**Revisión/puerta:** Comparar A/B/C antes de revelar D-03.

```text
Ejecuta ahora el Prompt 10 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Escena03 solo petición C-01; informe16 y línea base.
No continúes a otro paso. Antes de finalizar, comprueba: Comparar A/B/C antes de revelar D-03.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 11 · Revisar cambios

**Prompt original:** 11. **Entradas:** D-03 y repetición de P02 de escena03; versiones anteriores.  
**Guardar:** 07 y10 v1.1; nuevos estados; bitácora.  
**Revisión/puerta:** No borrar informe histórico al16.

```text
Ejecuta ahora el Prompt 11 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: D-03 y repetición de P02 de escena03; versiones anteriores.
No continúes a otro paso. Antes de finalizar, comprueba: No borrar informe histórico al16.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 12 · Preparar aceptación

**Prompt original:** 12. **Entradas:** 05 y criterios; plantilla22; solo evidencias ya conocidas.  
**Guardar:** 22 con pendientes.  
**Revisión/puerta:** No marcar cumple si todavía no se ha revelado evidencia.

```text
Ejecuta ahora el Prompt 12 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: 05 y criterios; plantilla22; solo evidencias ya conocidas.
No continúes a otro paso. Antes de finalizar, comprueba: No marcar cumple si todavía no se ha revelado evidencia.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 13 · Cerrar caso simulado

**Prompt original:** 13. **Entradas:** Escena04 completa,22 y datos del piloto.  
**Guardar:** 22 resuelto SIMULADO.  
**Revisión/puerta:** Firma real vacía; seis tickets quedan en operación.

```text
Ejecuta ahora el Prompt 13 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Escena04 completa,22 y datos del piloto.
No continúes a otro paso. Antes de finalizar, comprueba: Firma real vacía; seis tickets quedan en operación.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 14 · Aprender

**Prompt original:** 14. **Entradas:** Resultados de escena04; decisiones; plantilla24.  
**Guardar:** 24-lecciones.  
**Revisión/puerta:** No atribuir opiniones inventadas; contrastar con grupo.

```text
Ejecuta ahora el Prompt 14 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Resultados de escena04; decisiones; plantilla24.
No continúes a otro paso. Antes de finalizar, comprueba: No atribuir opiniones inventadas; contrastar con grupo.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.

## Paso 15 · Archivar

**Prompt original:** 15. **Entradas:** Ocho documentos revisados, históricos y evidencias.  
**Guardar:** Expediente y trazabilidad.  
**Revisión/puerta:** Revisar integridad y registrar ayuda de IA.

```text
Ejecuta ahora el Prompt 15 de la guía adjunta para AULA-INC, adaptando su salida a la plantilla de destino cuando corresponda.
Documentos que aporto en este mensaje: Ocho documentos revisados, históricos y evidencias.
No continúes a otro paso. Antes de finalizar, comprueba: Revisar integridad y registrar ayuda de IA.
```

La salida se compara con `03_solucion/` después de la revisión del equipo. Guardar el texto realmente utilizado y el resultado en la bitácora.
