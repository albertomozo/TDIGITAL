    Aquí tienes un conjunto de **ejercicios prácticos de Markdown** pensados para clase. Puedes pegarlos tal cual en un `.md` y dárselos al alumnado para que los resuelva.

***

# Ejercicios de Markdown

## Ejercicio 1: Dar formato a un texto plano

Convierte el siguiente texto plano en un documento Markdown bien estructurado con:

- Un título principal  
- Al menos dos subtítulos  
- Listas donde tenga sentido  
- Negritas y cursivas para resaltar ideas clave  

Texto a transformar:

> markdown es un lenguaje de marcado ligero. sirve para escribir de forma sencilla y luego convertir el texto a html u otros formatos. se usa mucho en documentacion tecnica, en apuntes y en repositorios de codigo como github. es importante aprender a usar encabezados, listas, enlaces, imagenes y bloques de codigo.

***

## Ejercicio 2: Encabezados y enlaces internos

1. Crea un documento con este esquema de secciones usando encabezados:

   - Título: “Guía rápida de Markdown”  
   - Sección 1: “Sintaxis básica”  
   - Sección 2: “Sintaxis avanzada”  
   - Sección 3: “Recursos recomendados”

2. Añade al principio un **índice** con enlaces internos a cada sección.

Ejemplo de lo que se espera (no copies, solo úsalo de referencia):

```markdown
[Ir a Sintaxis básica](#sintaxis-básica)
```

***

## Ejercicio 3: Arreglar una lista

Corrige la siguiente lista para que se vea correctamente como lista ordenada y con subpuntos:

```markdown
1 Primer paso Instalar el editor
2 Segundo paso Crear un archivo nuevo
- configurar el nombre del archivo
- guardar con extensión .md
3 tercer paso escribir texto con formato
- usar encabezados
- usar listas
- usar negritas y cursivas
```

Objetivo:  
- Que haya una lista ordenada principal  
- Que las acciones dependientes sean sub-listas correctamente anidadas

***

## Ejercicio 4: Imágenes y enlaces

Crea un bloque en Markdown que contenga:

- Un encabezado de nivel 2 con el texto: “Más información sobre Markdown”  
- Un párrafo con un enlace a la página oficial de Markdown  
- Una imagen con texto alternativo “Logo Markdown” (puedes usar cualquier URL de imagen o un marcador de posición, por ejemplo `https://ejemplo.com/logo.png`)

Ejemplo del formato esperado (no copies las mismas URLs necesariamente):

```markdown
## Más información sobre Markdown

Puedes encontrar más detalles en [esta página](URL_AQUI).

![Logo Markdown](URL_DE_IMAGEN_AQUI)
```

***

## Ejercicio 5: Bloques de código

Transforma este texto en un bloque de código bien formateado en Markdown, indicando el lenguaje adecuado:

> Programa en Python que pide el nombre al usuario y saluda:  
> name = input("¿Cómo te llamas? ")  
> print("Hola, " + name)

Pistas:

- Usa tres comillas invertidas  
- Indica el lenguaje después de las comillas

***

## Ejercicio 6: Tablas básicas y alineación

1. Crea una tabla con la siguiente información de alumnos:

   - Columnas: Nombre, Curso, Nota  
   - Filas:  
     - Ana, 1º DAW, 8.5  
     - Luis, 2º DAM, 7.3  
     - Marta, 1º ASIR, 9.1  

2. Modifica la tabla para que:

   - El texto de la columna “Nombre” esté alineado a la izquierda  
   - La columna “Curso” esté centrada  
   - La columna “Nota” esté alineada a la derecha

***

## Ejercicio 7: Lista de tareas (checklist)

Convierte estas instrucciones en una lista de tareas tipo checklist:

- Leer la guía básica de Markdown  
- Instalar un editor de texto compatible  
- Crear el primer documento `.md`  
- Subir el archivo a un repositorio (o plataforma) acordado en clase

Usa el formato:

```markdown
- [ ] ...
- [x] ...
```

Marca como completada solo la primera tarea.

***

## Ejercicio 8: Combinar Markdown con HTML

Crea un fragmento de documento Markdown que:

- Tenga un encabezado “Aviso importante”  
- Contenga un párrafo en HTML con el texto en rojo y negrita  
- Después del párrafo en HTML, añade una lista en Markdown con tres puntos importantes

Pista:  
Puedes usar algo similar a:

```markdown
<p style="color: red; font-weight: bold;">
Texto aquí
</p>
```

***

## Ejercicio 9: Corregir errores de Markdown

Localiza y corrige los errores de sintaxis en este fragmento:

```markdown
# Guía de Markdown avanzado

##Listas

-Elemento 1
-Elemento 2
 - Sub-elemento 2.1

##Enlaces e imagenes

[Enlace a Google] (https://www.google.com)

![Texto alternativo]https://ejemplo.com/imagen.png

```python
print("Hola mundo")
```
```

***

## Ejercicio 10: Crear una mini-guía propia

Pide al alumnado que cree su propia **mini-guía de Markdown** que incluya:

- Título y autor  
- Una breve explicación de qué es Markdown  
- Al menos:
  - Un encabezado de nivel 2  
  - Una lista ordenada y una no ordenada  
  - Un enlace externo  
  - Una tabla sencilla  
  - Un bloque de código  
- Al final, una lista de tareas con “cosas que aún quiero aprender sobre Markdown”

***

