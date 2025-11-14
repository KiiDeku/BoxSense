🥊 Proyecto Guardia-ML

Clasificación de guardia en boxeo mediante Pose Detection + Deep Learning

Este proyecto implementa un sistema capaz de detectar la guardia de un boxeador en tiempo real usando:

MediaPipe Pose

Modelos Dense Neural Network (Keras)

Procesamiento de video en vivo (OpenCV)

Dataset propio no incluido por privacidad

El objetivo es permitir entrenar modelos basados en posturas corporales y utilizarlos en tiempo real para clasificar la posición del usuario.

🚀 Características principales

✔ Detección de puntos corporales (pose landmarks)
✔ Cálculo de ángulos corporales
✔ Entrenamiento de modelo DNN
✔ Guardado automático de imágenes/dataset
✔ Inferencia en tiempo real
✔ Proyecto limpio sin datos sensibles
✔ Listo para producción

📂 Estructura del proyecto
src/
  train.py       # Entrenar modelo
  inference.py   # Inferencia en tiempo real (webcam)
  utils.py       # Carga, escalado, funciones
  angles.py      # Cálculo de ángulos con 3 puntos

models/          # Modelos entrenados (vacío)
data/            # Dataset privado (vacío)
notebooks/       # Notebooks limpios
requirements.txt # Dependencias
LICENSE          # Apache 2.0

🔧 Instalación

Clona el repositorio:

git clone https://github.com/tu_usuario/guardia-ml
cd guardia-ml


Instala dependencias:

pip install -r requirements.txt


Crea las carpetas necesarias:

mkdir data models

📥 Dataset (Privado)

Por privacidad, el dataset NO está incluido.

Debe colocarse en:

/data/tu_archivo.csv


Formato esperado:

feature1	feature2	...	label
🧠 Entrenar el modelo
python src/train.py


El modelo entrenado se guardará automáticamente en:

models/modelo_guardia.keras


Y el scaler en:

models/scaler_guardia.joblib

🎥 Inferencia en tiempo real

Con la webcam:

python src/inference.py


Esto mostrará:

Tu pose detectada

Tu guardia predicha

Precisión del modelo

Cantidad de frames procesados

📝 Licencia

Este proyecto está bajo la Apache License 2.0, permitiendo uso libre con atribución.
