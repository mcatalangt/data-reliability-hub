# IA Google Componets

Esta sección centraliza plantillas de IA (Machine Learning, Deep Learning , Generative IA)

## Arquitectura
El código está modularizado para permitir la reutilización en diferentes entornos (Dev, Staging, Prod) en Cloud y On-Prem.

!!! info "Stack Tecnológico"
    * **LlamaIndex:** Es un framework en Python (y JS) que sirve para conectar modelos de lenguaje (LLMs) como GPT con tus propios datos (PDFs, bases de datos, APIs, logs, etc.)
      
        ###¿Para qué sirve?

        Leer y cargar datos (PDF, CSV, SQL, JSON, APIs, etc.)
        Dividirlos en fragmentos (chunks)
        Convertirlos en embeddings
        Consultarlos de forma inteligente usando un LLM

        En pocas palabras:
        👉 LlamaIndex se encarga de preparar, organizar y consultar tus datos usando IA.


    * **Qdrant:**  Es una base de datos vectorial. Está diseñada para guardar y buscar embeddings (vectores numéricos que representan significado).

        ¿Para qué sirve?

        Almacenar embeddings de textos, imágenes, audio, etc.

        Buscar información por similitud semántica, no por palabras exactas

        Escalar búsquedas rápidas en millones de vectores

        En pocas palabras:
        👉 Qdrant es donde se guardan y se buscan los vectores.