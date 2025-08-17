# Trabajos Prácticos de Procesamiento de Lenguaje Natural 1 (PLN1)

Este repo contiene las soluciones a una serie de desafíos prácticos del curso de Procesamiento de Lenguaje Natural 1. El proyecto abarca desde tareas de clasificación de texto y creación de embeddings hasta la generación de texto y el desarrollo de un chatbot conversacional.

Cada desafío se encuentra en su propio Jupyter Notebook, donde se detalla el proceso de análisis, preprocesamiento, modelado y evaluación.

## 🚀 Tecnologías Utilizadas

El proyecto fue desarrollado utilizando las siguientes librerías y frameworks:

* **Python 3**
* **TensorFlow / Keras:** Para la construcción de modelos de redes neuronales.
* **Scikit-learn:** Para modelos de clasificación clásicos y métricas de evaluación.
* **Gensim:** Para la creación y análisis de embeddings de palabras (Word2Vec).
* **NLTK:** Para tareas de preprocesamiento de texto como tokenización y lematización.
* **Pandas:** Para la manipulación y análisis de datos.
* **Plotly y Matplotlib/Seaborn:** Para la visualización de datos y resultados.
* **Google Colab:** Como entorno de ejecución principal.

## 📂 Desafíos Resueltos

A continuación se describe cada uno de los trabajos prácticos incluidos en este proyecto:

### [Desafío 1: Clasificación de Texto con Naive Bayes y Similitud TF-IDF](./Desafio1/Jose_Perez_19co_PLN_Desafio_1.ipynb)

* **Objetivo:** Explorar técnicas de vectorización TF-IDF para clasificación de texto y análisis de similitud.
* **Dataset:** `20 Newsgroups`, un corpus clásico con 20 categorías de noticias.
* **Técnicas Clave:**
    * Vectorización de documentos usando **TF-IDF**.
    * Análisis de similitud entre documentos y palabras mediante **similitud de coseno**.
    * Entrenamiento y optimización de modelos de clasificación **Naive Bayes (Multinomial y Complement)**, evaluando diferentes configuraciones de n-gramas y filtrado de frecuencia.

### [Desafío 2: Creación de Embeddings con Gensim (Word2Vec)](./Desafio2/Jose_Perez_19co_PLN_Desafio_2.ipynb)

* **Objetivo:** Entrenar un modelo de embeddings de palabras desde cero utilizando un corpus en español.
* **Dataset:** Noticias de los diarios *La Razón* y *Público* de España.
* **Técnicas Clave:**
    * Preprocesamiento avanzado de texto en español (limpieza, tokenización, lematización).
    * Entrenamiento de un modelo **Word2Vec (Skip-gram)** con Gensim.
    * Evaluación de la calidad de los embeddings mediante pruebas de **similitud de palabras y analogías** (ej. "rey - hombre + mujer = reina").
    * Visualización del espacio vectorial de palabras con **t-SNE**.

### [Desafío 3: Modelo de Lenguaje a Nivel de Caracter con RNNs](./Desafio3/Jose_Perez_19co_PLN_Desafio_3.ipynb)

* **Objetivo:** Construir un modelo de lenguaje generativo a nivel de caracter para crear texto nuevo.
* **Dataset:** El texto completo de la obra *Don Quijote de la Mancha*.
* **Técnicas Clave:**
    * Tokenización a nivel de caracter.
    * Implementación de arquitecturas de **Redes Neuronales Recurrentes (SimpleRNN y LSTM)**.
    * Entrenamiento del modelo para predecir el siguiente caracter en una secuencia.
    * Generación de texto nuevo utilizando diferentes estrategias de decodificación:
        * **Greedy Search**.
        * **Beam Search (Determinista y Estocástico)**, explorando el efecto de la **temperatura** para controlar la creatividad del texto.

### [Desafío 4: Chatbot Conversacional con Seq2Seq y LSTMs](./Desafio4/Jose_Perez_19co_PLN_Desafio_4.ipynb)

* **Objetivo:** Desarrollar un bot conversacional (QA Bot) capaz de generar respuestas a preguntas usando una arquitectura Encoder-Decoder.
* **Dataset:** Corpus de conversaciones en inglés del challenge `ConvAI2`.
* **Técnicas Clave:**
    * Arquitectura **Sequence-to-Sequence (Seq2Seq)** con LSTMs.
    * Modelo **Encoder-Decoder** para mapear secuencias de entrada (preguntas) a secuencias de salida (respuestas).
    * Uso de **embeddings pre-entrenados (FastText)** para mejorar la representación semántica de las palabras.
    * Implementación de un bucle de **inferencia** para generar respuestas a nuevas entradas de texto.

## ⚙️ Cómo Ejecutar el Proyecto

Para explorar los notebooks y ejecutar el código:

### Instalación y Ejecución

1.  **Google Colab**
    Dado que el proyecto fue desarrollado en Colab, la forma más sencilla de ejecutarlo es subir cada archivo `.ipynb` a tu Google Drive, abrirlo con Google Colaboratory y ejecutarlo directamente, aprovechando las GPUs gratuitas.

## 👤 Autor

* **José Pérez** - [joseperez190498@gmail.com](mailto:joseperez190498@gmail.com)
