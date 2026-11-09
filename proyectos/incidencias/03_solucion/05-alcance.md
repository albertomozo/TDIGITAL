# Definición de alcance y entregables

> SIMULACIÓN DIDÁCTICA. Datos y decisiones ficticios; no acredita implantación ni aprobación real.

**Proyecto:** AULA-INC · **Código:** AINC-05  
**Versión:** 1.0 · **Fecha:** 2026-11-10  
**Responsable:** Coordinación · **Estado:** Aprobado para simulación

## Objetivo del producto

Permitir registrar un aviso, asignarlo y seguirlo hasta su validación y cierre. Producto: registro y procedimiento. Trabajo del proyecto: diseñar, configurar, probar, formar y entregar.

## Incluido

Una hoja con campos definidos, listas de valores, filtro de pendientes, reglas de prioridad y procedimiento. Diez tickets ficticios para un piloto. Seis pruebas de aceptación y sesión de transferencia.

## Excluido

Correo automático, WhatsApp, programación de una aplicación, migración histórica y mantenimiento 24/7. Las reparaciones reales de equipos no forman parte de la implantación.

## Entregables

| ID | Entregable | Responsable | Dependencia | Criterio de aceptación |
|---|---|---|---|---|
| E01 | Registro y vistas | Técnico | Diseño de campos T03 | Campos y estados definidos; diez IDs distintos; prioridad y responsable obligatorios; filtro de pendientes excluye Cerrada |
| E02 | Procedimiento de atención | Coordinación | Diseño T03 | Indica canal, roles, prioridad, transiciones, reapertura y revisión diaria; usuario lo interpreta en prueba P06 |
| E03 | Informe de pruebas y ajustes | Usuario representante | E01 y E02 en borrador | P01–P06 superadas; corrección IP-01 comprobada antes del piloto |
| E04 | Formación, transferencia y expediente | Coordinación | E03 | Usuario registra un caso; coordinación recibe hoja, procedimiento y pendientes; ocho documentos archivados y aceptación simulada registrada |

## Requisitos

RQT1: ID único. RQT2: prioridad y responsable en cada registro. RQT3: estados Nueva, Asignada, En curso, Resuelta y Cerrada. RQT4: cierre tras validación del usuario; si falla, vuelve a En curso. RQT5: datos exclusivamente ficticios y acceso de trabajo limitado al equipo. RQT6: copia de seguridad al final de cada jornada. La validación de celdas reduce errores; una hoja no se presenta como sistema con garantías de base de datos.

Supuestos: existe una hoja compartida utilizable sin compras, y el equipo tiene las horas asignadas. Deben comprobarse en una implantación real.

## Cambios de alcance

Propuesta escrita → análisis de impacto → Dirección decide → versionar documentos afectados → comunicar. C-01 pide correo automático: en D-03 se aplaza; no modifica esta línea base. La corrección IP-01 restaura un requisito ya incluido y se cubre con reserva.


## Historial de revisiones

| Versión | Fecha | Modificación | Autor/rol |
|---|---|---|---|
| 0.1 | 2026-11-09 | Borrador inicial previsto en el ejercicio | Equipo |
| 1.0 | 2026-11-10 | Versión de referencia de esta escena | Coordinación |
