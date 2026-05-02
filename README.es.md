🛡️ Sistema de Detección de URLs Spam con SVM
Este proyecto utiliza técnicas de Procesamiento de Lenguaje Natural (NLP) y Machine Learning para clasificar automáticamente si una dirección web (URL) es segura o contiene spam.

📊 Resultados del Proyecto
Tras un proceso de optimización, el modelo alcanzó un rendimiento sobresaliente:

Accuracy (Precisión) Final: ~97.48%.  

Mejores Parámetros (GridSearchCV):

C: 10.  

kernel: 'rbf'.  

gamma: 0.1.

🛠️ Tecnologías UtilizadasLenguaje: Python.  
Librerías principales:Pandas para manipulación de datos. 
Scikit-Learn para el modelo SVM y vectorización TF-IDF.  NLTK para lematización y eliminación de stopwords.  Regex para limpieza de texto.  

🚀 Pasos del ProyectoLimpieza de Datos:
Eliminación de duplicados y transformación de etiquetas categóricas a numéricas.  Preprocesamiento NLP: Limpieza de URLs con expresiones regulares, tokenización, eliminación de palabras vacías (stopwords) y lematización para obtener la raíz de las palabras.  Vectorización: Uso de TfidfVectorizer para convertir el texto en una matriz numérica procesable por el modelo.  Modelado: Implementación inicial de una Máquina de Vectores de Soporte (SVM) con kernel lineal.  

📦 Instalación y Uso
Para replicar este proyecto, instala las dependencias necesarias:
pip install -r requirements.txt

Para cargar el modelo entrenado (.sav):

import pickle
model = pickle.load(open('models/svm_url_spam_model_optimized.sav', 'rb'))







