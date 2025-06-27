# 🧠📰 Trabajo Práctico Final Integrador - Procesamiento de Lenguaje Natural

Este proyecto es un **notebook de Google Colab** que permite realizar Web Scraping de artículos de noticias argentinas, aplicar técnicas de procesamiento de lenguaje natural (PLN/NLP), y visualizar los resultados a través de una **interfaz interactiva con Gradio**.

---

## 🎯 Objetivo

Analizar y visualizar noticias de actualidad de medios argentinos (*Infobae* y *La Nación*) utilizando herramientas de NLP, IA generativa y visualización de datos.

---

## 🚀 Características Principales

- 📰 **Web Scraping**
  - Extracción automática de títulos y cuerpos de noticias de Infobae y La Nación.

- 🗃️ **Unificación de Datos**
  - Combinación de datos en un único DataFrame.
  - Exportación a archivo `CSV`.

- 🧹 **Procesamiento de Lenguaje Natural**
  - Limpieza y tokenización de texto.
  - Generación de **nubes de palabras (WordCloud)**.
  - Extracción de **Entidades Nombradas (NER)** usando `spaCy` y Gemini.
  - Análisis de **sentimiento** con `TextBlob`.
  - Visualización de distribución general de sentimientos.
  - Generación automática de:
    - 📄 **Resumen del artículo** (usando Gemini API)
    - 🐦 **Tweet/Introducción estilo argentino**

- 🖼️ **Interfaz interactiva con Gradio**
  - Selección de artículo desde un desplegable.
  - Visualización de texto original y procesado.
  - Botones para aplicar funciones como WordCloud, Sentimiento, NER, etc.

---

## 🧪 ¿Cómo usar?

### 1. Abrí el Notebook en Google Colab

### 2. Ejecutá todas las celdas paso a paso
Esto instalará las dependencias, hará scraping, preprocesará los datos y abrirá Gradio.

### 3. Interactuá con la interfaz
Desde el link generado por Gradio podés:

- 🔍 Ver el texto del artículo
- ✨ Limpiar texto (tokenización y normalización)
- ☁️ Generar WordCloud
- 📍 Extraer entidades nombradas (NER)
- 😊 Ver análisis de sentimiento (Positivo/Negativo/Neutro)
- 🧠 Generar resumen con IA
- 🇦🇷 Generar tweet con tono argentino

---

## 🔐 Requisitos

- ✅ Cuenta de Google (para abrir Colab)
- ✅ Clave de API de Google Gemini (guardada como `GOOGLE_API_KEY` en Colab)

---

## 📦 Dependencias (instaladas automáticamente)

```bash
gradio
transformers
sentencepiece
spacy
wordcloud
matplotlib
textblob
requests
beautifulsoup4
pandas
google-generativeai
nltk
