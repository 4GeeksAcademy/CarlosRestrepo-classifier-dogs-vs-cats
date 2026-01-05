 # 📑 Clasificador de Perros vs Gatos con CNN

Este proyecto implementa una Red Neuronal Convolucional (CNN) optimizada para la clasificación binaria de imágenes, permitiendo distinguir entre perros y gatos con alta precisión mediante aprendizaje profundo.


## 🚀 Funcionalidades

> - clasificación Automatizada: Identifica con precisión si una imagen corresponde a un perro o a un gato.
> - Procesamiento de Dataset: Carga y normalización eficiente de grandes volúmenes de datos visuales.
> - Inferencia de Resultados: Genera una predicción probabilística basada en patrones de pixeles.
> - Evaluación de Rendimiento: Cálculo de métricas de precisión durante el entrenamiento y la validación.


## 📂 Data:

El dataset utilizado puede descargarse desde este [link](https://storage.googleapis.com/datascience-materials/dogs-vs-cats.zip).


## 💻 Tecnologías y herramientas:

**Lenguaje:** Python 3.10.

**Framework:** TensorFlow con DirectML para aceleración por GPU AMD.

**Optimización:** Pipeline de datos optimizado con cache() y prefetch(AUTOTUNE).


## 🔧 Instalación de las dependencias:

pip install -r requirements.txt.


## ⚙️ Pipeline de Datos

Para maximizar el rendimiento y evitar cuellos de botella durante el entrenamiento, se implementó un pipeline de datos optimizado:
* **Resizing & Rescaling:** Normalización de píxeles y ajuste de dimensiones.
* **Caching:** Los datos se mantienen en memoria después de la primera época para acelerar la lectura.
* **Prefetching:** El software prepara los datos del siguiente lote mientras la GPU procesa el actual (AUTOTUNE).


## 📊 Resultados del Modelo:

> - El entrenamiento se realizó durante 10 épocas, logrando buenos resultados.
> - Precisión en Test (Accuracy): 89.72%.
> - Pérdida (Loss): 0.2498.
> - Generalización: El modelo muestra un comportamiento estable sin signos significativos de sobreajuste (overfitting).

**Puedes visualizar [aquí](assets\prediccion.png) la predicción final.**


## Insignias:

![Python](https://img.shields.io/badge/python-3.10-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![Accuracy](https://img.shields.io/badge/Accuracy-89.72%25-green.svg)
![Pipeline](https://img.shields.io/badge/Pipeline-Optimized-brightgreen.svg)
![License](https://img.shields.io/badge/license-MIT-yellow.svg)
![Status](https://img.shields.io/badge/status-completado-brightgreen.svg)


## ⚖️ Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.