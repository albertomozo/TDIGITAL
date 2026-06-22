## 🏪 Caso: "CaféDigital" — Una cafetería que quiere tomar mejores decisiones

La idea es simple: una cafetería pequeña que **digitaliza su operación** recogiendo datos de tres fuentes distintas y los combina para tomar decisiones. Es un negocio que todos entienden, sin importar el sector.

---

### El problema que resuelven

> *"Vendemos todos los días pero no sabemos qué nos deja más dinero, cuándo hay más clientes, ni qué opinan realmente."*

---

### Las 3 fuentes de datos (una por módulo del curso)

**Módulo 1 — Formulario / Encuesta**
Los clientes escanean un QR al salir y responden 3 preguntas en Google Forms o Microsoft Forms: ¿Cómo calificarías tu visita? ¿Qué producto pediste? ¿Volverías?. Esto genera una hoja de respuestas automática. Los participantes aprenden que los datos pueden llegar solos, sin digitarlos manualmente.

**Módulo 2 — Archivo Excel / CSV**
El cajero registra cada venta en una hoja simple: fecha, hora, producto, cantidad, precio. Este archivo se exporta diariamente. Los participantes aprenden a estructurar bien una tabla (sin celdas combinadas, sin colores como datos, con encabezados claros) y a importar un CSV.

**Módulo 3 — Sistema ERP / Base de datos**
El proveedor de ingredientes entrega un reporte mensual en Excel con las compras: fecha, ingrediente, cantidad, costo. Esto simula lo que haría un ERP real. Los participantes aprenden a cruzar datos de compras vs. ventas para calcular margen.

---

### El flujo acumulativo (cómo se conecta todo)

```
Formulario (satisfacción)  ──┐
                              ├──▶  Hoja Maestra en Excel  ──▶  Dashboard
Ventas diarias (CSV)       ──┤         (Power Query o
                              │          VLOOKUP/BUSCARV)
Compras/ERP (reporte)      ──┘
```

En la **Hoja Maestra** los participantes consolidan todo con herramientas básicas: copiar-pegar estructurado, BUSCARV, tablas dinámicas. No se necesita programar nada.

---

### El Dashboard final responde 4 preguntas de negocio

Con una tabla dinámica y gráficos básicos de Excel, el dashboard muestra: cuál es el producto más vendido y más rentable, en qué horas hay más clientes, cómo varía la satisfacción según el producto, y si el margen de ganancia está cubriendo los costos de ingredientes.

---

### Por qué funciona para el curso

Es acumulativo porque cada módulo **añade una capa** sobre la anterior. Al final, los participantes ven que la transformación digital no es tecnología compleja, sino conectar datos que ya existen para tomar mejores decisiones. Y como el caso es una cafetería, cualquier participante —sea de salud, manufactura o educación— puede traducirlo fácilmente a su propio contexto.

-----------------

El archivo **CafeDigital_Master.xlsx** tiene 5 hojas con colores de pestaña diferenciados:

**📋 Satisfaccion** (pestaña azul) — 90 registros ficticios de encuestas con fecha, hora, producto, calificación 1-5, si regresan y comentarios.

**📋 Ventas** (pestaña verde) — 120 registros de ventas diarias con fecha, hora, producto, cantidad, precio unitario, total en COP y mes. Incluye fila de totales con fórmulas.

**📋 Compras** (pestaña naranja) — 16 registros de compras a proveedores (simulando ERP) para marzo y abril, con ingrediente, proveedor, cantidad en kg y costo total.

**📋 Analisis** (pestaña azul oscuro) — 4 tablas resumen con fórmulas SUMIF y AVERAGEIF que cruzan las tres fuentes: ventas por producto, satisfacción promedio, ingresos vs. costos por mes y franjas horarias.

**📊 Dashboard** (pestaña morada) — 4 KPIs en la parte superior + 4 gráficos: ventas por producto, satisfacción por producto, ingresos vs. costos y clientes por franja horaria.

Todo está vinculado con fórmulas: si los participantes cambian un dato en las hojas fuente, el análisis y el dashboard se actualizan solos. Perfecto para mostrar el poder de la integración de datos en vivo.