# Homework-6-Multilayer-neural-network-with-hyperparameter-optimisation
Este repositorio contiene la implementación completa de una red neuronal multicapa con optimización de hiperparámetros, early stopping y evaluación multiclase para clasificar el estado de salud fetal a partir de variables médicas obtenidas por cardiotocografía.


El modelo clasifica los datos en tres clases:
•⁠  ⁠0: Normal
•⁠  ⁠1: Suspect
•⁠  ⁠2: Pathological

Se aplican técnicas de:
•⁠  ⁠Preprocesamiento de datos
•⁠  ⁠Estandarización
•⁠  ⁠Redes neuronales (Keras/TensorFlow)
•⁠  ⁠Optimización de hiperparámetros con Optuna
•⁠  ⁠Early Stopping
•⁠  ⁠Evaluación con métricas de clasificación

## Requisitos

Instalar las siguientes librerías:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow optuna
Cómo ejecutar
Clonar el repositorio:
git clone <TU_LINK>
cd <NOMBRE_DEL_REPO>
Abrir el notebook en Google Colab o Jupyter Notebook.
Asegurarse de tener el archivo:
fetal_health.csv

en la misma carpeta.

Ejecutar todas las celdas en orden.
Flujo del proyecto
Carga y exploración de datos
Limpieza (eliminación de duplicados)
Separación de variables (X, y)
División en train / validation / test
Estandarización
Diseño de la red neuronal
Entrenamiento del modelo
Optimización con Optuna
Early Stopping
Análisis de curvas de aprendizaje
Evaluación final (confusion matrix y métricas)
Guardado del modelo
Resultados
Accuracy aproximado de 0.94 en test
Buen desempeño general
Ligero overfitting controlado
Mejor desempeño en la clase Normal
Mayor dificultad en la clase Suspect
Modelo

El modelo se guarda en formato:

fetal_model.h5

Puede cargarse con:

from tensorflow.keras.models import load_model
model = load_model("fetal_model.h5")
Autores
Roberto Sandoval
Mauricio Gonzales
Dataset

Dataset obtenido de Kaggle:
https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification
