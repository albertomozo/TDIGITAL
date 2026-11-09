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
