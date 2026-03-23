    Perfecto, Alberto. Aquí tienes un documento en **formato Markdown (.md)** con la **sintaxis básica**, explicado paso a paso y listo para copiar directamente a tu manual o archivo de ejemplo. He añadido ejemplos reales y comentarios breves para hacerlo útil en clase.

***

# Guía básica de sintaxis Markdown

Markdown permite escribir texto con formato de forma sencilla y legible. A continuación se presentan los elementos más comunes con ejemplos que puedes probar directamente.

***

## 1. Encabezados

Usa el símbolo `#` para crear títulos.  
Cuantos más `#`, menor es el nivel del encabezado.

```markdown
# Título principal (h1)
## Subtítulo (h2)
### Sección (h3)
#### Subsección (h4)
##### Detalle (h5)
###### Nivel más bajo (h6)
```

**Ejemplo:**

# Título principal (h1)
## Subtítulo (h2)
### Sección (h3)

***

## 2. Énfasis de texto

Markdown permite resaltar texto con *cursivas*, **negritas** o ***ambas*** usando asteriscos o guiones bajos.

```markdown
*Texto en cursiva*  
**Texto en negrita**  
***Texto en negrita y cursiva***  
~~Texto tachado~~
```

**Ejemplo:**

*Texto en cursiva*  
**Texto en negrita**  
***Texto en negrita y cursiva***  
~~Texto tachado~~

***

## 3. Listas

### Listas no ordenadas  

Usa `-`, `*` o `+` seguido de un espacio.

```markdown
- Elemento 1
- Elemento 2
  - Sub-elemento 2.1
  - Sub-elemento 2.2
```

**Ejemplo:**

- Elemento 1  
- Elemento 2  
  - Sub-elemento 2.1  
  - Sub-elemento 2.2  

### Listas ordenadas  

Usa números seguidos de un punto.

```markdown
1. Primer paso
2. Segundo paso
3. Tercer paso
```

**Ejemplo:**

1. Primer paso  
2. Segundo paso  
3. Tercer paso  

***

## 4. Enlaces y URLs

Puedes insertar enlaces con esta sintaxis:

```markdown
[Texto del enlace](https://ejemplo.com)
```

**Ejemplo:**

[Visita la página de Markdown](https://daringfireball.net/projects/markdown/)

***

## 5. Imágenes

Las imágenes se insertan igual que los enlaces, pero con un signo de exclamación `!` delante.

```markdown
![Texto alternativo](https://ruta/a/la/imagen.png)
```

**Ejemplo:**



***

## 6. Citas o bloques de texto

Usa `>` para crear citas o resaltados de párrafos.

```markdown
> Este es un bloque de cita.
> Puedes escribir varias líneas aquí.
```

**Ejemplo:**

> Este es un bloque de cita.  
> Puedes escribir varias líneas aquí.

***

## 7. Código en línea y bloques de código

Para código dentro de una línea, usa comillas invertidas (\`).

```markdown
Usa el comando `git status` para ver el estado de tu repositorio.
```

Para bloques de código, usa tres comillas invertidas (```) y, opcionalmente, indica el lenguaje:

    ```python
    def saludar():
        print("Hola Mundo")
    ```

**Ejemplo:**

```python
def saludar():
    print("Hola Mundo")
```

***

## 8. Tablas

Puedes crear tablas usando barras verticales `|` y guiones.

```markdown
| Nombre  | Rol        | País     |
|----------|------------|----------|
| Ana      | Docente    | España   |
| Luis     | Estudiante | México   |
```

**Ejemplo:**

| Nombre  | Rol        | País     |
|----------|------------|----------|
| Ana      | Docente    | España   |
| Luis     | Estudiante | México   |

***

## 9. Separadores

Usa tres o más guiones (`---`), asteriscos (`***`) o guiones bajos (`___`) para una línea divisoria.

```markdown
---
```

**Ejemplo:**

***

## 10. Enlaces internos (índice)

Puedes enlazar secciones dentro del mismo archivo usando el texto del encabezado en minúsculas y reemplazando los espacios por guiones.

```markdown
[Ir a la sección de imágenes](#5-imágenes)
```

**Nota:** la forma exacta del enlace interno depende del renderizador. GitHub simplifica los acentos y los símbolos especiales.

## 11. Escape de caracteres especiales

Markdown interpreta caracteres como `*`, `_`, `#`, `[`, `]`, `(`, `)`, `>`, `-` y `!`. Si quieres mostrarlos literalmente, precede con barra invertida (`\`).

```markdown
\*no cursiva\* y \# no encabezado
``` 

## 12. Diferencias: Markdown estándar vs extensiones (GFM / CommonMark)

- Markdown original (John Gruber, 2004) contempla encabezados, listas, énfasis, enlaces, imágenes, citas, código y párrafos.
- GitHub Flavored Markdown (GFM) añade tablas, listas de tareas, tachado (`~~`), blocs de código con resaltado y autolinks.
- CommonMark es una especificación estricta y moderna que unifica el comportamiento entre motores.

Los ejemplos vistos en esta guía están orientados a GFM; en entornos estrictos es posible que algunas funciones no funcionen (tablas, checklist, tachado).

## 13. Enlaces referenciados y URLs automáticas

Enlaces referenciados:

```markdown
[GitHub][1]

[1]: https://github.com
```

URLs automáticas:

```markdown
<https://example.com>
```

## 14. Saltos de línea y párrafos

En Markdown, un salto de línea simple no crea un nuevo párrafo. Para forzar un salto de línea usa dos espacios al final de la línea o escribe una línea en blanco entre párrafos.

```markdown
Primera línea con dos espacios al final.  
Segunda línea.

Nuevo párrafo.
```
**Ejemplo:**

[Ir a la sección de imágenes](#5-imágenes)

***


# Sintaxis avanzada de Markdown

En esta sección se muestran elementos más avanzados y extensiones comunes que encontrarás en muchas plataformas (especialmente en GitHub y otros entornos de desarrollo). [freecodecamp](https://www.freecodecamp.org/news/github-flavored-markdown-syntax-examples/)

***

## 1. Listas de tareas (checklists)

Las listas de tareas son muy útiles para gestionar pendientes en documentación, repositorios o apuntes de clase. [github](https://github.blog/news-insights/product-news/task-lists-in-all-markdown-documents/)
Se escriben como una lista normal, pero con corchetes `[]` o `[x]`.

```markdown
- [ ] Tarea pendiente
- [x] Tarea completada
- [ ] Revisar ejercicios de Markdown
```

**Ejemplo:**

- [ ] Tarea pendiente  
- [x] Tarea completada  
- [ ] Revisar ejercicios de Markdown  

***

## 2. Tablas con alineación

Además de las tablas básicas, puedes **alinear** el contenido de las columnas usando dos puntos `:` en la fila del encabezado. [markdowncheatsheet](https://markdowncheatsheet.com/reference/tables)

```markdown
| Alineación    | Sintaxis   | Ejemplo      |
|:--------------|:----------:|-------------:|
| Izquierda     | `:---`     | texto        |
| Centrada      | `:---:`    | centrado     |
| Derecha       | `---:`     |      123.45  |
```

**Ejemplo:**

| Alineación    | Sintaxis   | Ejemplo      |
|:--------------|:----------:|-------------:|
| Izquierda     | `:---`     | texto        |
| Centrada      | `:---:`    | centrado     |
| Derecha       | `---:`     |      123.45  |

***

## 3. Emojis

Muchas plataformas permiten insertar emojis usando códigos entre dos puntos, por ejemplo `:smile:`. [ecweb.ecer](https://ecweb.ecer.com/topic/en/detail-287446-guide_to_using_emojis_in_professional_documentation.html)
El soporte depende del motor de renderizado (no todos lo interpretan igual). [agenda](https://agenda.community/t/add-markdown-emoji-markup-support-or-similar/3175)

```markdown
Texto con emoji :smile:  
Documento aprobado :white_check_mark:  
¡Alerta importante! :warning:
```

**Ejemplo (si la plataforma lo soporta):**

Texto con emoji :smile:  
Documento aprobado :white_check_mark:  
¡Alerta importante! :warning:  

***

## 4. Combinación con HTML

La mayoría de intérpretes de Markdown permiten **insertar HTML embebido**, útil cuando Markdown se queda corto (por ejemplo, estilos especiales o estructuras complejas). [discourse.gohugo](https://discourse.gohugo.io/t/markdown-not-being-rendered-within-html-block/2532)
Ten en cuenta que algunos motores desactivan parte del HTML por seguridad. [forums.docker](https://forums.docker.com/t/support-for-inline-html-in-markdown-description/1644)

```markdown
<p style="color: red; font-weight: bold;">
Este texto está en HTML dentro de un documento Markdown.
</p>

<div>
  <strong>Negrita en HTML</strong> y *cursiva en Markdown* en el mismo documento.
</div>
```

En muchos casos el HTML se respeta exactamente como se escribe, mientras que el texto fuera de estas etiquetas se procesa como Markdown normal. [discourse.gohugo](https://discourse.gohugo.io/t/markdown-not-being-rendered-within-html-block/2532)

***

## 5. Bloques de código avanzados

Además de indicar el lenguaje para **resaltado de sintaxis**, puedes incluir bloques largos de código, salidas de consola o pseudocódigo. [freecodecamp](https://www.freecodecamp.org/news/github-flavored-markdown-syntax-examples/)

```markdown
```bash
# Instalar dependencias
npm install

# Ejecutar el proyecto
npm run dev
```
```

**Ejemplo:**

```bash
# Instalar dependencias
npm install

# Ejecutar el proyecto
npm run dev
```

***

## 6. Comentarios “ocultos” (según la plataforma)

Markdown estándar no define comentarios, pero en muchos entornos se usan comentarios HTML para dejar notas que no se muestran al renderizarse. [discourse.gohugo](https://discourse.gohugo.io/t/markdown-not-being-rendered-within-html-block/2532)

```markdown
<!-- Este texto no se verá en el documento final -->
Este sí será visible.
```

**Ejemplo:**

<!-- Este texto no se verá en el documento final -->
Este sí será visible.

***

## 7. Buenas prácticas para docentes

- Usa listas de tareas para planificar **actividades o entregas** del alumnado. [github](https://github.blog/news-insights/product-news/task-lists-in-all-markdown-documents/)
- Alinea números a la derecha en tablas (notas, tiempos, cantidades) para facilitar su lectura. [technicalwritingmp](https://technicalwritingmp.com/docs/advanced-syntax-formatting-in-markdown/)
- Emplea emojis solo cuando aporten claridad o motivación, evitando saturar documentos formales. [help.tempo](https://help.tempo.io/structure/latest/text-formatting-with-emojis-and-markdown)
- Recurre a HTML embebido solo cuando Markdown no sea suficiente, y documenta a tu alumnado qué partes pertenecen a cada lenguaje. [discourse.gohugo](https://discourse.gohugo.io/t/markdown-not-being-rendered-within-html-block/2532)

***

## 8. Visualizadores, editores y exportación de Markdown

### 8.1. Visualizadores (renderizadores)

- GitHub (web): renderiza `README.md`, wikis y issues.
- GitLab (web): renderiza Markdown en repos de proyectos.
- Markdown Preview (VSCode): vista en tiempo real dentro del editor.
- Obsidian/Logseq: visualizador local para notas con preview instantáneo.
- Typora: entrada WYSIWYG y renderizado inmediato.

### 8.2. Editores recomendados

- Visual Studio Code + extensión `Markdown All in One`.
- Obsidian (notas enlazadas y plugins).
- Typora (edición casi WYSIWYG y soporte de tablas, ecuaciones y diagramas).
- Atom con `markdown-preview`.
- StackEdit (web offline-ready).

### 8.3. Exportación a otros formatos

Markdown se convierte a formatos estáticos y finales mediante herramientas:

- Pandoc (comando CLI pesado y flexible): `pandoc input.md -o output.pdf` o `-o output.docx`.
- Markdown-it / Remark (JS): para generar HTML personalizado.
- Hugo / Jekyll / MkDocs: transforma Markdown en sitios web estáticos.
- VSCode: `Ctrl+Shift+P > Markdown: Open Preview to the Side` y luego “Export as PDF” con impresora virtual / extensión.
- Obsidian: exportar a PDF/HTML (plugin o nativo según versión).

### 8.4. Consejo de compatibilidad

- Comprueba el dialecto que usas (GFM, CommonMark, MultiMarkdown). Algunas funciones (tablas, footnotes, task list) pueden fallar en renderizadores estrictos.
- Usa un pipeline de validación (https://github.com/igorshubovych/markdownlint, https://github.com/remarkjs/remark-lint) antes de la exportación.
- Haz pruebas en la plataforma de destino (GitHub/GitLab/Notion) porque cada motor interpreta de forma ligeramente diferente.