Proyecto Guardia-ML
Clasificación de guardia en boxeo mediante Pose Detection + Deep Learning

Este proyecto implementa un sistema capaz de detectar la guardia de un boxeador en tiempo real usando:
- MediaPipe Pose
- Modelos Dense Neural Network (Keras)
- Procesamiento de video en vivo (OpenCV)
- Dataset propio no incluido por privacidad

Características principales:
- Detección de puntos corporales (pose landmarks)
- Cálculo de ángulos corporales
- Entrenamiento de modelo DNN
- Guardado automático de imágenes/dataset
- Inferencia en tiempo real
- Proyecto limpio sin datos sensibles
- Listo para producción

Estructura del proyecto:
src/ - Código fuente
models/ - Modelos entrenados
data/ - Dataset privado
notebooks/ - Notebooks limpios

Instalación:
git clone https://github.com/tu_usuario/guardia-ml
cd guardia-ml
pip install -r requirements.txt
mkdir data models

Dataset:
Colocar dataset en data/archivo.csv

Entrenar modelo:
python src/train.py

Inferencia:
python src/inference.py

Licencia:
Apache 2.0 © KiiDeku
