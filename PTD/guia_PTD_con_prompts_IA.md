# 🚀 Guía para Generar Planes de Transformación Digital (PTD) con IA

> Guía práctica con prompts de inteligencia artificial para elaborar un Plan de Transformación Digital completo, sección por sección, adaptado a cualquier empresa o caso particular.

---

## 📋 Índice

1. [Cómo usar esta guía](#cómo-usar-esta-guía)
2. [Sección 1 – Portada e Identificación](#sección-1--portada-e-identificación)
3. [Sección 2 – Diagnóstico y Reflexión Estratégica](#sección-2--diagnóstico-y-reflexión-estratégica)
4. [Sección 3 – Análisis del Entorno (PESTEL + Porter + Benchmarking)](#sección-3--análisis-del-entorno)
5. [Sección 4 – Test de Diagnóstico Digital (Madurez Digital)](#sección-4--test-de-diagnóstico-digital)
6. [Sección 5 – Áreas de Actuación y Propuesta de Herramientas](#sección-5--áreas-de-actuación-y-propuesta-de-herramientas)
7. [Prompt maestro: PTD completo en una sola llamada](#prompt-maestro-ptd-completo-en-una-sola-llamada)
8. [Consejos generales de uso](#consejos-generales-de-uso)

---

## Cómo usar esta guía

Esta guía proporciona **prompts listos para copiar y pegar** en cualquier asistente de IA (Claude, ChatGPT, Gemini, etc.). Para cada sección del PTD encontrarás:

- 📌 **Qué debe contener** esa sección según la plantilla oficial.
- 🤖 **Prompt base** para generarla (personalizable).
- 🔧 **Variables a sustituir** marcadas con `[CORCHETES]`.
- 💡 **Consejo de uso** para obtener mejores resultados.

**Flujo de trabajo recomendado:**

```
1. Reúne información básica de la empresa (sector, tamaño, servicios, situación actual)
2. Ejecuta los prompts en orden, sección por sección
3. Revisa y valida cada output con el equipo o el cliente
4. Integra todo en el documento final
```

---

## Sección 1 – Portada e Identificación

### 📌 Qué incluye
- Título del proyecto
- Equipo de trabajo (miembros, edades, formación)
- Responsable del proyecto y contacto

### 🤖 Prompt

```
Actúa como consultor de transformación digital. Genera la portada e identificación 
de un Plan de Transformación Digital para la siguiente empresa:

- Nombre de la empresa: [NOMBRE_EMPRESA]
- Sector / Actividad: [SECTOR]
- Número de empleados: [Nº EMPLEADOS]
- Ubicación: [CIUDAD, PAÍS]
- Equipo que elabora el plan:
    [NOMBRE 1], [EDAD], [FORMACIÓN]
    [NOMBRE 2], [EDAD], [FORMACIÓN]
    ...
- Responsable del proyecto: [NOMBRE], [EMAIL]

Estructura la portada con: título formal del documento, subtítulo descriptivo, 
tabla del equipo de trabajo y datos de contacto. Usa un tono profesional y formal.
```

### 💡 Consejo
Si el equipo es ficticio (práctica académica), pide a la IA que también proponga nombres y perfiles coherentes con el sector añadiendo: *"El equipo es simulado; propón perfiles realistas para el sector."*

---

## Sección 2 – Diagnóstico y Reflexión Estratégica

### 📌 Qué incluye
- **Identidad Corporativa**: Misión, Visión, Valores
- **Análisis DAFO**: Fortalezas, Debilidades, Oportunidades, Amenazas

---

### 2a – Identidad Corporativa (Misión, Visión, Valores)

#### 🤖 Prompt

```
Actúa como consultor estratégico especializado en pymes. Define la identidad 
corporativa de la siguiente empresa para su Plan de Transformación Digital:

- Empresa: [NOMBRE_EMPRESA]
- Sector: [SECTOR]
- Productos o servicios principales: [DESCRIPCIÓN BREVE]
- Antigüedad en el mercado: [AÑOS]
- Modelo de negocio: [B2B / B2C / mixto]
- Valores o cultura que ya practican (si los conoces): [OPCIONAL]

Genera:
1. MISIÓN: propuesta de valor actual, a quién sirven y cómo (2-3 frases).
2. VISIÓN: dónde quiere estar la empresa a 3-5 años, enfocada en transformación 
   digital (2-3 frases).
3. VALORES: lista de 5-6 valores éticos y operativos relevantes para el sector, 
   con una línea de explicación para cada uno.

Formato: secciones claras con encabezados, lenguaje corporativo pero accesible.
```

---

### 2b – Análisis DAFO

#### 🤖 Prompt

```
Actúa como consultor de estrategia digital. Elabora un análisis DAFO completo 
para el siguiente caso:

- Empresa: [NOMBRE_EMPRESA]
- Sector: [SECTOR]
- Tamaño: [Nº EMPLEADOS] empleados, [FACTURACIÓN APROX. o "pequeña/mediana empresa"]
- Situación digital actual: [descripción breve, ej: "sin presencia online, 
  gestión en papel, sin software de gestión"]
- Contexto de mercado: [ej: "mercado local muy competido, clientes mayoritariamente 
  de 40-60 años, tendencia creciente a la compra online en el sector"]

Genera las 4 dimensiones del DAFO con 4-6 ítems cada una:
- FORTALEZAS: capacidades internas y ventajas competitivas.
- DEBILIDADES: puntos críticos internos que frenan la digitalización.
- OPORTUNIDADES: factores externos favorables para digitalizar.
- AMENAZAS: riesgos externos que podrían perjudicar a la empresa.

Presenta el resultado en formato de tabla markdown con dos columnas 
(Factores Internos / Factores Externos) y cuatro cuadrantes.
```

### 💡 Consejo
Para resultados más precisos, comparte con la IA cualquier dato real disponible: entrevistas al propietario, reseñas en Google, página web actual o catálogo de productos.

---

## Sección 3 – Análisis del Entorno

### 📌 Qué incluye
- **Análisis PESTEL** (Político, Económico, Sociocultural, Tecnológico, Ecológico, Legal)
- **Benchmarking** de competidores innovadores
- **5 Fuerzas de Porter**

---

### 3a – Análisis PESTEL

#### 🤖 Prompt

```
Actúa como analista de entorno empresarial. Realiza un análisis PESTEL orientado 
a la transformación digital para:

- Sector: [SECTOR]
- País / Región: [PAÍS o COMUNIDAD AUTÓNOMA]
- Año de referencia: [AÑO ACTUAL]

Para cada dimensión, incluye 3-4 factores clave con su impacto potencial en 
la digitalización de una pyme del sector:

P – Político/Legal: normativas, ayudas (ej: Kit Digital), regulación de datos (RGPD).
E – Económico: ciclos de mercado, inflación, acceso a financiación y subvenciones.
S – Sociocultural: hábitos del consumidor, brecha digital, tendencias generacionales.
T – Tecnológico: adopción de IA, cloud, IoT, infraestructura de conectividad.
E – Ecológico: sostenibilidad digital, huella de carbono tecnológica, ecodiseño.
L – Legal: protección de datos, facturación electrónica obligatoria, ciberseguridad.

Formato: tabla markdown con columnas: Dimensión | Factor | Descripción | 
Impacto (Alto/Medio/Bajo).
```

---

### 3b – Benchmarking de Competidores

#### 🤖 Prompt

```
Actúa como analista de inteligencia competitiva digital. Realiza un benchmarking 
de 3-5 empresas innovadoras del siguiente sector:

- Sector: [SECTOR]
- Tipo de empresa objetivo: [ej: "tienda local de alimentación ecológica", 
  "taller mecánico familiar", "clínica dental independiente"]
- País o mercado de referencia: [PAÍS]

Para cada competidor o referente analizado, incluye:
1. Nombre de la empresa
2. Modelo de negocio (en 1-2 frases)
3. Estrategia digital: presencia web, redes sociales activas, SEO/SEM, 
   e-commerce, app propia
4. Innovaciones digitales destacadas
5. Catálogo de productos/servicios principales
6. Lección aprendida para la empresa objetivo

Presenta el resultado en una tabla markdown comparativa.
Finaliza con un párrafo de conclusiones: qué tendencias dominan en el sector 
y qué debería priorizar la empresa para ser competitiva.
```

---

### 3c – Las 5 Fuerzas de Porter

#### 🤖 Prompt

```
Actúa como consultor de estrategia empresarial. Aplica el modelo de las 5 Fuerzas 
de Porter al siguiente caso, enfocándote en el impacto sobre la estrategia digital:

- Empresa: [NOMBRE_EMPRESA]
- Sector: [SECTOR]
- Mercado: [LOCAL / REGIONAL / NACIONAL]

Para cada fuerza, evalúa:
- Descripción de la fuerza en el contexto del sector
- Intensidad actual: Alta / Media / Baja (con justificación breve)
- Implicación para la transformación digital de la empresa

Las 5 fuerzas a analizar:
1. Rivalidad entre competidores existentes
2. Amenaza de nuevos entrantes
3. Amenaza de productos o servicios sustitutos
4. Poder de negociación de los clientes
5. Poder de negociación de los proveedores

Formato: tabla markdown + párrafo final de síntesis estratégica.
```

### 💡 Consejo
Para el benchmarking, si la IA no conoce empresas reales del sector concreto, pídele que use empresas de referencia en el sector a nivel europeo o que proponga perfiles tipo realistas.

---

## Sección 4 – Test de Diagnóstico Digital

### 📌 Qué incluye
- **Índice de Intensidad Digital** (nivel de madurez: Muy Bajo → Muy Alto)
- **Desglose por áreas operativas** con porcentaje:
  - Estrategia y Organización
  - Infraestructura y Tecnología
  - Ciberseguridad
  - Relación con Clientes
  - Procesos de Negocio

---

### 🤖 Prompt

```
Actúa como auditor de madurez digital especializado en pymes. Simula la aplicación 
del test de diagnóstico digital "Acelera Pyme" para la siguiente empresa:

- Empresa: [NOMBRE_EMPRESA]
- Sector: [SECTOR]
- Situación tecnológica actual:
    * Dispositivos: [ej: "2 ordenadores de sobremesa, sin tablets ni móviles 
      corporativos"]
    * Software de gestión: [ej: "Excel para contabilidad, sin ERP ni CRM"]
    * Presencia online: [ej: "sin web, perfil de Facebook desactualizado"]
    * Ciberseguridad: [ej: "antivirus básico, sin política de contraseñas"]
    * Comunicación interna: [ej: "WhatsApp personal, sin herramientas corporativas"]
    * Marketing digital: [ej: "ninguno activo"]

Genera:
1. Índice de Intensidad Digital global (escala: Muy Bajo / Bajo / Medio / 
   Alto / Muy Alto) con puntuación estimada sobre 100.
2. Desglose por áreas con puntuación porcentual (0-100%) y calificación cualitativa:
   - Estrategia y Organización
   - Infraestructura y Tecnología
   - Ciberseguridad
   - Relación con Clientes (CRM, redes sociales, marketing)
   - Procesos de Negocio (automatización, herramientas internas)
3. Representación visual del "termómetro digital" usando texto/ASCII.
4. Principales brechas detectadas (top 3).

Formato: tabla markdown para el desglose + texto explicativo por sección.
```

### 💡 Consejo
Si tienes acceso a resultados reales del test [Acelera Pyme](https://acelerapyme.gob.es/test-diagnostico), pégalos directamente en el prompt para que la IA los interprete y elabore el análisis en lugar de simularlo.

---

## Sección 5 – Áreas de Actuación y Propuesta de Herramientas

### 📌 Qué incluye
- Áreas prioritarias de intervención
- Propuesta concreta de herramientas o tecnologías para cerrar brechas

---

### 🤖 Prompt

```
Actúa como consultor tecnológico especializado en transformación digital de pymes. 
Basándote en el diagnóstico siguiente, define las áreas de actuación prioritarias 
y propón un plan de herramientas digitales:

DIAGNÓSTICO PREVIO (resumido):
- Empresa: [NOMBRE_EMPRESA], sector [SECTOR]
- Brechas principales detectadas: [lista las brechas del análisis anterior, ej:
    * Sin presencia web ni e-commerce
    * Gestión administrativa completamente manual
    * Sin estrategia de captación de clientes digitales
    * Ciberseguridad inexistente
    * Comunicación interna desorganizada]
- Presupuesto aproximado disponible: [ej: "limitado (<5.000€/año)", "medio 
  (5.000-20.000€/año)", "sin restricción definida"]
- Nivel de capacitación digital del equipo: [Bajo / Medio / Alto]

Genera:
1. ÁREAS PRIORITARIAS DE ACTUACIÓN (ordenadas por urgencia):
   Para cada área: nombre, justificación, impacto esperado (Alto/Medio/Bajo).

2. PROPUESTA DE HERRAMIENTAS DIGITALES:
   Para cada área prioritaria, recomienda 2-3 herramientas específicas indicando:
   - Nombre de la herramienta
   - Función principal
   - Plan/versión recomendada y coste estimado (mensual o anual)
   - Dificultad de implementación (Fácil / Media / Avanzada)
   - Compatibilidad con ayudas tipo "Kit Digital" (Sí / No / Posible)

3. HOJA DE RUTA SUGERIDA:
   Cronograma simplificado en 3 fases (0-3 meses / 3-9 meses / 9-18 meses) 
   con las acciones clave de cada fase.

Formato: tablas markdown + texto explicativo. Prioriza herramientas con versión 
gratuita o de bajo coste para pymes.
```

### 💡 Consejo
Añade al prompt la frase *"Ten en cuenta las ayudas del programa Kit Digital vigentes en España"* si el caso es español, para que la IA alinee sus recomendaciones con las soluciones subvencionables.

---

## Prompt maestro: PTD completo en una sola llamada

> ⚠️ **Úsalo con precaución**: genera un documento extenso de una vez. Recomendado solo si tienes contexto suficiente sobre la empresa. Para mayor calidad, usa los prompts individuales por sección.

```
Actúa como consultor senior de transformación digital. Genera un Plan de 
Transformación Digital (PTD) completo y estructurado para la siguiente empresa:

===== DATOS DE LA EMPRESA =====
- Nombre: [NOMBRE_EMPRESA]
- Sector / Actividad: [SECTOR]
- Años en el mercado: [AÑOS]
- Nº de empleados: [Nº]
- Facturación aproximada: [RANGO o "no disponible"]
- Ubicación: [CIUDAD, PAÍS]
- Productos/servicios principales: [DESCRIPCIÓN]
- Situación digital actual: [DESCRIPCIÓN DETALLADA]
- Presupuesto para digitalización: [RANGO o "limitado"]

===== ESTRUCTURA REQUERIDA =====

Genera el PTD con las siguientes secciones, en formato markdown:

## 1. PORTADA E IDENTIFICACIÓN
   Título formal, equipo ficticio con perfiles coherentes al sector, 
   responsable y contacto.

## 2. DIAGNÓSTICO Y REFLEXIÓN ESTRATÉGICA
   2.1 Misión, Visión y Valores corporativos
   2.2 Análisis DAFO (tabla de 4 cuadrantes con 5 ítems cada uno)

## 3. ANÁLISIS DEL ENTORNO
   3.1 Análisis PESTEL (tabla con 6 dimensiones, 3 factores cada una, 
       orientado a digitalización)
   3.2 Benchmarking (tabla con 3 competidores/referentes del sector)
   3.3 5 Fuerzas de Porter (tabla con intensidad y síntesis estratégica)

## 4. DIAGNÓSTICO DE MADUREZ DIGITAL
   Índice de Intensidad Digital global + desglose por 5 áreas operativas 
   (con puntuación % y brechas detectadas)

## 5. ÁREAS DE ACTUACIÓN Y PROPUESTA DE HERRAMIENTAS
   Áreas prioritarias + propuesta de herramientas específicas + 
   hoja de ruta en 3 fases (0-3, 3-9, 9-18 meses)

===== REQUISITOS DE FORMATO =====
- Todo el documento en markdown válido (tablas, encabezados, listas)
- Lenguaje profesional, concreto y orientado a la acción
- Herramientas reales y accesibles para pymes (con costes aproximados)
- Extensión estimada: documento completo y detallado
```

---

## Consejos generales de uso

### ✅ Para obtener mejores resultados

| Recomendación | Por qué importa |
|---|---|
| Proporciona datos reales de la empresa | La IA mejora radicalmente con contexto concreto |
| Ejecuta los prompts en orden | Cada sección alimenta a la siguiente |
| Revisa y ajusta cada output | La IA puede cometer errores factuales sobre herramientas o precios |
| Pide variantes si no convence | Añade "genera una versión alternativa más conservadora/más ambiciosa" |
| Usa un hilo de conversación único | Mantener contexto entre secciones mejora la coherencia |

### 🔁 Iteración y refinamiento

Si un output no es satisfactorio, usa estos prompts de mejora:

```
# Para pedir más detalle:
"Amplía el apartado de [SECCIÓN] con más ejemplos específicos para el sector [SECTOR]."

# Para ajustar el tono:
"Reescribe la sección [X] con un lenguaje más técnico / más accesible para 
un empresario sin formación digital."

# Para validar coherencia:
"Revisa si las herramientas propuestas en la Sección 5 son coherentes con 
las brechas detectadas en la Sección 4. Ajusta si es necesario."

# Para añadir métricas:
"Añade KPIs e indicadores de éxito medibles para cada área de actuación 
de la Sección 5."
```

### ⚠️ Limitaciones a tener en cuenta

- Los **precios de herramientas** cambian frecuentemente. Verifica siempre en la web oficial.
- La IA puede **alucinar nombres de empresas** en el benchmarking. Contrasta con búsquedas reales.
- El **test Acelera Pyme** simulado es una estimación; para un diagnóstico oficial usa la [plataforma oficial](https://acelerapyme.gob.es).
- Las **ayudas Kit Digital** tienen convocatorias con fechas límite. Consulta el BOE y la web de Red.es para vigencia actual.

---

## 📚 Recursos adicionales

| Recurso | URL |
|---|---|
| Test oficial Diagnóstico Digital (Acelera Pyme) | https://acelerapyme.gob.es/test-diagnostico |
| Programa Kit Digital (España) | https://www.acelerapyme.gob.es/kit-digital |
| Plantilla PTD base (este documento) | `PTD_01_plantilla.pdf` |
| Generador de análisis PESTEL online | https://pestleanalysis.com |

---

*Guía elaborada a partir de la Plantilla Base PTD — adaptable a cualquier sector y tamaño de empresa.*
