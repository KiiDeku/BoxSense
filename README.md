# 🥊 Guardia-ML: Clasificación de Guardia en Boxeo

> **🤖 Clasifica la guardia de un boxeador en tiempo real usando Pose Detection y Deep Learning**

---

## ✨ ¿Qué es Guardia-ML?
Un sistema capaz de **detectar la guardia** de un boxeador en vivo a partir de su postura corporal, combinando lo mejor de la visión computacional y el aprendizaje profundo.

---

## 🏗️ Tecnologías
- 🎯 **[MediaPipe Pose](https://google.github.io/mediapipe/solutions/pose.html)**  
  Detección avanzada de puntos corporales (*pose landmarks*)
- 🧠 **Deep Neural Networks (Keras)**  
  Redes neuronales para clasificar la guardia
- 🎥 **Procesamiento de video en vivo (OpenCV)**
- 📁 **Dataset propio (privado por privacidad)**

---

## 🚀 Características principales

| Función                       | Descripción                                |
|-------------------------------|--------------------------------------------|
| 📍 Detección de pose          | Ubicación precisa de puntos corporales     |
| 📐 Cálculo de ángulos         | Ángulos automáticos entre puntos clave     |
| 🏋️ Entrenamiento personalizado| Ajusta el modelo a tus propios datos       |
| 🗂️ Guardado automático        | Imágenes + datasets en disco               |
| ⚡ Inferencia en tiempo real   | Clasificación instantánea con webcam       |
| 🔒 Sin datos sensibles        | Proyecto limpio y modular                  |
| 🚢 Listo para producción      | ¡Usa, prueba, expande!                     |

---

## 🗂️ Estructura del proyecto

```
📦 guardia-ml/
│
├─ src/
│    ├─ train.py       # 🏋️ Entrenamiento del modelo
│    ├─ inference.py   # ⚡ Inferencia en tiempo real (webcam)
│    ├─ utils.py       # 🛠️ Utilidades y escalado de datos
│    └─ angles.py      # 📐 Cálculo de ángulos
│
├─ models/             # 📦 Modelos entrenados (vacío)
├─ data/               # 📊 Dataset privado (vacío)
├─ notebooks/          # 📓 Notebooks limpios
├─ requirements.txt    # 📜 Dependencias del proyecto
└─ LICENSE             # 📄 Licencia Apache 2.0
```

---

## 🔧 Instalación

1. **Clona el repositorio:**  
   ```bash
   git clone https://github.com/tu_usuario/guardia-ml
   cd guardia-ml
   ```

2. **Instala las dependencias:**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Crea las carpetas necesarias:**  
   ```bash
   mkdir data models
   ```

---

## 📥 Dataset (Privado)

🚫 **Por privacidad, el dataset NO está incluido.**

Debes colocar tu dataset en la ruta:

```
data/tu_archivo.csv
```

**Formato esperado:**
```
feature1,feature2,...,label
(valores separados por comas o tabulaciones)
```

---

## 🧠 Entrenamiento del modelo

Entrena tu propio modelo con:

```bash
python src/train.py
```

Se guardan automáticamente:
- 🤖 Modelo: `models/modelo_guardia.keras`
- 🧮 Escalador: `models/scaler_guardia.joblib`

---

## 🎥 Inferencia en tiempo real

¡Usa tu webcam para clasificar tu guardia!

```bash
python src/inference.py
```

Verás en pantalla:
- 🕴️ Tu pose detectada
- 🥊 Tu guardia predicha
- 📊 Precisión del modelo
- 🖼️ Frames procesados por segundo

---

## ⚖️ Licencia

Este proyecto está bajo la [Apache License 2.0](LICENSE).  
¡Uso libre, siempre con atribución! 🚀

---

> _Disfruta clasificando guardias y lleva tu entrenamiento de boxeo al siguiente nivel._  
> _¡Contribuciones, ideas y mejoras siempre son bienvenidas!_ 🥇🥊✨
