# 📰 Proyecto de Preprocesamiento y Tokenización de Noticias

## ✨ **Propósito del Proyecto**

Este proyecto tiene como objetivo el desarrollo de herramientas de preprocesamiento y tokenización para analizar datos de noticias. Al limpiar y transformar los textos, el proyecto permite extraer información relevante y preparar los datos para su posterior uso en tareas de aprendizaje automático, como clasificación y agrupamiento.

## 📚 **Archivos Incluidos**

- **Datos**: Archivos en formato `.xlsx` con noticias a procesar.
- **Cuadernos**: Notebooks de Jupyter para realizar el preprocesamiento, tokenización, y cálculo de representaciones numéricas.

## 🚀 **Instrucciones de Instalación y Ejecución**

### Requisitos

- Python `^3.10`
- Dependencias gestionadas con `poetry` o instaladas manualmente con `pip`.

### Instalación con Poetry

1. Clona el repositorio y navega al directorio del proyecto:
   ```bash
   git clone https://github.com/Jiliar/text-preprocessing-project.git
   cd text-preprocessing-project/
   ```

2. Instala las dependencias:
   ```bash
   poetry install
   ```

3. Activa el entorno y ejecuta Jupyter Notebook:
   ```bash
   poetry shell
   jupyter notebook
   ```

### Instalación con pip

Si prefieres no usar Poetry, puedes instalar las dependencias manualmente:

```bash
pip install pandas numpy scikit-learn nltk gensim scipy openpyxl
```

### Configuración Adicional para NLTK

Descarga los recursos necesarios de NLTK ejecutando el siguiente código:

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

## 📆 **Actividades Principales**

### 1. **Preprocesamiento del Texto**

- Convertir el texto a minúsculas.
- Eliminar puntuación, números y espacios en blanco adicionales.

### 2. **Tokenización**

- Dividir el texto en palabras individuales utilizando NLTK.

### 3. **Eliminación de Stop Words**

- Excluir palabras irrelevantes para el análisis semántico, como "el", "la" o "de".

### 4. **Cálculo de TF-IDF**

- Convertir el texto en representaciones vectoriales numéricas basadas en la frecuencia y relevancia de las palabras en el corpus.

### 5. **Generación de Embeddings con Word2Vec**

- Crear representaciones densas que capturan el significado semántico de las palabras.

## 📄 **Dependencias**

```toml
[tool.poetry.dependencies]
python = "^
