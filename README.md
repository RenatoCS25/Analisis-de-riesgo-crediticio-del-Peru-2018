# 🧠 Análisis de Riesgo Crediticio en el Perú

Este proyecto tiene como finalidad aplicar técnicas de ciencia de datos y machine learning para abordar un problema real del sector financiero: **la evaluación del riesgo crediticio de potenciales clientes**.

A través del análisis de datos históricos de personas evaluadas por entidades financieras peruanas, se busca construir un modelo capaz de predecir con precisión el nivel de riesgo crediticio que representa un solicitante, clasificándolo en distintas categorías (por ejemplo: bajo, medio, alto, etc.).

El modelo puede ser utilizado por instituciones financieras para optimizar decisiones relacionadas con la aprobación de préstamos, asignación de garantías o necesidad de avales. Una evaluación automatizada y precisa del riesgo reduce la morosidad y mejora la inclusión financiera.

---

## 🎯 Objetivo

Desarrollar un sistema predictivo de clasificación multiclase que, a partir de atributos personales y económicos de los solicitantes, determine su **segmentación de riesgo crediticio**. El modelo busca:

- Anticipar el nivel de riesgo (bajo, medio, alto, etc.) asociado a un cliente.
- Automatizar la evaluación de perfiles crediticios.
- Proporcionar una herramienta de apoyo a la toma de decisiones crediticias.
- Evaluar y comparar distintos algoritmos de clasificación aplicables al contexto financiero peruano.

El resultado final es un modelo entrenado, evaluado y documentado, listo para ser integrado como parte de un sistema de análisis de riesgo en entornos reales.


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

