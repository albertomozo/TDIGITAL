# ⚡ Hoja de Trucos: Automatiza tu Calendario con IA

Esta guía contiene los "comandos" (prompts) y pasos exactos para convertir un PDF estático en un calendario inteligente.

## 1. El Prompt "Mágico" para la IA

Copia y pega este texto en tu chat de IA (Gemini, ChatGPT, etc.) junto con el archivo PDF del calendario:

```
Actúa como un experto en gestión de datos. Lee este calendario en PDF y extrae exclusivamente las sesiones de los Módulos [X e Y]. Genera una tabla con estas columnas exactas: **Subject, Start Date, Start Time, End Date, End Time, Description**. Asegúrate de que las fechas tengan el formato DD/MM/AAAA y que las horas incluyan AM/PM. Una vez hecha la tabla, genera el código en formato CSV para que pueda copiarlo.
```

---

## 2. Formato del Archivo (El "Traductor")

Para que Google o Outlook entiendan tus datos, el archivo debe verse así. **Copia el código generado por la IA, pégalo en el Bloc de Notas y guárdalo como `micurso.csv**`:

| Campo | ¿Qué significa? | Ejemplo |
| --- | --- | --- |
| **Subject** | Nombre de la clase | M1: Estrategia Digital |
| **Start Date** | Fecha de inicio | 29/01/2026 |
| **Start Time** | Hora que empieza | 09:00 AM |
| **Description** | Temario o link Zoom | Módulo 1 - Pág 7-15 |

---

## 3. Guía Rápida de Importación (Clic a Clic)

### Para Google Calendar:

1. **Entra** en [calendar.google.com](https://calendar.google.com).
2. **Rueda dentada** ⚙️ (arriba a la derecha) → **Configuración**.
3. Menú izquierdo → **Importar y exportar**.
4. **Selecciona tu archivo** `micurso.csv`.
5. Pulsa **Importar**.

### Para Notion:

1. Crea una **Nueva Página**.
2. Haz clic en **Importar** (en el menú de la página).
3. Selecciona **CSV**.
4. Arrastra tu archivo.
5. Cambia la vista de "Table" a **"Calendar"**.

---

## 💡 Pro-Tip de Eficiencia

Si el horario tiene un descanso (ej. 11:00 a 11:30 ), no crees dos eventos. Crea uno solo de **09:00 a 14:00** y pon en la **Description**: *"Descanso de 11:00 a 11:30"*. ¡Ahorrarás espacio visual en tu agenda!

---

