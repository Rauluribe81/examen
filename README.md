# 🧠 Clasificación de Supervivencia por Cáncer de Pulmón

Este proyecto corresponde a un ejercicio práctico de clasificación supervisada utilizando un conjunto de datos sobre pacientes con cáncer de pulmón. El objetivo es predecir si un paciente sobrevivió (`survived`) en función de variables médicas y tratamientos previos.

## 📂 Archivos utilizados

- `lung_cancer_mortality_data_large_v2.csv` — Datos de entrenamiento.
- `lung_cancer_mortality_data_test_v2.csv` — Datos de prueba para predicción final.

## 🎯 Objetivo del ejercicio

- Aplicar técnicas de Machine Learning para resolver un problema de clasificación binaria.
- Usar `RandomForestClassifier` como modelo principal.
- Evaluar el rendimiento del modelo con métricas estándar.
- Interpretar resultados mediante matriz de confusión y precisión del modelo.

---

🧪 Pasos realizados

 1. Carga y exploración de datos
- Carga de los datasets con `pandas`.
- Revisión de tipos de variables, valores nulos y distribución de la variable objetivo.

 2. Preprocesamiento
- Codificación de variables categóricas con `get_dummies`.
- Eliminación de columnas no numéricas o poco útiles como `end_treatment_date`.
- Verificación de correlación entre variables y la variable objetivo.

 3. Entrenamiento del modelo
- Se seleccionaron **solo las primeras 20 filas** del dataset para entrenamiento, según lo solicitado.
- División entre entrenamiento y validación (`train_test_split`).
- Entrenamiento del modelo con `RandomForestClassifier`.

 4. Evaluación
- Predicciones sobre el conjunto de validación.
- Generación de matriz de confusión.
- Métricas de clasificación: precisión, recall, F1-score y exactitud (`accuracy_score`).

---

 📊 Resultados

 Métricas obtenidas (entrenamiento con 20 registros)

- El modelo puede sobreajustarse debido al bajo volumen de datos.
- Las predicciones pueden no ser representativas del comportamiento real.
- A pesar de esto, se logró evaluar el flujo completo de un proyecto de clasificación.

 Matriz de Confusión

Se visualiza el rendimiento del modelo sobre datos de validación, con recuento de predicciones correctas e incorrectas.

---

 ✅ Conclusiones

- El volumen de datos usado (20 registros) limita severamente el rendimiento y generalización del modelo.
- Random Forest es una buena opción para explorar relacio
  

