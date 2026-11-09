# Tablero Kanban

> SIMULACIÓN DIDÁCTICA. Datos y decisiones ficticios; no acredita implantación ni aprobación real.

**Proyecto:** AULA-INC · **Código:** AINC-13  
**Versión:** 1.1 · **Fecha:** 2026-11-20  
**Responsable:** Coordinación · **Estado:** Finalizado solo en la simulación

## Política de flujo

Pendiente → En curso → Revisión → Hecho. WIP máximo 2 en En curso y 2 en Revisión. Bloqueo es una marca, no una quinta columna; la tarjeta bloqueada cuenta en su columna. No iniciar una dependencia hasta que la anterior esté Hecha. Revisión usa los criterios y puede devolver la tarjeta a En curso.

## Tarjetas

| ID | Tarea | Responsable | Prioridad | Columna al cierre SIMULADO | Bloqueos | Entregable | Dependencia | Fecha objetivo | Criterio terminado |
|---|---|---|---|---|---|---|---|---|---|
| T01 | Definir y validar inicio | Coordinación | Media | Hecho | Ninguno | E04 | — | 09/11/2026 | Acta revisada y D-01 |
| T02 | Validar alcance, calendario y riesgos | Coordinación | Media | Hecho | Ninguno | E04 | T01 | 10/11/2026 | 05,07,10 revisados y D-02 |
| T03 | Diseñar campos, estados y prioridad | Técnico | Media | Hecho | Ninguno | E01 | T02 | 11/11/2026 | Diccionario y listas definidos |
| T04 | Configurar registro y vistas | Técnico | Alta | Hecho | Ninguno | E01 | T03 | 13/11/2026 | Registro disponible para ensayo |
| T05 | Redactar procedimiento | Coordinación | Media | Hecho | Ninguno | E02 | T03 | 13/11/2026 | Roles y transiciones revisados |
| T06 | Ensayar seis pruebas | Usuario representante | Alta | Hecho | Ninguno | E03 | T04,T05 | 16/11/2026 | Resultados P01–P06 registrados |
| T07 | Corregir y volver a probar | Técnico | Alta | Hecho | Ninguno | E03 | T06 | 17/11/2026 | IP-01 resuelta en simulación y P02 repetida |
| T08 | Ejecutar piloto con diez avisos | Usuario representante | Media | Hecho | Ninguno | E03 | T07 | 18/11/2026 | Lista de diez cotejada con registro |
| T09 | Formar, transferir y cerrar | Coordinación | Media | Hecho | Ninguno | E04 | T08 | 20/11/2026 | Formación, pendientes, 22 y24 archivados |

## Criterios para mover tarjetas

En curso: responsable disponible y dependencias hechas. Revisión: producto de trabajo y evidencia adjuntos. Hecho: revisión humana superada. T04 queda Hecha cuando permite el ensayo inicial; la aceptación final de E01 depende también de T06 y T07. Un ensayo puede estar Hecho con un fallo documentado; eso no equivale a producto aceptado.

## Revisión del tablero

Reunión diaria de cinco minutos. Priorizar correcciones que bloquean el piloto, registrar decisiones y respetar WIP. Las columnas operativas de los tickets INC son distintas de este tablero de proyecto. Ver `../05_escenas/estados_tablero.csv` para tres cortes de la simulación.


## Historial de revisiones

| Versión | Fecha | Modificación | Autor/rol |
|---|---|---|---|
| 0.1 | 2026-11-09 | Borrador inicial previsto en el ejercicio | Equipo |
| 1.0 | 2026-11-10 | Versión de referencia de esta escena | Coordinación |
| 1.1 | 2026-11-20 | Actualización según escenas; versión anterior conservada | Coordinación |

Actualización: D-03 en la simulación; conservar línea base y cortes previos. Las tarjetas siguen los estados de cada escena, no el estado final de este archivo.
