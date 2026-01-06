# Machine Learning II – Actividad 2  
**Magíster en Data Science – Universidad de Las Américas (UDLA)**

Este repositorio contiene el desarrollo de la **Actividad 2 del curso Machine Learning II**, correspondiente al Magíster en Data Science de la Universidad de Las Américas (UDLA).

El trabajo aborda un problema de **clasificación binaria en el contexto de salud**, utilizando técnicas de aprendizaje supervisado, con énfasis en el preprocesamiento adecuado de variables clínicas, validación cruzada y evaluación rigurosa del desempeño de los modelos.

---

## Objetivo del trabajo

Desarrollar y evaluar modelos de clasificación capaces de predecir la variable **PCV** a partir de variables clínicas y demográficas, aplicando buenas prácticas de Machine Learning, tales como:

- Separación clara entre variables predictoras y variable objetivo.
- Tratamiento diferenciado de variables numéricas y categóricas.
- Uso de pipelines y preprocesamiento reproducible.
- Evaluación mediante validación cruzada estratificada.
- Comparación de métricas de desempeño relevantes para clasificación.

---

## Estructura del repositorio

MACHINE-LEARNING-II/
│
├── notebooks/
│ └── ACTIVIDAD_2_ML_II_2025.ipynb
│
├── data/
│ └── data_model_pvc_quellon_2024_fin.xlsx
│
├── src/
│ └── utils.py
│
└── README.md


### Descripción de carpetas

- **notebooks/**  
  Contiene el notebook principal con todo el desarrollo del análisis: carga de datos, exploración, preprocesamiento, entrenamiento de modelos, evaluación y visualización de resultados.

- **data/**  
  Contiene el dataset utilizado para el modelamiento. Los datos se encuentran **anonimizados** y su uso es exclusivamente académico.

- **src/**  
  Incluye funciones auxiliares reutilizables (`utils.py`) para evaluación de modelos, cálculo de métricas, validación cruzada y generación de curvas ROC y Precision–Recall.

---

## Metodología

El flujo metodológico seguido en el notebook incluye:

1. Carga y revisión inicial del dataset.
2. Análisis exploratorio de datos (EDA).
3. Definición de la variable objetivo (**PCV**).
4. Identificación y separación de:
   - Variables numéricas.
   - Variables categóricas (forzando `SEXO` como categórica).
5. Construcción de pipelines de preprocesamiento.
6. Entrenamiento de modelos de clasificación.
7. Evaluación mediante validación cruzada estratificada.
8. Comparación de modelos utilizando métricas:
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - AUC-ROC
   - PR-AUC
9. Determinación de umbral óptimo mediante el índice de Youden.

---

## Resultados

Los resultados obtenidos permiten comparar el desempeño de distintos modelos de clasificación en términos de discriminación y balance entre sensibilidad y especificidad, utilizando tanto métricas numéricas como representaciones gráficas (curvas ROC y Precision–Recall).

El análisis se orienta a un contexto de apoyo a la toma de decisiones en salud, sin constituir una herramienta clínica aplicable directamente.

---

## Consideraciones éticas y de uso

- El dataset utilizado se encuentra anonimizado.
- El análisis tiene **fines exclusivamente académicos**.
- Los modelos desarrollados **no deben ser utilizados para diagnóstico clínico real**.
- El trabajo respeta principios básicos de ética y confidencialidad de datos.

---

## Autores

- **Evelyn Sánchez**  
  Académica – Nutricionista  
  Estudiante Magíster en Data Science  
  Universidad de Las Américas (UDLA)

- **Claudio Cárdenas**  
  Estudiante Magíster en Data Science  
  Universidad de Las Américas (UDLA)

---

## Curso

**Machine Learning II**  
Magíster en Data Science – UDLA  
Año 2026
