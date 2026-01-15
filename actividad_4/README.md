# Actividad 4 – Machine Learning II  
**Redes Neuronales Artificiales y Convolucionales**

## Contexto
En esta actividad se aborda el uso de **Redes Neuronales Artificiales (ANN)** y **Redes Neuronales Convolucionales (CNN)** aplicadas a un problema de **clasificación de churn**, dando continuidad al trabajo realizado en actividades previas con modelos tradicionales como regresión logística, Random Forest y SVM.

El objetivo es comprender la formulación, entrenamiento y evaluación de redes neuronales, así como analizar sus ventajas y limitaciones en comparación con modelos clásicos de Machine Learning.

## Objetivos de aprendizaje
Al finalizar esta actividad, se busca:
- Implementar una red neuronal artificial tipo *Multi-Layer Perceptron (MLP)* para clasificación.
- Comprender el rol de las funciones de activación, función de pérdida y algoritmos de optimización.
- Analizar el impacto del *learning rate*, *batch size* y número de épocas en el entrenamiento.
- Implementar una red neuronal convolucional (CNN) básica.
- Comparar redes neuronales con modelos tradicionales en términos de desempeño, interpretabilidad y costo computacional.

## Dataset
Se utiliza el **dataset de churn** empleado en actividades anteriores, manteniendo el mismo esquema de preprocesamiento:
- Imputación de valores faltantes.
- Codificación *one-hot* de variables categóricas.
- Escalamiento de variables numéricas.

## Metodología

### 1. Red Neuronal Artificial (MLP)
- Definición de una red densa con:
  - Capa de entrada acorde al número de variables.
  - Una o dos capas ocultas.
  - Capa de salida con activación sigmoidal.
- Justificación de:
  - Número de capas y neuronas.
  - Funciones de activación.
  - Función de pérdida y optimizador.
- Entrenamiento del modelo y análisis de la convergencia.

### 2. Análisis del entrenamiento
- Evaluación del efecto de distintos valores de *learning rate*.
- Comparación de distintos *batch sizes* (16, 32 y 64).
- Discusión sobre estabilidad, convergencia y tiempo de entrenamiento.
- Evaluación en conjunto de test mediante:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - AUC-ROC
  - PR-AUC
- Visualización de curvas ROC y Precision–Recall.

### 3. Red Neuronal Convolucional (CNN)
- Transformación del dataset a una representación matricial simple.
- Implementación de una CNN básica con:
  - Capa convolucional.
  - Operación de *pooling*.
  - Capa densa final.
- Discusión del rol de *kernels*, *stride* y *pooling*.

### 4. Comparación final
Se comparan los siguientes modelos:
- Regresión Logística  
- Random Forest  
- SVM  
- Red Neuronal Artificial (MLP)  
- Red Neuronal Convolucional (CNN)  

El análisis considera:
- Desempeño predictivo.
- Interpretabilidad.
- Costo computacional.
- Escalabilidad.
- Riesgo de sobreajuste.
- Influencia del tamaño del dataset.
- Pertinencia del uso de redes neuronales desde una perspectiva de negocio.

## Resultados y conclusiones
Los resultados permiten evaluar en qué escenarios las redes neuronales aportan ventajas reales frente a modelos clásicos, destacando los compromisos entre desempeño, complejidad y costos computacionales en el contexto del problema de churn.

## Formato de entrega
La actividad se entrega mediante un **notebook en Python**, que incluye:
- Código limpio y ordenado.
- Visualizaciones y tablas de resultados.
- Secciones en Markdown con:
  - Descripción del preprocesamiento.
  - Comparación de modelos.
  - Discusión de resultados.
  - Conclusiones.

## Autores
**Claudio Cardenas**  
**Evelyn Sánchez**  
Magíster en Data Science – Universidad de Las Américas
