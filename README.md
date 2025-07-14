# 🩺 Predicción de Enfermedad Coronaria con KNN
Proyecto de clasificación aplicado al **Framingham Heart Study Dataset**, que busca predecir si un paciente desarrollará enfermedad coronaria en los próximos 10 años. Se compararon modelos de K-Nearest Neighbors (KNN) y Regresión Logística, siendo KNN el modelo más efectivo.

---

## 📁 Dataset
- Fuente: [Framingham Heart Study Dataset (Kaggle)](https://www.kaggle.com/datasets/aasheesh200/framingham-heart-study-dataset)
- Descripción: Estudio longitudinal iniciado en 1948 en Framingham, Massachusetts, con datos médicos y demográficos de adultos entre 30 y 62 años.
- Variable objetivo: `TenYearCHD` (1 si la persona desarrolló enfermedad coronaria en los 10 años siguientes, 0 en caso contrario).

---

## ⚙️ Tecnologías utilizadas
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🔍 Análisis exploratorio (EDA)
- Visualización de la distribución de variables numéricas mediante histogramas con KDE.
- Cálculo de skewness para detectar variables asimétricas.
- Heatmap de correlaciones.
- Evaluación y tratamiento de valores faltantes.

---

## 🧪 Modelado
- Se implementaron dos modelos:
  - **Regresión Logística**: desempeño limitado.
  - **K-Nearest Neighbors (KNN)**: mejor rendimiento.
- Se utilizó **validación cruzada (5 folds)** con la métrica **ROC-AUC** para encontrar el mejor valor de `k` (n_neighbors).
- El valor óptimo fue **k = 1**.

---

## 📊 Evaluación del modelo
- **AUC-ROC en Validación:** 0.9247
- **AUC-ROC en Test:** 0.9565
- Se generó:
  - Reporte de clasificación (precision, recall, F1-score)
  - Matriz de confusión
  - Evaluación adicional sobre una muestra aleatoria del dataset original.

---

## 📌 Conclusión
El modelo KNN ajustado con validación cruzada mostró excelente desempeño en la predicción del riesgo de enfermedad coronaria, superando a la regresión logística. Este proyecto demuestra habilidades en análisis exploratorio, preprocesamiento, tuning de hiperparámetros y evaluación de modelos supervisados con Python.

---

## 📎 Archivo
Este proyecto se encuentra en un archivo Jupyter Notebook (`.ipynb`) con celdas bien documentadas, visualizaciones y resultados reproducibles.

