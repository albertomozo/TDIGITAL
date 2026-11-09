# Producto E01 · Especificación para configurar una hoja

Este archivo es un diseño implementable; no se ha creado una hoja externa. En clase, crear una hoja, copiar encabezados, definir listas y ejecutar pruebas con datos ficticios. Una copia local permite trabajar sin cuentas.

## Diccionario de campos

| Campo | Tipo/regla | Ejemplo |
|---|---|---|
| id | Texto único; coordinación asigna secuencia y comprueba duplicados | INC-001 |
| fecha | Fecha de recepción ISO | 2026-11-18 |
| solicitante | Alias ficticio | Docente A |
| aula | Lista Aula 1, Aula 2, Administración | Aula 1 |
| categoria | Lista Hardware, Software, Conectividad, Acceso | Hardware |
| descripcion | Texto breve, sin contraseñas | Pantalla sin señal |
| impacto | Lista Alto, Medio, Bajo | Medio |
| urgencia | Lista Alta, Media, Baja | Media |
| prioridad | Alta, Media, Baja; obligatoria | Media |
| responsable | Técnico o Coordinación; obligatorio | Técnico |
| estado | Nueva, Asignada, En curso, Resuelta, Cerrada | Asignada |
| resolucion | Texto; requerido al pasar a Resuelta | Cable ajustado |
| validacion_usuario | Pendiente o Conforme; Conforme antes de Cerrada | Pendiente |

Preparar vistas/filtros: pendientes (estado distinto de Cerrada), por responsable y por prioridad. No confundir filtros con permisos.

## Reglas de prioridad

Alta si impacto Alto o urgencia Alta. Baja solo si impacto Bajo y urgencia Baja. Media en los demás casos. Son reglas acordadas del caso, no un estándar universal ni un SLA contractual.

## Pruebas de configuración

Usar validación de celdas para los valores permitidos y revisar vacíos/duplicados antes de aceptar. Verificar el comportamiento real de la hoja: una validación puede ser eludida al pegar datos, por lo que no se promete integridad automática. Si no se dispone de hoja compartida, simular la comprobación con tabla impresa; registrar esa limitación.
