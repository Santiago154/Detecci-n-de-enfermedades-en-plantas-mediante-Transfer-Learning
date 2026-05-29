# Detección de Enfermedades en Hojas mediante Transfer Learning

Proyecto desarrollado como parte de la asignatura de Aprendizaje de Máquinas, enfocado en la clasificación automática de enfermedades vegetales a partir de imágenes de hojas utilizando técnicas de Deep Learning y Transfer Learning.

## Descripción

La detección temprana de enfermedades en cultivos es un factor clave para reducir pérdidas agrícolas y mejorar la productividad. Tradicionalmente, este proceso depende de inspecciones visuales realizadas por especialistas, lo que puede resultar costoso y difícil de escalar.

Este proyecto implementa una solución basada en Visión por Computador utilizando la arquitectura **EfficientNetB0** preentrenada sobre **ImageNet**, con el objetivo de identificar diferentes enfermedades presentes en hojas de cultivos.

## Objetivos

- Implementar un modelo de clasificación de imágenes mediante Transfer Learning.
- Evaluar la capacidad de EfficientNetB0 para reconocer enfermedades vegetales.
- Comparar el desempeño de un modelo preentrenado frente a una CNN construida desde cero.
- Analizar métricas de rendimiento mediante matrices de confusión y reportes de clasificación.

## Dataset

Se utilizó el conjunto de datos **PlantVillage**, disponible públicamente en Kaggle.

**Fuente:**
https://www.kaggle.com/datasets/emmarex/plantdisease

Debido a limitaciones de tiempo de entrenamiento y recursos computacionales, se trabajó con una versión reducida del dataset.

### Clases utilizadas

1. Pepper Bell Bacterial Spot
2. Pepper Bell Healthy
3. Potato Early Blight
4. Potato Healthy
5. Potato Late Blight
6. Tomato Bacterial Spot
7. Tomato Early Blight
8. Tomato Healthy
9. Tomato Late Blight

## Tecnologías Utilizadas

- Python
- TensorFlow
- Keras
- EfficientNetB0
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Google Colab

## Arquitectura Principal

### Transfer Learning

Se empleó la arquitectura **EfficientNetB0** con pesos preentrenados en ImageNet.

Características:

- Capas convolucionales congeladas durante la fase inicial.
- Capa de clasificación personalizada.
- Data Augmentation.
- Early Stopping.
- Reduce Learning Rate on Plateau.

## Metodología

1. Carga y preparación del dataset.
2. División en entrenamiento y validación.
3. Aplicación de técnicas de aumento de datos.
4. Entrenamiento mediante Transfer Learning.
5. Evaluación del modelo.
6. Generación de métricas y matrices de confusión.
7. Predicción sobre imágenes externas.

## Resultados

Durante el entrenamiento se analizaron:

- Accuracy de entrenamiento y validación.
- Loss de entrenamiento y validación.
- Matriz de confusión.
- Precision, Recall y F1-Score por clase.

Los resultados evidencian que el uso de Transfer Learning permite obtener un alto desempeño utilizando menos datos y menos tiempo de entrenamiento en comparación con modelos entrenados desde cero.

## Estructura del Proyecto
