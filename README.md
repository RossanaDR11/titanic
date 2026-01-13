# Titanic EDA & Preprocesamiento (Notebook)
 
Este repositorio contiene un notebook de **análisis exploratorio (EDA)** y **preprocesamiento** usando el dataset **Titanic**. El objetivo es practicar un flujo típico de preparación de datos: revisión de tipos, manejo de nulos, detección/tratamiento de duplicados y outliers, escalado, y análisis de relaciones entre variables numéricas y categóricas.
 
---
 
## 📌 Contenido del notebook
 
El notebook está organizado en secciones (con explicaciones y ejemplos):
 
### 1) Carga de datos
- Se utiliza el dataset `titanic` disponible en **seaborn**:
  - `sns.load_dataset("titanic")`
 
### 2) Preprocesamiento
- Revisión de tipos de datos.
- **Manejo de valores faltantes (nulos)** con estrategias simples.
- Revisión de **filas duplicadas** y decisión de eliminación (si aplica).
 
### 3) EDA (Análisis Exploratorio)
- Visualizaciones para entender distribuciones y comportamiento de variables.
- **Test de normalidad** para orientar decisiones estadísticas.
- Detección de **outliers**:
  - Si la distribución no es normal → enfoque basado en **IQR**
  - Si es normal → enfoque con **Z-score**
- Estrategias de tratamiento de outliers:
  - **Winsorizing** (reemplazo por límites superior/inferior)
 
### 4) Transformaciones y escalado
- Transformaciones (incluyendo **logarítmicas**) cuando tiene sentido por distribución.
- Alternativas de escalado, incluyendo **Robust Scaling**.
 
### 5) Correlaciones y relaciones entre variables
- Correlación entre variables numéricas y visualización (p.ej. heatmap).
- Relación entre variables **categóricas** (ej.: `sex` vs `survived`, `pclass` vs `survived`)
  - Tablas de contingencia (`pd.crosstab`)
  - **Test chi-cuadrado** (Chi-square)
 
### 6) Guía de selección de gráficos
- Tabla final con recomendaciones de visualizaciones según tipo de variable y objetivo.
 
---
 
## 🧰 Requisitos
 
Python 3.9+ recomendado.
 
**Librerías principales**:
- pandas
- numpy
- matplotlib
- seaborn
- scipy
 

pip install pandas numpy matplotlib seaborn scipy
