Para importar estos ejercicios a Google Forms de forma masiva (sin tener que ir uno por uno), existen dos métodos principales. El más profesional y rápido es usar un pequeño Script (Google Apps Script) que crea el formulario automáticamente por ti.

## Opción A: Forms automatico con Google script

Aquí tienes los pasos y el código listo para usar:


Este documento contiene la solución técnica para automatizar la creación de los 20 ejercicios de KPIs con identificación de alumnos.

1. Preparación:

Crea un Formulario de Google vacío y copia su ID (el código largo en la URL).

Abre un Google Sheets, ve a Extensiones > Apps Script y pega el siguiente código sustituyendo la ID.

2. Código Definitivo (Copia y Pega):

```Javascript 
function crearTestKPIsFinal() {
  var idFormulario = 'TU_ID_AQUÍ'; // <--- PEGA TU ID
  var form = FormApp.openById(idFormulario);
  
  // Limpiar y configurar
  var items = form.getItems();
  for (var i = items.length - 1; i >= 0; i--) { form.deleteItem(items[i]); }
  form.setTitle('Certificación Práctica: KPIs y Estrategia Digital');
  form.setDescription('Módulo 1: Gestión Estratégica. Transforma cada objetivo en un KPI SMART.');

  // SECCIÓN 1: Identificación
  form.addTextItem().setTitle("Nombre y Apellidos").setRequired(true);
  form.addTextItem().setTitle("Correo Electrónico").setRequired(true);
  form.addPageBreakItem().setTitle("Bloque Práctico: Definición de KPIs SMART");

  // SECCIÓN 2: 20 Ejercicios
  var objetivos = [
    "Más seguidores en Instagram", "Formar empleados en nuevas tecnologías", 
    "Responder más rápido al soporte", "Lanzar nuevos productos", 
    "Conseguir más reuniones de ventas", "Reducir carritos abandonados",
    "Ser empresa más ecológica", "Mejorar calidad de leads", 
    "Entregar pedidos más rápido", "Gastar menos en oficina",
    "Reuniones diarias más cortas", "Web más estable", 
    "Reducir rotación de personal", "Mejorar retorno de anuncios",
    "Fomentar uso de Notion/herramientas", "Bajar errores de fabricación",
    "Expandir ventas nacionales", "Aumentar apertura de emails",
    "Hacer la app más intuitiva", "Aumentar margen de beneficio"
  ];

  for (var j = 0; j < objetivos.length; j++) {
    form.addParagraphTextItem()
        .setTitle("Ejercicio " + (j + 1) + ": " + objetivos[j])
        .setHelpText("Redacta el KPI: Qué, Cuánto y Cuándo.")
        .setRequired(true);
  }
}
```


## Opción B: Copia y Pega Manual Optimizado
Si prefieres no usar código, la forma más rápida es tener la lista preparada para copiar y pegar. Aquí te dejo los enunciados limpios:

Instrucciones para Google Forms:

Crea un formulario nuevo.

Añade una pregunta de tipo "Párrafo".

Copia cada línea de esta lista:

Seguidores: Queremos tener más seguidores en Instagram.

Formación: Hay que formar a los empleados en nuevas tecnologías.

Soporte: Responder más rápido a los correos de soporte.

Innovación: Lanzar nuevos productos al mercado.

Ventas: Conseguir más reuniones con clientes potenciales.

E-commerce: Reducir la cantidad de gente que deja el carrito abandonado.

Sostenibilidad: Ser una empresa más ecológica y gastar menos papel.

Marketing: Mejorar la calidad de los leads que recibimos.

Logística: Entregar los pedidos más rápido.

Costes: Gastar menos en material de oficina este año.

Agilidad: Que las reuniones diarias (Daily) duren menos.

IT: Que la web no se caiga tanto.

Talento: Que la gente no se vaya de la empresa.

Ads: Que los anuncios en Google funcionen mejor.

Herramientas: Que todos usen la herramienta colaborativa (ej. Notion).

Calidad: Tener menos fallos en la cadena de producción.

Expansión: Vender más fuera de nuestra provincia.

Email: Que más gente lea nuestro boletín semanal.

UX: Que la aplicación sea más fácil de usar.

Finanzas: Aumentar los beneficios totales de la empresa.

Consejo para tu Clase en Directo:
Cuando uses el Google Form, recuerda ir a la pestaña "Respuestas" y activar el icono verde (Crear hoja de cálculo).