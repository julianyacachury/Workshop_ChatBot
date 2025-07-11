# Visualización y análisis de emails exportados desde Outlook

Este notebook de Google Colab permite analizar y visualizar información contenida en correos electrónicos exportados desde Outlook. Utiliza archivos `.eml` como fuente de datos y extrae campos relevantes como remitente, asunto, fecha y contenido, con el objetivo de facilitar el análisis exploratorio de emails.

## 📁 Estructura esperada

El Colab trabaja con una carpeta que contenga archivos `.eml` previamente exportados. Se espera una estructura como:

/content/
└── carpeta_emails/
├── email1.eml
├── email2.eml
└── ...

## 🚀 Funcionalidades principales

- 📥 Carga y parseo de archivos `.eml`
- 🧠 Extracción de metadatos: `From`, `Subject`, `Date`, etc.
- 🧹 Limpieza y preprocesamiento de texto
- 📊 Visualización de:
  - Frecuencia de correos por día
  - Palabras más frecuentes por remitente
  - Evolución temporal de términos clave
- 🧪 Búsqueda e inspección de emails según criterios personalizados

## 🧰 Librerías utilizadas

- `pandas`
- `matplotlib`
- `seaborn`
- `email` (librería estándar de Python)
- `datetime`
- `os`
- `re`

## 🛠 Cómo usar

1. Montá tu Google Drive si tenés los `.eml` ahí.
2. Ajustá la variable `ruta` al directorio donde están tus archivos `.eml`.
3. Ejecutá cada celda del notebook paso a paso.
4. Explorá los resultados visuales y los DataFrames generados.

## 📌 Notas

- El parser puede fallar si los `.eml` no siguen el formato estándar RFC822.
- Para datasets grandes, puede demorar el procesamiento de los archivos.

---

✍️ _Notebook desarrollado para facilitar auditorías, análisis de patrones de comunicación o monitoreo de actividad en cuentas de correo._

