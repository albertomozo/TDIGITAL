# Manual TDIGITAL (Markdown + IA)

---

## Índice

1. [Propósito](#proposito)
2. [Cómo usar este repositorio](#como-usar-este-repositorio)
3. [Contenido principal](#contenido-principal)
   - [Markdown: índice y guía](#markdown-indice-y-guia)
   - [Sintaxis](#sintaxis)
   - [Ejercicios](#ejercicios)
   - [Soluciones](#soluciones)
   - [Ficheros de ingeniería de prompts](#ficheros-de-ingenieria-de-prompts)
   - [Futuro de Markdown e IA](#futuro-de-markdown-e-ia)
   - [Guía de skill](#guia-de-skill)
4. [Flujo de trabajo de ejemplo](#flujo-de-trabajo-de-ejemplo)
5. [Colaboración](#colaboracion)
6. [Licencia](#licencia)

---

## Propósito

El repositorio TDIGITAL reúne recetas prácticas y minimalistas para automatizar tareas de oficina usando **IA generativa**. Cada receta incluye:

- Un **prompt listo para usar**
- Pasos claros para ejecutar la receta
- Una **comprobación mínima** para validar resultados

> ⚠️ Siempre revisa manualmente los resultados de la IA antes de usarlos en producción.

---

## Cómo usar este repositorio

1. Navega a la carpeta de la temática que quieras automatizar.
2. Copia el prompt y el texto/archivo de entrada en tu IA preferida (ChatGPT, Gemini, etc.).
3. Ejecuta el prompt y valida los resultados.

---

## Contenido principal

- `calendario/` — Prompts y ejemplos para extraer eventos de PDFs y generar CSV/ICS.
- `actas/` — Plantillas y prompts para generar actas/minutas a partir de transcripciones o notas.
- `prompts/` — Colección de prompts generales y plantillas reutilizables.
- `examples/` — Ejemplos de entrada/salida que ayudan a entender cómo usar cada receta.
- `markdown/` — Manual educativo de Markdown con teoría, sintaxis, ejercicios y tendencias.

---

## Markdown: índice y guía

Basado en `markdown/README.md`.

- `manual.md` — Introducción a Markdown, filosofía, uso con IA y sintaxis avanzada.
- `sintaxis.md` — Referencia completa de sintaxis: encabezados, párrafos, listas, enlaces, imágenes, tablas, código y más.
- `ejercicios.md` — Ejercicios prácticos para fijar conceptos.
- `soluciones.md` — Soluciones modelo para verificar resultados.
- `futuro.md` — Tendencias y usos de Markdown con IA.
- `guia_skill.md` — Markdown para estructurar el "cerebro" de la IA.
- `ficheros.md` — Ingeniería de prompts modular.

### Cómo usar el contenido de markdown/

1. Leer `manual.md` para entender qué es Markdown y sus variantes (original, CommonMark, GFM).
2. Estudiar `sintaxis.md` para dominar reglas y ejemplos.
3. Resolver `ejercicios.md` y comparar con `soluciones.md`.
4. Consultar `futuro.md` para ideas de innovación con IA y flujos de trabajo.
5. Revisar `guia_skill.md` para mejorar el nivel de prompting.

---

## Sintaxis

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

### Listas ordenadas

```markdown
1. Primer paso
2. Segundo paso
3. Tercer paso
```

***

## 4. Enlaces y URLs

```markdown
[Texto del enlace](https://ejemplo.com)
```

***

## 5. Imágenes

```markdown
![Texto alternativo](https://ruta/a/la/imagen.png)
```

***

## 6. Citas o bloques de texto

```markdown
> Este es un bloque de cita.
> Puedes escribir varias líneas aquí.
```

***

## 7. Código en línea y bloques de código

`git status` y bloques con triple backtick:

```python
def saludar():
    print("Hola Mundo")
```

***

## 8. Tablas

```markdown
| Nombre  | Rol        | País     |
|----------|------------|----------|
| Ana      | Docente    | España   |
| Luis     | Estudiante | México   |
```

***

## 9. Separadores

`---` , `***` o `___`

***

## 10. Enlaces internos (índice)

[Ir a la sección de imágenes](#5-imagenes)

***

## 11. Escape de caracteres especiales

\*no cursiva\* y \# no encabezado

---

## 12. Diferencias: Markdown estándar vs extensiones (GFM / CommonMark)

- Markdown original (John Gruber, 2004).
- GFM añade tablas, checklists, tachado y autolinks.
- CommonMark unifica comportamientos.

---

## 13. Enlaces referenciados y URLs automáticas

```markdown
[GitHub][1]

[1]: https://github.com

<https://example.com>
```

---

## 14. Saltos de línea y párrafos

- Usa dos espacios al final para salto de línea dentro de un párrafo.
- Línea en blanco para párrafos nuevos.

---

# Sintaxis avanzada de Markdown

## 1. Listas de tareas (checklists)

```markdown
- [ ] Tarea pendiente
- [x] Tarea completada
```

---

## Ejercicios

# Ejercicios de Markdown

## Ejercicio 1: Dar formato a un texto plano

Convierte el siguiente texto plano en un documento Markdown bien estructurado con:

- Un título principal  
- Al menos dos subtítulos  
- Listas donde tenga sentido  
- Negritas y cursivas para resaltar ideas clave

Texto a transformar:

> markdown es un lenguaje de marcado ligero. sirve para escribir de forma sencilla y luego convertir el texto a html u otros formatos. se usa mucho en documentacion tecnica, en apuntes y en repositorios de codigo como github. es importante aprender a usar encabezados, listas, enlaces, imagenes y bloques de codigo.

## Ejercicio 2: Encabezados y enlaces internos

1. Crea un documento con este esquema de secciones usando encabezados:
   - Título: "Guía rápida de Markdown"  
   - Sección 1: "Sintaxis básica"  
   - Sección 2: "Sintaxis avanzada"  
   - Sección 3: "Recursos recomendados"

2. Añade al principio un **índice** con enlaces internos a cada sección.

## Ejercicio 3: Arreglar una lista

Corrige la lista (ordenada con subpuntos) y conviértela en sintaxis válida.

## Ejercicio 4: Imágenes y enlaces

Crea un bloque con un encabezado, un enlace y una imagen.

## Ejercicio 5: Bloques de código

Transforma el texto de Python en un bloque de código bien formado.

## Ejercicio 6: Tablas básicas y alineación

Crea tabla con Nombre/Curso/Nota y aplica alineación.

## Ejercicio 7: Lista de tareas (checklist)

Convierte instrucciones en checklist.

## Ejercicio 8: Combinar Markdown con HTML

Usa HTML junto con Markdown.

## Ejercicio 9: Corregir errores de Markdown

Repara un fragmento con errores en encabezados, listas, enlaces e imágenes.

## Ejercicio 10: Crear una mini-guía propia

Pide al alumnado crear mini-guía con título-autor, texto, listas, enlace, tabla, código y tareas.

---

## Soluciones

# Solucionario de ejercicios Markdown

## Ejercicio 1: Dar formato a un texto plano

```markdown
# Introducción a Markdown

Markdown es un *lenguaje de marcado ligero*.  
Sirve para **escribir de forma sencilla** y luego convertir el texto a HTML u otros formatos.

## ¿Para qué se usa?

Se usa mucho en:
- Documentación técnica
- Apuntes
- Repositorios de código como GitHub

Es importante aprender a usar:
- Encabezados
- Listas
- Enlaces
- Imágenes
- Bloques de código
```

## Ejercicio 2: Encabezados y enlaces internos

```markdown
# Guía rápida de Markdown

## Índice
- [Sintaxis básica](#sintaxis-basica)
- [Sintaxis avanzada](#sintaxis-avanzada)
- [Recursos recomendados](#recursos-recomendados)

## Sintaxis básica
Contenido de la sección...

## Sintaxis avanzada
Contenido de la sección...

## Recursos recomendados
Contenido de la sección...
```

## Ejercicio 3: Arreglar una lista

```markdown
1. Primer paso: Instalar el editor
2. Segundo paso: Crear un archivo nuevo
   - Configurar el nombre del archivo
   - Guardar con extensión `.md`
3. Tercer paso: Escribir texto con formato
   - Usar encabezados
   - Usar listas
   - Usar negritas y cursivas
```

## Ejercicio 4: Imágenes y enlaces

```markdown
## Más información sobre Markdown

Puedes encontrar más detalles en  
[esta página](https://daringfireball.net/projects/markdown/).

![Logo Markdown](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)
```

## Ejercicio 5: Bloques de código

```python
name = input("¿Cómo te llamas? ")
print("Hola, " + name)
```

## Ejercicio 6: Tablas básicas y alineación

```markdown
| Nombre | Curso   | Nota |
|:-------|:-------:|-----:|
| Ana    | 1º DAW  |  8.5 |
| Luis   | 2º DAM  |  7.3 |
| Marta  | 1º ASIR |  9.1 |
```

## Ejercicio 7: Lista de tareas (checklist)

```markdown
- [x] Leer la guía básica de Markdown
- [ ] Instalar un editor de texto compatible
- [ ] Crear el primer documento `.md`
- [ ] Subir el archivo a un repositorio (o plataforma) acordado en clase
```

## Ejercicio 8: Combinar Markdown con HTML

```markdown
# Aviso importante

<p style="color: red; font-weight: bold;">
Este es un aviso importante para todo el alumnado.
</p>

- Leer las instrucciones con atención
- Entregar las tareas en plazo
- Consultar dudas al docente cuando sea necesario
```

## Ejercicio 9: Corregir errores de Markdown

```markdown
# Guía de Markdown avanzado

## Listas

- Elemento 1
- Elemento 2
  - Sub-elemento 2.1

## Enlaces e imágenes

[Enlace a Google](https://www.google.com)

![Texto alternativo](https://ejemplo.com/imagen.png)

```python
print("Hola mundo")
```
```

## Ejercicio 10: Mini-guía (posible solución ejemplo)

```markdown
# Mini-guía de Markdown
Autor: Nombre del Alumno

Markdown es un lenguaje de marcado ligero que permite dar formato al texto de forma sencilla.

## Elementos básicos

Lista no ordenada:
- Encabezados
- Listas
- Enlaces

Lista ordenada:
1. Escribir texto
2. Aplicar formato
3. Exportar o compartir

Enlace externo:  
Visita [GitHub Docs sobre Markdown](https://docs.github.com/en).

Tabla sencilla:

| Elemento   | Tipo     |
|:----------|:---------|
| `#`       | Encabezado |
| `-`       | Lista     |
| `[]()`    | Enlace    |

Bloque de código:

```bash
echo "Hola Markdown"
```

## Cosas que aún quiero aprender sobre Markdown

- [ ] Crear plantillas complejas
- [ ] Integración con otros lenguajes (LaTeX, etc.)
- [ ] Automatizar documentación


---

## Ficheros de ingeniería de prompts

Cuando pasas de usar un solo prompt a gestionar archivos Markdown, estás haciendo **Ingeniería de Prompts Modular**. Aquí tienes tres usos avanzados:

- Skill.md (prompts estructurados)
- Library.md (biblioteca de conocimiento)
- Style_Voice.md (manual de identidad)
- Master_Orchestrator.md (director de orquesta)

---

## Futuro de Markdown e IA

## El futuro de Markdown

Markdown nació como un lenguaje de marcado ligero para escribir texto legible y convertirlo a HTML, pero ahora se usa como protocolo de colaboración humano‑IA.

### 1. Markdown como “protocolo” de colaboración humano‑IA

- Documentar problemas y soluciones trabajadas con IA.
- Guardar prompts complejos en archivos.

### 2. Markdown para prompts estructurados

Patrón típico:

```markdown
# Rol
Actúa como ...

# Tarea
Tu objetivo es ...

# Requisitos
- ...

# Formato de salida
- ...
```

### 3. Markdown como “lenguaje de programación” asistido por IA

- Especificaciones en Markdown que IA transforma en código.

### 4. Markdown en infraestructura y web

- Plataformas que sirven contenido en Markdown de forma nativa.

### 5. Qué significa esto para docentes y estudiantes

- Markdown ya no solo es documentar, sino diseñar prompts y flujos de trabajo IA.

---

## Guía de skill

El archivo `skill.md` es una técnica modular. Organiza:

1. Rol
2. Contexto
3. Habilidades
4. Restricciones
5. Formato de salida
6. Ejemplos

---

## Flujo de trabajo de ejemplo

1. Selecciona el caso de uso.
2. Carga tu fuente (documento, transcripción, formulario, etc.).
3. Aplica el prompt base y ajusta parámetros.
4. Revisa la salida y corrige.
5. Guarda en el formato final (`.md`, `.pdf`, `.csv`, etc.).

---

## Colaboración

- Abre un issue con ideas o mejoras.
- Envía un pull request con nuevas recetas, ejemplos o mejoras de documentación.

---

## Licencia

MIT
