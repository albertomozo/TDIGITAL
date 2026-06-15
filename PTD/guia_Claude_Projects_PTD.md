# 🧠 Guía: Cómo usar Claude Projects para elaborar Planes de Transformación Digital (PTD)

> Guía práctica paso a paso para configurar un **Proyecto en Claude** como asistente especializado en transformación digital, capaz de acompañar todo el proceso de elaboración del PTD con contexto persistente, base de conocimiento propia y comportamiento personalizado.

---

## 📋 Índice

1. [¿Qué es Claude Projects y por qué usarlo para el PTD?](#1-qué-es-claude-projects-y-por-qué-usarlo-para-el-ptd)
2. [Requisitos previos: plan y acceso](#2-requisitos-previos-plan-y-acceso)
3. [Paso 1 – Crear el Proyecto en Claude](#3-paso-1--crear-el-proyecto-en-claude)
4. [Paso 2 – Configurar las Instrucciones del Proyecto (System Prompt)](#4-paso-2--configurar-las-instrucciones-del-proyecto-system-prompt)
5. [Paso 3 – Construir la Base de Conocimiento](#5-paso-3--construir-la-base-de-conocimiento)
6. [Paso 4 – Flujo de trabajo: elaborar el PTD sección por sección](#6-paso-4--flujo-de-trabajo-elaborar-el-ptd-sección-por-sección)
7. [Paso 5 – Gestionar el historial y la memoria del proyecto](#7-paso-5--gestionar-el-historial-y-la-memoria-del-proyecto)
8. [Paso 6 – Colaboración en equipo (planes Team/Enterprise)](#8-paso-6--colaboración-en-equipo-planes-teamenterprise)
9. [Buenas prácticas y errores frecuentes](#9-buenas-prácticas-y-errores-frecuentes)
10. [Plantilla de instrucciones lista para copiar](#10-plantilla-de-instrucciones-lista-para-copiar)

---

## 1. ¿Qué es Claude Projects y por qué usarlo para el PTD?

Claude Projects son **espacios de trabajo aislados** dentro de claude.ai que combinan tres elementos clave:

| Elemento | Qué hace | Beneficio para el PTD |
|---|---|---|
| **Instrucciones personalizadas** | Define el rol, tono y comportamiento de Claude para ese proyecto | Claude actúa siempre como consultor de transformación digital, sin necesidad de explicarlo en cada chat |
| **Base de conocimiento (Knowledge Base)** | Archivos y documentos que Claude consulta en cada conversación | Sube la plantilla PTD, ejemplos de otros planes, datos de la empresa y Claude los usa automáticamente |
| **Historial de conversaciones** | Las conversaciones dentro del proyecto se mantienen y organizan | Puedes retomar el trabajo donde lo dejaste, sin perder contexto |

**¿Por qué no usar Claude normal?**

En el chat convencional de Claude, cada conversación empieza desde cero. Para elaborar un PTD —que tiene 5 secciones interconectadas, documentación de la empresa y un proceso que puede durar días o semanas— necesitas que Claude recuerde el contexto, la empresa, y cómo quieres trabajar. Projects resuelve exactamente eso.

---

## 2. Requisitos previos: plan y acceso

| Plan | Projects | Proyectos compartidos | Recomendado para |
|---|---|---|---|
| **Free** | ✅ Hasta 5 proyectos | ❌ | Uso individual, pruebas |
| **Pro** (~20 $/mes) | ✅ Ilimitados + RAG ampliado | ❌ | Un consultor o alumno trabajando solo |
| **Team** (~25 $/usuario/mes) | ✅ Ilimitados + RAG | ✅ Compartir con el equipo | Grupos de trabajo, consultoras |
| **Enterprise** | ✅ Todo lo anterior + SSO/SAML | ✅ Con permisos granulares | Organizaciones grandes |

> 💡 **Para un trabajo académico o de prácticas**, el plan **Pro** es suficiente. Para un equipo consultor que trabaja con varios clientes simultáneos, considerar **Team**.

---

## 3. Paso 1 – Crear el Proyecto en Claude

### Instrucciones

1. Accede a [claude.ai](https://claude.ai) e inicia sesión.
2. En el menú lateral izquierdo, localiza la sección **"Projects"** y haz clic en **"New Project"**.
3. Asigna un nombre descriptivo. Ejemplos:

```
PTD – [Nombre de la Empresa] – [Año]
PTD Consultoría – Cliente: Panadería García 2025
Taller PTD – Grupo 3 – Master Digitalización
```

4. Añade una descripción breve (opcional, pero útil si tienes varios proyectos):

```
Proyecto para elaborar el Plan de Transformación Digital completo de [empresa].
Incluye diagnóstico, análisis estratégico, madurez digital y propuesta de herramientas.
```

5. Haz clic en **"Create Project"**.

---

## 4. Paso 2 – Configurar las Instrucciones del Proyecto (System Prompt)

Este es el paso más importante. Las instrucciones del proyecto funcionan como un **"briefing permanente"** que Claude leerá al inicio de cada conversación dentro del proyecto.

### Cómo acceder

Una vez dentro del proyecto, haz clic en **"Set project instructions"** o el ícono de configuración (⚙️).

### Qué incluir en las instrucciones

Las instrucciones deben cubrir cinco bloques:

```
1. ROL Y EXPERTISE
2. DATOS DE LA EMPRESA (o placeholder si es plantilla reutilizable)
3. ESTRUCTURA DEL PTD
4. FORMATO Y ESTILO DE RESPUESTA
5. RESTRICCIONES Y COMPORTAMIENTO
```

> 👉 En la **Sección 10** de esta guía encontrarás la plantilla completa lista para copiar y pegar.

### Ejemplo de instrucciones mínimas (versión corta)

```
Eres un consultor senior de transformación digital especializado en pymes.
Estás ayudando a elaborar el Plan de Transformación Digital (PTD) de [NOMBRE_EMPRESA],
una empresa del sector [SECTOR] con [Nº] empleados ubicada en [CIUDAD].

El PTD sigue esta estructura:
1. Portada e Identificación
2. Diagnóstico y Reflexión Estratégica (Misión/Visión/Valores + DAFO)
3. Análisis del Entorno (PESTEL + Benchmarking + 5 Fuerzas de Porter)
4. Test de Madurez Digital (Diagnóstico Acelera Pyme)
5. Áreas de Actuación y Propuesta de Herramientas

Responde siempre en español. Usa formato markdown con tablas cuando sea útil.
Cuando no tengas información suficiente sobre la empresa, pregunta antes de asumir.
Mantén un tono profesional pero accesible.
```

---

## 5. Paso 3 – Construir la Base de Conocimiento

La base de conocimiento es el "cerebro especializado" de tu proyecto. Claude consultará estos documentos automáticamente cuando sean relevantes.

### Archivos recomendados para un proyecto PTD

Organiza los documentos en tres categorías:

#### 📁 Categoría A — Plantillas y metodología (siempre presentes)

| Archivo | Descripción |
|---|---|
| `PTD_01_plantilla.pdf` | La plantilla base oficial del PTD |
| `guia_PTD_prompts_IA.md` | Esta misma guía (como referencia metodológica) |
| `ejemplos_PTD_completos/` | 1-2 PTDs de ejemplo de otros sectores (si los tienes) |
| `herramientas_digitales_pymes_2025.md` | Lista de herramientas recomendadas por categoría y precio |

#### 📁 Categoría B — Datos de la empresa (específicos de cada caso)

| Archivo | Descripción |
|---|---|
| `empresa_descripcion.txt` | Descripción general, historia, servicios, mercado |
| `empresa_entrevista.pdf` | Notas o transcripción de la entrevista con el cliente |
| `empresa_web_captura.pdf` | Captura o export de la web actual (si existe) |
| `empresa_competidores.txt` | Lista de competidores identificados |
| `empresa_procesos_actuales.docx` | Descripción de los procesos internos actuales |

#### 📁 Categoría C — Contexto sectorial (opcional pero valioso)

| Archivo | Descripción |
|---|---|
| `informe_sector_[X]_2025.pdf` | Informe de tendencias del sector |
| `kit_digital_soluciones.pdf` | Catálogo de soluciones subvencionables Kit Digital |
| `pestel_[sector]_referencia.md` | Factores PESTEL preelaborados para el sector |

### Cómo subir archivos

1. Dentro del proyecto, haz clic en **"Add content"** o el ícono de archivos.
2. Puedes subir desde:
   - **Tu dispositivo**: arrastra o selecciona archivos
   - **Google Drive**: conecta tu cuenta y selecciona documentos
   - **GitHub**: enlaza un repositorio
   - **Texto pegado**: copia y pega contenido directamente
3. Formatos soportados: PDF, DOCX, TXT, CSV, HTML, MD y más.
4. Límite por archivo: **30 MB**. El total debe caber en la ventana de contexto (~200.000 tokens ≈ 500 páginas).

### ⚠️ Consejo crítico sobre los archivos

> Nombra los archivos de forma descriptiva. Claude usa el nombre del archivo para entender qué contiene.
>
> ✅ `empresa_panaderia_garcia_descripcion_2025.txt`
> ❌ `documento1.txt`

---

## 6. Paso 4 – Flujo de trabajo: elaborar el PTD sección por sección

Una vez configurado el proyecto, trabaja **sección a sección en conversaciones separadas** dentro del mismo proyecto. Esto mantiene el contexto limpio y las conversaciones organizadas.

### Estructura de chats recomendada

```
Proyecto: PTD – Panadería García
│
├── 💬 Chat 1: "Portada y datos del equipo"
├── 💬 Chat 2: "Misión, Visión y Valores"
├── 💬 Chat 3: "Análisis DAFO"
├── 💬 Chat 4: "Análisis PESTEL"
├── 💬 Chat 5: "Benchmarking competidores"
├── 💬 Chat 6: "5 Fuerzas de Porter"
├── 💬 Chat 7: "Diagnóstico madurez digital"
├── 💬 Chat 8: "Propuesta de herramientas"
└── 💬 Chat 9: "Revisión y coherencia global"
```

### Prompts de arranque para cada chat (optimizados para Projects)

Dado que las instrucciones del proyecto ya dan contexto completo sobre la empresa, los prompts dentro del proyecto pueden ser más directos:

---

**Chat 1 – Portada**
```
Genera la portada e identificación del PTD.
Equipo: [NOMBRE 1] ([EDAD], [FORMACIÓN]), [NOMBRE 2] ([EDAD], [FORMACIÓN]).
Responsable: [NOMBRE], email: [EMAIL].
```

---

**Chat 2 – Misión, Visión, Valores**
```
Basándote en la información de la empresa que tienes disponible, 
redacta la identidad corporativa: Misión, Visión y 5 Valores.
Si necesitas datos adicionales para ser más preciso, pregúntame.
```

---

**Chat 3 – DAFO**
```
Elabora el análisis DAFO completo en tabla markdown (4 cuadrantes, 5 ítems cada uno).
Fundamenta cada ítem en los datos reales de la empresa y el sector.
```

---

**Chat 4 – PESTEL**
```
Desarrolla el análisis PESTEL orientado a la digitalización de la empresa.
Tabla markdown: Dimensión | Factor | Descripción | Impacto (Alto/Medio/Bajo).
3 factores por dimensión. Referencia regulación española vigente donde aplique.
```

---

**Chat 5 – Benchmarking**
```
Realiza el benchmarking de 3-4 competidores o referentes del sector.
Incluye: modelo de negocio, estrategia digital, innovaciones y lección aprendida.
Tabla comparativa en markdown.
```

---

**Chat 6 – Porter**
```
Aplica el modelo de las 5 Fuerzas de Porter.
Para cada fuerza: descripción, intensidad (Alta/Media/Baja) e implicación digital.
Cierra con una síntesis estratégica de 3-4 líneas.
```

---

**Chat 7 – Madurez Digital**
```
Simula el test de diagnóstico de madurez digital (estilo Acelera Pyme).
Genera: índice global (escala 0-100), desglose por las 5 áreas operativas 
con porcentaje, y lista de las 3 brechas más críticas detectadas.
```

---

**Chat 8 – Herramientas**
```
Basándote en las brechas identificadas en el diagnóstico de madurez digital,
propón las áreas de actuación prioritarias y recomienda herramientas digitales 
específicas para cada una.
Incluye: nombre, función, coste estimado, dificultad y compatibilidad Kit Digital.
Finaliza con una hoja de ruta en 3 fases: 0-3 meses / 3-9 meses / 9-18 meses.
```

---

**Chat 9 – Revisión final**
```
Revisa la coherencia global del PTD:
1. ¿Las herramientas propuestas en la Sección 5 responden a las brechas de la Sección 4?
2. ¿El DAFO y el PESTEL son consistentes entre sí?
3. ¿La hoja de ruta es realista para el tamaño y recursos de la empresa?
Señala cualquier contradicción o gap y sugiere correcciones.
```

---

## 7. Paso 5 – Gestionar el historial y la memoria del proyecto

### Lo que Claude recuerda automáticamente

✅ El contenido de los archivos subidos a la base de conocimiento.
✅ Las instrucciones del proyecto (en cada conversación).

### Lo que NO persiste automáticamente entre chats

❌ El contenido generado en conversaciones anteriores (cada chat es independiente).

### Solución: convertir outputs en conocimiento persistente

Para que Claude use el trabajo previo en chats futuros, tienes dos opciones:

**Opción A – Añadir outputs a la Knowledge Base**

1. Al terminar cada sección, copia el resultado en un archivo `.txt` o `.md`.
2. Nómbralo claramente: `PTD_seccion2_DAFO_final.md`
3. Súbelo a la base de conocimiento del proyecto.
4. En chats futuros, Claude lo consultará automáticamente.

**Opción B – Crear un documento de síntesis progresivo**

Mantén un único documento `PTD_borrador_acumulado.md` que actualices manualmente tras cada chat y re-subas al proyecto. Claude siempre leerá la versión más reciente.

```markdown
# PTD Borrador Acumulado – [Empresa] – v[X]
_Última actualización: [fecha]_

## Sección 1 – Portada ✅ [completada]
[contenido final aquí]

## Sección 2 – Identidad Corporativa ✅ [completada]
[contenido final aquí]

## Sección 3 – DAFO ✅ [completada]
[contenido final aquí]

## Sección 4 – PESTEL 🔄 [en progreso]
...
```

---

## 8. Paso 6 – Colaboración en equipo (planes Team/Enterprise)

Si trabajáis en grupo (varios alumnos o consultores), el plan **Team** permite compartir el proyecto completo.

### Cómo compartir un proyecto

1. Dentro del proyecto, accede a **"Share"** o **"Manage members"**.
2. Invita a miembros por su email de Claude.
3. Define los permisos:
   - **Editor**: puede añadir archivos, editar instrucciones y crear chats.
   - **Viewer**: solo puede leer el historial y hacer nuevos chats.

### Buenas prácticas en equipos

| Práctica | Por qué |
|---|---|
| Asignar una sección del PTD a cada miembro | Evita duplicidades y conflictos de contexto |
| Acordar el formato de nombres de chat antes de empezar | Facilita navegar el historial del equipo |
| Designar un "gestor de Knowledge Base" | Una persona responsable de mantener los archivos actualizados |
| No editar las instrucciones del proyecto sin consenso | Cambiar el system prompt afecta a todos los chats del equipo |
| Revisar los outputs de otros miembros antes de subirlos como KB | Controlar la calidad del conocimiento que Claude va a usar |

---

## 9. Buenas prácticas y errores frecuentes

### ✅ Buenas prácticas

- **Un proyecto por empresa/cliente**: nunca mezcles datos de diferentes empresas en el mismo proyecto.
- **Actualiza los archivos cuando cambien**: si cambian los datos de la empresa o los precios de herramientas, re-sube el documento.
- **Incluye ejemplos en las instrucciones**: en lugar de decir "responde de forma concisa", muestra un ejemplo de respuesta ideal directamente en las instrucciones.
- **Usa el chat de revisión final** (Chat 9) antes de exportar el documento definitivo.
- **Nombra los chats descriptivamente**: así puedes navegar el historial fácilmente semanas después.

### ❌ Errores frecuentes a evitar

| Error | Consecuencia | Solución |
|---|---|---|
| Subir archivos sin limpiar (con secciones irrelevantes) | Claude "contamina" sus respuestas con información innecesaria | Limpia los PDFs antes de subirlos; elimina páginas que no aporten |
| Confiar en que Claude "recuerda" chats anteriores | Respuestas incoherentes entre secciones | Usa el documento borrador acumulado como KB |
| Instrucciones del proyecto demasiado largas o contradictorias | Claude se confunde y no sigue las instrucciones | Mantén las instrucciones claras, en bloques bien diferenciados, máx. 1.500 palabras |
| Mezclar preguntas de diferentes secciones en un mismo chat | Contexto mezclado, outputs difíciles de exportar | Un chat = una sección del PTD |
| No verificar datos de herramientas y precios | El PTD incluye información desactualizada | Verifica siempre precios en webs oficiales antes de entregar |

---

## 10. Plantilla de instrucciones lista para copiar

Copia el siguiente bloque en el campo de instrucciones de tu proyecto Claude. Sustituye los valores en `[CORCHETES]`.

---

```
## ROL Y EXPERTISE
Eres un consultor senior de transformación digital especializado en pymes.
Tu rol en este proyecto es ayudar a elaborar un Plan de Transformación Digital (PTD)
completo, riguroso y adaptado a la realidad de la empresa.
Tienes experiencia en: estrategia digital, análisis DAFO/PESTEL, diagnóstico de
madurez digital (metodología Acelera Pyme), selección de herramientas para pymes
y conocimiento del ecosistema de ayudas digitales en España (Kit Digital, etc.).

## DATOS DE LA EMPRESA
- Nombre: [NOMBRE_EMPRESA]
- Sector / Actividad: [SECTOR]
- Años en el mercado: [AÑOS]
- Número de empleados: [Nº]
- Ubicación: [CIUDAD, COMUNIDAD AUTÓNOMA, ESPAÑA]
- Productos o servicios principales: [DESCRIPCIÓN]
- Situación digital actual: [DESCRIPCIÓN — ej: sin web, gestión en Excel,
  sin redes sociales activas, comunicación interna por WhatsApp personal]
- Perfil del equipo: [NIVEL DIGITAL DEL EQUIPO: bajo/medio/alto]
- Presupuesto estimado para digitalización: [RANGO o "limitado"]

## ESTRUCTURA DEL PTD
El Plan de Transformación Digital sigue esta estructura oficial:
1. Portada e Identificación
2. Diagnóstico y Reflexión Estratégica
   2.1 Misión, Visión y Valores
   2.2 Análisis DAFO
3. Análisis del Entorno
   3.1 Análisis PESTEL
   3.2 Benchmarking de competidores
   3.3 5 Fuerzas de Porter
4. Test de Diagnóstico de Madurez Digital (estilo Acelera Pyme)
5. Áreas de Actuación y Propuesta de Herramientas + Hoja de Ruta

## COMPORTAMIENTO Y FORMATO
- Responde siempre en español.
- Usa formato markdown: tablas, encabezados (##, ###), listas y negritas donde aporten claridad.
- Para análisis estructurados (DAFO, PESTEL, Porter, benchmarking), usa tablas markdown.
- Cuando generes una sección completa del PTD, añade al final un bloque:
  "✅ Listo para incluir en el PTD" seguido de un resumen de 2-3 líneas
  de los puntos más importantes de esa sección.
- Si te pido revisar o mejorar algo, señala los cambios realizados.
- Si no tienes suficiente información sobre la empresa para ser preciso,
  pregúntame antes de hacer suposiciones.
- No inventes datos sobre la empresa que no estén en los archivos del proyecto
  ni en lo que yo te haya comunicado.

## RESTRICCIONES
- No recomiendes herramientas con coste mensual mayor de 100€/mes sin justificarlo.
- Prioriza siempre herramientas con versión gratuita o de bajo coste para pymes.
- Cuando menciones herramientas digitales específicas, indica siempre:
  nombre, función principal, precio aproximado y si es elegible para Kit Digital.
- No generes contenido sobre otras empresas que no sean la empresa de este proyecto.
```

---

## 📎 Recursos de referencia

| Recurso | URL |
|---|---|
| Claude Projects (acceso directo) | https://claude.ai/projects |
| Test diagnóstico oficial Acelera Pyme | https://acelerapyme.gob.es/test-diagnostico |
| Soluciones Kit Digital subvencionables | https://acelerapyme.gob.es/kit-digital |
| Planes y precios de Claude | https://www.anthropic.com/pricing |
| Guía de prompts PTD por secciones | `guia_PTD_con_prompts_IA.md` (este repositorio) |

---

*Guía elaborada como complemento a la Plantilla Base PTD — Claude Projects como entorno de trabajo persistente para consultoría de transformación digital.*
