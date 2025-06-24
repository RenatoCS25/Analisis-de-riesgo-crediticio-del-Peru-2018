# 🧠 Análisis de Riesgo Crediticio en el Perú

Este proyecto aplica técnicas de análisis de datos y aprendizaje automático para predecir la segmentación de riesgo crediticio de clientes, usando datos de entidades financieras peruanas. El modelo permite clasificar a los clientes en distintos niveles de riesgo para facilitar decisiones de crédito.

---

## 🎯 Objetivo

Predecir la **segmentación de riesgo crediticio** (bajo, medio, alto, etc.) de un cliente con base en variables personales, económicas y financieras.

---

## 📊 Fases del proyecto

### 🔹 1. Carga de datos

Se utilizó un archivo CSV con información sobre clientes: sexo, edad, ingresos, tipo de vivienda, garantías, avales, actividad económica y la clase de riesgo asignada.

---

### 🔹 2. Exploración inicial

Se analizó:
- Estructura del dataset
- Tipos de datos
- Distribución de clases
- Variables categóricas y numéricas

---

### 🔹 3. Limpieza de datos

- Tratamiento de valores faltantes
- Conversión de tipos
- Eliminación de columnas irrelevantes o redundantes

---

### 🔹 4. Análisis exploratorio de datos (EDA)

- Visualización de distribuciones y correlaciones
- Análisis por categoría de riesgo
- Gráficos de barras y boxplots

---

### 🔹 5. Ingeniería de características

- Codificación de variables categóricas con One-Hot Encoding
- Codificación de la variable objetivo con `LabelEncoder`
- Eliminación de columnas irrelevantes para el modelo

---

### 🔹 6. Preparación para el modelado

- Separación entre variables predictoras (`X`) y variable objetivo (`y`)
- Escalado de variables numéricas con `StandardScaler` (solo para modelos lineales)

---

### 🔹 7. División del conjunto de datos

- División del dataset en entrenamiento (70%) y prueba (30%)
- Estratificación para conservar proporciones de clases

---

### 🔹 8. Entrenamiento de modelos

Se entrenaron y compararon dos modelos de clasificación multiclase:

- **Regresión Logística (`LogisticRegression`)**: modelo base con escalado de datos.
- **Random Forest (`RandomForestClassifier`)**: modelo robusto que no requiere escalado.

---

### 🔹 9. Evaluación de modelos

- Reporte de clasificación (`classification_report`): precision, recall, f1-score
- Matriz de confusión (`confusion_matrix`)
- Visualización con heatmap (`Seaborn`)

---

### 🔹 10. Conclusiones

- El modelo de **Random Forest superó a la regresión logística** en todas las métricas.
- Mayor precisión en clases minoritarias.
- Random Forest fue el modelo seleccionado para el portafolio.

---

## 🛠️ Herramientas utilizadas

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib

---

## 📂 Estructura del proyecto

