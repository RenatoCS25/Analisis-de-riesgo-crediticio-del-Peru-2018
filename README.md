#  Análisis de riesgo crediticio en el Perú (2018)

**Autor:** [RenatoCS25](https://github.com/RenatoCS25)  
**Repositorio:** [Analisis-de-riesgo-crediticio-del-Peru-2018](https://github.com/RenatoCS25/Analisis-de-riesgo-crediticio-del-Peru-2018)  
**Archivo de datos:** [`credit_risk_es.csv`](https://github.com/RenatoCS25/Analisis-de-riesgo-crediticio-del-Peru-2018/blob/main/credit_risk_es.csv)

---

##  1. Contexto del negocio

En el sistema financiero peruano, los bancos y entidades crediticias enfrentan el desafío de equilibrar la rentabilidad con la gestión del riesgo. Este proyecto analiza los factores que influyen en el **riesgo crediticio de los clientes en el Perú durante el año 2018**, con el objetivo de identificar patrones, perfilar clientes de alto riesgo y proponer estrategias que permitan reducir la morosidad.

---

##  2. Objetivos y preguntas de análisis

### **Objetivo general**
Analizar los factores que determinan el nivel de riesgo crediticio de los clientes peruanos y generar recomendaciones accionables para mejorar la gestión del riesgo en instituciones financieras.

### **Preguntas clave**
- ¿Qué características (edad, ingresos, tipo de crédito, región, etc.) están más asociadas con un mayor riesgo crediticio?  
- ¿Existen diferencias significativas en el riesgo entre regiones del país?  
- ¿Qué tipo de crédito presenta mayor probabilidad de morosidad o incumplimiento?  
- ¿Qué variables pueden ser más útiles para construir un modelo de scoring crediticio?  
- ¿Qué acciones concretas pueden tomarse para reducir la exposición al riesgo?

---

##  3. Descripción del dataset

El dataset [`credit_risk_es.csv`](https://github.com/RenatoCS25/Analisis-de-riesgo-crediticio-del-Peru-2018/blob/main/credit_risk_es.csv) contiene información de clientes crediticios en el Perú durante el 2018. Incluye variables demográficas, financieras y de comportamiento crediticio, tales como:

| Tipo de variable | Ejemplo |
|------------------|----------|
| **Demográficas** | Edad, género, región, estado civil |
| **Financieras** | Ingresos, monto del crédito, tipo de crédito |
| **Historial de pago** | Días de mora, número de incumplimientos |
| **Clasificación de riesgo** | Bajo, medio o alto |

Antes del análisis se realizó limpieza, eliminación de valores faltantes, detección de outliers y transformación de variables categóricas.

---

##  4. Análisis exploratorio y hallazgos

- Los **clientes jóvenes** (menores de 30 años) y con **bajos ingresos** presentaron mayor probabilidad de caer en mora.  
- El **riesgo crediticio fue más alto en créditos de consumo**, mientras que los créditos hipotecarios o empresariales mostraron menor tasa de incumplimiento.  
- **Regiones con menor desarrollo económico** presentaron más casos de alto riesgo, reflejando el impacto del entorno socioeconómico.  
- El **historial de pagos previos** fue la variable más predictiva del nivel de riesgo, destacando su importancia para futuros modelos de scoring.  
- En general, los patrones demográficos por sí solos no explican el riesgo; se requiere una combinación de factores financieros y conductuales.

---

##  5. Insights clave

1. **Segmentos de alto riesgo:** jóvenes de bajos ingresos con créditos de consumo sin garantía concentran gran parte de los casos de morosidad.  
2. **Producto = riesgo:** los créditos de consumo muestran una mayor volatilidad y exposición a impagos.  
3. **Importancia del historial:** el historial de cumplimiento es el mejor indicador de riesgo; su calidad debe garantizarse en los sistemas internos.  
4. **Impacto regional:** la ubicación geográfica influye significativamente en el comportamiento crediticio, por lo que las políticas deben adaptarse al contexto regional.  
5. **Diversificación:** una cartera concentrada en créditos de alto riesgo eleva la exposición del banco; se debe equilibrar el portafolio.

---

##  6. Recomendaciones de negocio

1. Implementar un sistema de scoring crediticio segmentado, considerando edad, ingresos, tipo de crédito y ubicación del cliente.  
2. Revisar políticas para créditos de consumo, aplicando garantías adicionales o límites más estrictos para clientes de alto riesgo.  
3. Incorporar datos geográficos y socioeconómicos al análisis para una evaluación más contextualizada.  
4. Mejorar la calidad y trazabilidad del historial crediticio, evitando vacíos de información que afecten la predicción.  
5. Monitorear clientes en transición de riesgo medio a alto, aplicando alertas tempranas para evitar la morosidad.  
6. Capacitar al personal de crédito en detección temprana de señales de riesgo y en evaluación integral del cliente.

---

##  7. Tecnologías utilizadas

- **Lenguaje:** Python  
- **Entorno:** Jupyter Notebook  
- **Principales librerías:**  
  - `pandas` — manipulación y limpieza de datos  
  - `numpy` — cálculos numéricos  
  - `matplotlib` / `seaborn` — visualización de datos  
  - `scikit-learn` — análisis predictivo (si se aplica modelo de clasificación)  

---

##  8. Cómo reproducir el proyecto

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/RenatoCS25/Analisis-de-riesgo-crediticio-del-Peru-2018.git
