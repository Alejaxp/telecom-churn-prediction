# Predicción de Cancelación de Clientes (Customer Churn)
## Descripción del proyecto

Este proyecto tiene como objetivo analizar los factores que influyen en la cancelación de clientes (churn) en una empresa de telecomunicaciones y desarrollar modelos de Machine Learning capaces de predecir qué clientes tienen mayor probabilidad de abandonar el servicio.

Para ello se realizó un proceso completo de preparación de datos, análisis exploratorio, construcción de modelos predictivos y evaluación de resultados, con el fin de identificar patrones relevantes y proponer estrategias de retención de clientes.

## Objetivos

1. Analizar los factores que influyen en la cancelación de clientes.
2. Preparar y transformar los datos para su uso en modelos de Machine Learning.
3. Construir modelos predictivos para identificar clientes con alto riesgo de churn.
4. Comparar el desempeño de diferentes modelos de clasificación.
5. Identificar variables clave que impactan en la cancelación de clientes.
6. Proponer estrategias de retención basadas en los resultados obtenidos.

## Dataset

El conjunto de datos contiene información sobre clientes de una empresa de telecomunicaciones, incluyendo:

- Información demográfica del cliente
- Servicios contratados
- Tipo de contrato
- Método de pago
- Cargos mensuales y totales
- Antigüedad del cliente
- Estado de cancelación del servicio (Churn)

La variable objetivo del análisis es Churn, que indica si el cliente canceló el servicio o permaneció activo.

## Proceso de análisis

El proyecto se desarrolló siguiendo varias etapas del flujo de trabajo en ciencia de datos:

1. Limpieza y preparación de datos
   
- Eliminación de variables irrelevantes (como identificadores).
- Conversión de variables categóricas a formato numérico mediante One-Hot Encoding.
- Revisión de valores faltantes.
- Análisis del balance de clases.

2. Análisis exploratorio de datos

Se exploraron relaciones entre variables relevantes y la cancelación de clientes mediante visualizaciones como:

- Matriz de correlación
- Boxplots
- Scatter plots

Esto permitió identificar patrones importantes relacionados con el churn.

3. División del conjunto de datos

El dataset fue dividido en:

- 70% entrenamiento
- 30% prueba

Esto permite evaluar la capacidad de generalización de los modelos.

4. Modelos predictivos

Se implementaron dos modelos de clasificación:

### Regresión Logística

- Requiere normalización de los datos
- Permite interpretar la influencia de las variables mediante coeficientes

### Random Forest

- Modelo basado en árboles de decisión
- No requiere normalización
- Permite identificar la importancia de las variables

5. Evaluación de modelos

Los modelos fueron evaluados utilizando diferentes métricas:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión

Esto permitió comparar el desempeño de cada modelo en la predicción de la cancelación de clientes.

## Resultados principales

El análisis permitió identificar varios factores asociados con la cancelación de clientes, entre ellos:

- Antigüedad del cliente
- Cargo mensual
- Cargo total acumulado
- Tipo de contrato
- Servicios adicionales de internet

Los resultados indican que los clientes con menor tiempo de permanencia y contratos más flexibles presentan mayor probabilidad de cancelar el servicio.

En la comparación de modelos, Random Forest mostró un mejor desempeño predictivo, al capturar relaciones más complejas entre las variables.

## Estrategias de retención propuestas

Con base en los resultados del análisis, se proponen algunas estrategias para reducir la cancelación de clientes:

1. Fortalecer la fidelización durante los primeros meses del servicio.
2. Incentivar contratos de mayor duración mediante beneficios o descuentos.
3. Promover servicios adicionales que aumenten el valor percibido del servicio.
4. Identificar y monitorear clientes con alto riesgo de cancelación para aplicar acciones preventivas.

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Estructura del repositorio

├── data
│   └── telecom_churn_limpio.csv
├── notebooks
│   └── analisis_churn.ipynb
├── README.md


## Autor

Proyecto desarrollado por Alejandra Pardo como parte de un ejercicio de análisis de datos y machine learning enfocado en la predicción de cancelación de clientes.
