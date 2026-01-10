# Actividad 3 – Machine Learning II

Magíster en Data Science  
Universidad de Las Américas (UDLA)

## Descripción general

Esta actividad corresponde a la **Actividad 3** de la asignatura *Machine Learning II* y se
desarrolla utilizando como base el proyecto trabajado previamente en el curso. Se mantiene el
mismo conjunto de datos, la definición de la variable objetivo y el esquema de preprocesamiento,
con el objetivo de profundizar en el análisis comparativo de modelos de clasificación supervisada.

El problema abordado consiste en la **predicción del riesgo de progresión hacia criterios del
Programa de Salud Cardiovascular (PSCV)** en usuarios atendidos en Atención Primaria de Salud (APS)
de la comuna de Quellón.

## Dataset

El dataset incluye **3.058 registros** provenientes del Control Cardiovascular y del Examen de
Medicina Preventiva del Adulto (EMPA), recopilados entre los años 2021 y 2023.

Variables consideradas:
- Variables clínicas continuas (edad, peso, talla, presión arterial, circunferencia de cintura, entre otras).
- Variable categórica (sexo).
- Variable objetivo binaria: progresión a PSCV.

El archivo de datos utilizado es:
- `data_model_pvc_quellon_2024_fin.xlsx`

## Metodología

Se aplicó un flujo metodológico consistente con lo visto en clases:
- Preprocesamiento mediante escalamiento de variables numéricas y codificación one-hot de variables categóricas.
- Separación train/test con muestreo estratificado.
- Validación cruzada estratificada para selección de hiperparámetros.
- Evaluación mediante métricas apropiadas para clases desbalanceadas.

## Modelos implementados

- **Gaussian Naïve Bayes**
  - Análisis de supuestos e independencia entre predictores.
  - Evaluación de desempeño y costo computacional.

- **Support Vector Machines (SVM)**
  - Comparación entre kernel lineal y kernel RBF.
  - Optimización de hiperparámetros mediante GridSearch.
  - Evaluación con y sin `class_weight="balanced"`.

## Resultados

Los resultados muestran que:
- Gaussian Naïve Bayes presenta un desempeño competitivo con bajo costo computacional.
- SVM con kernel RBF obtiene el mejor desempeño global en términos de PR-AUC y F1-score, a costa de
  un mayor tiempo de entrenamiento.
- El uso de `class_weight="balanced"` mejora el recall de la clase positiva, aspecto relevante en
  un contexto clínico.

## Ejecución

El análisis completo se encuentra documentado en el notebook:

- `Actividad_3.ipynb`

El notebook puede ejecutarse de forma secuencial sin requerir archivos adicionales.

