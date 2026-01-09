# Proyecto Final – Machine Learning II

## Predicción temprana de progresión a riesgo cardiovascular en APS rural

### Autores
- Claudio Cárdenas Mansilla  
- Evelyn Sánchez Cabezas  

### Programa
Magíster en Data Science  
Universidad de Las Américas (UDLA)  

---

## 1. Descripción del proyecto

Este proyecto tiene como objetivo desarrollar y evaluar modelos de aprendizaje supervisado para la **predicción temprana de la progresión hacia criterios del Programa de Salud Cardiovascular (PSCV)** en usuarios de Atención Primaria de Salud (APS) rural de la comuna de Quellón.

El enfoque busca apoyar la **priorización preventiva**, utilizando exclusivamente variables clínicas rutinarias obtenidas del Examen de Medicina Preventiva del Adulto (EMPA) y controles cardiovasculares, sin requerir exámenes complejos ni de alto costo.

---

## 2. Datos utilizados

Se utilizaron registros clínicos reales de APS rural, que incluyen variables como:
- Edad
- Sexo
- Presión arterial sistólica y diastólica
- Circunferencia de cintura
- Colesterol total
- Peso y talla

Archivo principal de datos:
- `data_model_pscv_quellon_2024_fin.xlsx`

---

## 3. Metodología

El problema fue abordado como una **clasificación binaria** (progresión / no progresión a criterios PSCV).

Las principales etapas metodológicas fueron:
- Análisis exploratorio de datos (EDA)
- Preprocesamiento mediante pipelines reproducibles (tratamiento de outliers, escalamiento y codificación)
- Entrenamiento y comparación de modelos supervisados
- Validación cruzada estratificada
- Evaluación con métricas robustas, priorizando PR-AUC
- Análisis de interpretabilidad mediante SHAP

---

## 4. Modelos evaluados

Se entrenaron y compararon los siguientes modelos:
- Regresión logística (base, L1, L2 y polinómica)
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- XGBoost

El modelo **XGBoost optimizado** presentó el mejor desempeño global, con un equilibrio adecuado entre sensibilidad y precisión, siendo seleccionado como modelo principal para priorización preventiva.

---

## 5. Interpretabilidad y uso responsable

Se incorporaron técnicas de interpretabilidad basadas en **SHAP**, permitiendo identificar variables clínicamente relevantes como edad, circunferencia de cintura y presión arterial sistólica.

El modelo debe utilizarse **exclusivamente como herramienta de apoyo a la decisión clínica y planificación sanitaria**, y no como sistema automático de diagnóstico.

---

## 6. Archivos del proyecto

- `PROYECTO_FINAL_ML_II_MDS CLAUDIO E EVELYN S.ipynb`  
  Notebook principal con el desarrollo completo del análisis y modelamiento.

- `PRESENTACION PROYECTO FINAL ML II MDS.pdf`  
  Presentación final del proyecto.

- `Resumen del Proyecto Final ML II Claudio Cardenas Evelyn Sanchez.pdf`  
  Resumen ejecutivo del proyecto.

- `data_model_pscv_quellon_2024_fin.xlsx`  
  Base de datos utilizada para el análisis.

---

## 7. Observaciones finales

Este proyecto demuestra la factibilidad de utilizar datos clínicos rutinarios de APS para apoyar estrategias de detección precoz y gestión del riesgo cardiovascular, con potencial de escalabilidad a otros contextos, previa validación externa.

