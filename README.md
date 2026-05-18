
# 💎 Clasificación de Gemas: CNN vs Transfer Learning (VGG16)

![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) 

Este proyecto desarrolla un sistema de clasificación profunda para identificar **87 tipos de gemas** utilizando el dataset de Kaggle (https://www.kaggle.com/datasets/lsind18/gemstones-images). Comparamos una arquitectura CNN básica construida desde cero contra un modelo avanzado basado en **VGG16** con Fine-Tuning.

## Aspectos Destacados del Proyecto

*   **Arquitecturas:** Baseline CNN (Simple) vs. VGG16 (Transfer Learning).
*   **Optimización:** Uso de `CosineDecay` para el learning rate y `Mixed Precision` para acelerar el entrenamiento en GPU.
*   **Manejo de Desequilibrio:** Implementación de `Class Weights` para mejorar el rendimiento en clases con pocas muestras.
*   **Regularización:** Aplicación de L2, Dropout y Data Augmentation para mitigar el sobreajuste.

## Resultados Comparativos

| Modelo | Accuracy | Macro F1-Score | Características |
| :--- | :--- | :--- | :--- |
| **CNN Simple** | ~53% | 0.50 | Modelo base, alto sobreajuste. |
| **VGG16 + Tuning** | **~69%** | **0.68** | **Transfer Learning + Data Augmentation.** |

## Instalación y Uso

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/Clasificacion_de_Gemas.git
   ```
2. Instala las dependencias:
   ```bash
   pip install tensorflow pandas matplotlib seaborn scikit-learn kagglehub
   ```
3. Ejecuta el notebook en Google Colab o Jupyter para replicar el entrenamiento.

## Visualizaciones
El proyecto incluye reportes detallados de 
  **clasificación**, 
  **matrices de confusión**,
  análisis de las **Top 10** y **Bottom 10** clases según su desempeño
Lo que permite una interpretación clara de los puntos fuertes del modelo.

---
*Proyecto desarrollado para el Laboratorio 10 de Inteligencia Artificial - Universidad Autónoma de Chile - (2026).*
