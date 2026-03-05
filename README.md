# Wine-Analytics-Project

<img width="2816" height="1536" alt="Gemini_Generated_Image_fr6ap4fr6ap4fr6a" src="https://github.com/user-attachments/assets/57d0bd13-4779-4e89-a257-ceda907e496c" />

ML Lab: Predicción de Calidad Vitivinícola
Análisis Exploratorio y Clasificación con Random Forest

Objetivo del Proyecto
Este repositorio contiene un entorno de experimentación desarrollado en Google Colab para explorar el ciclo completo de ciencia de datos: desde la ingesta automatizada mediante la API de Kaggle hasta la implementación de un modelo predictivo para categorizar vinos "Premium".

Hallazgos de Negocio (EDA)
A través del análisis de un dataset de 130k reseñas, se identificaron los siguientes puntos clave:

Segmentación de Valor: Identificación de las variedades más costosas (lideradas por Champagne Blend).

Geografía del Mercado: Análisis del Top 10 de países exportadores y su impacto en el precio promedio.

Procesamiento de Texto: Generación de una Nube de Palabras (Tag Cloud) para sintetizar los descriptores más frecuentes en las críticas especializadas.

Desafíos y Soluciones Técnicas
Sesgo de Variables: Detecté que el modelo inicial dependía excesivamente del precio. Lo solucioné mediante Feature Engineering (One-Hot Encoding) integrando el país y la variedad, subiendo la precisión del 74.7% al 75.5%.

Seguridad (Security by Design): Implementé un flujo de autenticación por tokens temporales para el manejo de la API Key de Kaggle, evitando la exposición de credenciales en el código público.

Tecnologías Utilizadas
Lenguaje: Python (Pandas, Numpy)

Visualización: Matplotlib, Seaborn, WordCloud

Machine Learning: Scikit-Learn (Random Forest Classifier)

Entorno: Google Colab & GitHub Integration
