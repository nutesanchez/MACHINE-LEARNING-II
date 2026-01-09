# Actividad 1 – Machine Learning II  
**Magíster en Data Science – Universidad de Las Américas (UDLA)**

##  Contexto
Esta actividad se desarrolla en el marco de la asignatura **Machine Learning II** y utiliza un **dataset propio**, construido a partir de registros del **Programa de Salud Cardiovascular (PSCV)**, el cual ha sido trabajado de forma transversal en las distintas actividades del curso.

El problema abordado corresponde a un **problema de clasificación supervisada**, donde el objetivo es **predecir un evento binario de interés clínico** asociado al PSCV, utilizando variables sociodemográficas, clínicas y de control de salud.

El uso de un dataset propio permite contextualizar el modelamiento en un escenario real del ámbito de la salud, manteniendo coherencia metodológica con los contenidos de la asignatura.

---

## Objetivo de la actividad
Implementar y evaluar modelos de **regresión logística**, comparando:

1. Un **modelo base** con variables preprocesadas.
2. Un modelo que incorpora **transformaciones polinomiales** sobre variables numéricas seleccionadas.
3. Modelos con **penalización (regularización)** para controlar la complejidad y el sobreajuste.

La evaluación se realiza mediante **validación cruzada k-fold**, utilizando métricas adecuadas para problemas de clasificación y potencial desbalance de clases.

---

## Estructura del repositorio

```text
actividad_1/
│
├── notebooks/
│   └── actividad_1_ml2.ipynb
│
├── data/
│   └── dataset_pscv.csv
│
└── README.md

