# Práctica de Machine Learning – Predicción de precios en Airbnb

## Autor
Rubén Cerezo

## Objetivo de la práctica

El objetivo de esta práctica es abordar un problema de Machine Learning realista siguiendo la metodología y las buenas prácticas explicadas durante el curso.

El problema planteado es de regresión, y consiste en predecir el precio de un alojamiento de Airbnb a partir de un conjunto de datos reales obtenido mediante técnicas de scraping.

Tal y como se especifica en el enunciado oficial de la práctica, no se buscan resultados espectaculares, sino un proceso coherente, bien razonado y sin errores conceptuales graves, priorizando la correcta aplicación de las técnicas vistas en clase.

He mantenido la entrega 1 en caso de que se quiera comprobar el primer intento de esta práctica, pero realmente el archivo importante es la entrega 2. 
Además, pese a que es requisito entregar el notebook con las celdas ejecutadas, no he ejecutado la celda con el iprofiler ya que este hacía imposible subir el archivo a github (ocupaba demasiado espacio)
---

## Estructura del repositorio

airbnb-listings-extract.csv  
entrega.ipynb  
entrega2.ipynb        ← Notebook principal de la práctica  
Práctica ML.pdf       ← Enunciado oficial  
profiling_report.html  
profiling_report_madrid.html  
.gitattributes  
.git/  

El desarrollo completo de la práctica se encuentra en el notebook entrega2.ipynb.

---

## Conjunto de datos

El dataset utilizado contiene datos reales de Airbnb, lo que implica:

- Presencia de valores nulos  
- Distribuciones no uniformes  
- Posibles outliers  
- Variables heterogéneas (numéricas y categóricas)  

Este carácter realista obliga a realizar un análisis y limpieza más profundos que en datasets académicos simplificados, tal y como se indica en el enunciado de la práctica.

---

## Metodología seguida

El notebook entrega2.ipynb sigue los pasos recomendados en el enunciado oficial.

### 1. Preparación de los datos

- División del dataset en train / test  
- Separación de variables predictoras y variable objetivo (precio)  

---

### 2. Análisis exploratorio de datos (EDA)

- Inspección inicial del dataset (head, describe, dtypes)  
- Análisis de valores nulos  
- Detección de outliers  
- Estudio de correlaciones  
- Apoyo visual mediante gráficas  

Además, se incluyen informes automáticos de profiling para facilitar el análisis exploratorio:

- profiling_report.html  
- profiling_report_madrid.html  

---

### 3. Preprocesamiento

Durante esta fase se aplican distintas técnicas de preparación de los datos, entre ellas:

- Eliminación de variables poco relevantes o problemáticas  
- Tratamiento de valores perdidos  
- Selección de variables basada en correlación y modelos  
- Inputación de valores nulos con distintas opciones según sea necesario (0, moda, media, mediana...)


---

### 4. Modelado

Se entrenan y evalúan distintos modelos de regresión siguiendo una aproximación incremental:

- Lasso
- Ridge
- Random Forest

El objetivo no es maximizar una métrica concreta, sino comparar el comportamiento de los modelos y detectar posibles problemas de overfitting o underfitting.

---

### 5. Conclusiones

La práctica finaliza con una breve reflexión escrita en la que se resumen:

- Los procedimientos llevados a cabo.
- Resumen de resultados obtenidos por cada modelo
- Comparativa y explicación de las métricas obtenidas por cada modelo 

Siguiendo las indicaciones del enunciado, estas conclusiones son cualitativas y razonadas, no puramente numéricas.

---

## Tecnologías utilizadas

- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- Jupyter Notebook
- Ydata_profiling  

--  

