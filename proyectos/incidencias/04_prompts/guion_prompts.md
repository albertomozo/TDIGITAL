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
