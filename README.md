# 📊 Telecom X 02 – Predicción de Cancelación de Clientes (Churn)

## 📌 Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar un **modelo predictivo capaz de identificar clientes con alta probabilidad de cancelar el servicio (churn)** en una empresa de telecomunicaciones.

A partir de datos previamente tratados, se realizó un **análisis exploratorio, selección de variables, preprocesamiento y entrenamiento de modelos de clasificación** para comprender los factores asociados al churn y evaluar qué modelo ofrece mejor desempeño predictivo.

El objetivo final es **apoyar la toma de decisiones empresariales mediante analítica de datos**, permitiendo anticipar clientes en riesgo y mejorar las estrategias de retención.

---

# 🎯 Objetivos

- Analizar la relación entre variables del cliente y la cancelación del servicio.
- Identificar **factores clave asociados al churn**.
- Preparar los datos para modelos de **Machine Learning**.
- Comparar distintos modelos de clasificación.
- Evaluar el desempeño mediante métricas adecuadas para **datasets desbalanceados**.

---

# 📂 Dataset

El dataset contiene información de clientes de telecomunicaciones, incluyendo:

- Datos demográficos del cliente
- Tipo de contrato
- Servicios contratados
- Antigüedad del cliente
- Cargos mensuales y totales
- Estado de cancelación (Churn)

La variable objetivo del modelo es **Churn_bin**, que indica si el cliente canceló o no el servicio.

---

# 🧰 Tecnologías Utilizadas

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

# 🔎 Metodología

El proyecto se desarrolló siguiendo las principales etapas de un flujo de trabajo en **Data Science**.

### 1. Importación de librerías
Se utilizaron bibliotecas para análisis de datos, visualización y modelado predictivo.

### 2. Carga de datos
Se trabajó con un dataset previamente procesado y estructurado para facilitar el análisis.

### 3. Análisis de correlación
Se evaluó la relación entre variables numéricas y la variable objetivo para identificar posibles predictores relevantes.

Principales hallazgos:

- **Tenure (antigüedad)** muestra correlación negativa con el churn.
- **Total Charges** también presenta relación negativa con la cancelación.
- **Monthly Charges** presenta una ligera correlación positiva.

Esto sugiere que **clientes con mayor permanencia tienden a cancelar menos**.

---

### 4. Preprocesamiento de datos

Se realizaron tareas de preparación para el modelado:

- Codificación de variables categóricas (**Encoding**)
- Normalización de variables numéricas
- Separación en **variables predictoras (X)** y **variable objetivo (y)**

---

# 🤖 Modelos de Machine Learning

Se entrenaron y compararon dos modelos de clasificación:

### Árbol de Decisión
- Modelo interpretable
- Permite identificar reglas de decisión
- Mejora la detección de churn respecto al modelo base

### Regresión Logística
- Modelo estadístico ampliamente utilizado en clasificación
- Presenta **mejor equilibrio entre precisión y recall**
- Obtiene el **mayor F1-score**

---

# 📊 Evaluación de Modelos

Los modelos fueron evaluados utilizando métricas adecuadas para problemas de churn:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión

Debido al **desbalance de clases**, se priorizaron **Recall y F1-score** para evaluar la capacidad de detectar clientes que cancelan.

---

# 📉 Principales Resultados

- El **modelo baseline** presenta alta accuracy pero no detecta correctamente clientes que cancelan.
- El **Árbol de Decisión** mejora la detección de churn.
- La **Regresión Logística** muestra el **mejor desempeño general**, con el mayor F1-score y mejor equilibrio entre precisión y recall.

---

# 🔑 Variables Relevantes para el Churn

El análisis permitió identificar factores asociados a la cancelación:

Mayor probabilidad de churn:

- Clientes con **menor antigüedad**
- **Contratos de corto plazo**
- Menor vinculación con servicios

Menor probabilidad de churn:

- **Mayor permanencia**
- **Contratos de largo plazo**
- Mayor uso de múltiples servicios

Esto indica que la cancelación depende de **una combinación de factores contractuales, económicos y de comportamiento del cliente**.

---

# 📌 Conclusiones

El proyecto demuestra que el uso de **modelos predictivos puede ayudar a identificar clientes en riesgo de cancelación**, permitiendo a las empresas:

- Anticipar pérdidas de clientes
- Diseñar estrategias de retención
- Tomar decisiones basadas en datos

La **Regresión Logística** resultó ser el modelo con mejor desempeño para este problema.
