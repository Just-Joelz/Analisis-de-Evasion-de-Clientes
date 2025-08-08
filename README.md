Challenge 2 del Programa ONE de Oracle
# Análisis de Evasión de Clientes (Churn) - TelecomX

## Introducción

Este proyecto tiene como objetivo analizar los factores que influyen en la tasa de cancelación de clientes (Churn) de la empresa de telecomunicaciones TelecomX. La pérdida de clientes representa un desafío significativo para la empresa, por lo que comprender las causas subyacentes es fundamental para desarrollar estrategias de retención efectivas y mejorar la rentabilidad.

El análisis se basa en un conjunto de datos que contiene información detallada sobre los clientes, incluyendo datos demográficos, servicios contratados, información de facturación y estado de evasión (Churn).

## Objetivo

El objetivo principal de este análisis es:

* Identificar los principales factores que contribuyen a la evasión de clientes.
* Extraer información valiosa de los datos para informar la toma de decisiones estratégicas.
* Proporcionar insights que puedan ser utilizados por el equipo de Data Science para desarrollar modelos predictivos de Churn.

## Conjunto de Datos

El conjunto de datos utilizado en este análisis proviene del archivo `TelecomX_Data.json`, disponible en el siguiente enlace:

[https://raw.githubusercontent.com/Just-Joelz/Analisis-de-Evasion-de-Clientes/refs/heads/main/TelecomX_Data.json](https://raw.githubusercontent.com/Just-Joelz/Analisis-de-Evasion-de-Clientes/refs/heads/main/TelecomX_Data.json)

El diccionario de datos se incluye en el notebook para una mejor comprensión de las variables.

## Metodología

El análisis se llevó a cabo siguiendo las siguientes etapas:

1.  **Extracción de Datos:** Carga de los datos desde el archivo JSON.
2.  **Transformación de Datos:**
    *   Normalización de las columnas anidadas (`customer`, `phone`, `internet`, `account`) para crear un DataFrame plano.
    *   Limpieza de datos: identificación y tratamiento de valores nulos, duplicados y vacíos.
    *   Conversión de tipos de datos para las columnas numéricas.
    *   Creación de nuevas columnas derivadas (ej. `Cuentas Diarias`).
3.  **Análisis Exploratorio de Datos (EDA):**
    *   Análisis descriptivo de las variables.
    *   Visualización de la distribución de Churn y su relación con diferentes variables (género, edad, tipo de contrato, método de pago, cargos, antigüedad).
    *   Cálculo de la tasa de Churn por antigüedad.
4.  **Informe Final:** Resumen de los hallazgos clave, conclusiones e insights obtenidos del análisis exploratorio, y recomendaciones estratégicas.

## Herramientas y Librerías

*   Python
*   Pandas para manipulación y análisis de datos.
*   NumPy para operaciones numéricas.
*   Matplotlib y Seaborn para visualizaciones estáticas.
*   Plotly Express para visualizaciones interactivas.

## Resultados y Conclusiones

Los resultados del análisis exploratorio sugieren que varios factores están fuertemente asociados con la evasión de clientes, incluyendo:

*   **Tipo de Contrato:** Los clientes con contratos mes a mes presentan una tasa de evasión significativamente mayor.
*   **Método de Pago:** El pago electrónico está asociado con una mayor probabilidad de evasión.
*   **Antigüedad (Tenure):** Los clientes con menor antigüedad tienen una tasa de evasión considerablemente más alta.
*   **Cargos Mensuales:** Los clientes que evaden tienden a tener cargos mensuales más altos.

El informe final detallado en el notebook presenta conclusiones más específicas y recomendaciones basadas en estos hallazgos.

## Recomendaciones

Basado en los insights del análisis, se proponen recomendaciones estratégicas para reducir la tasa de Churn, como ofrecer incentivos para contratos a largo plazo, promover métodos de pago alternativos al cheque electrónico, implementar programas de retención temprana y segmentar a los clientes para personalizar las estrategias de retención.

## Cómo Ejecutar el Notebook

Para ejecutar este análisis, sigue los pasos a continuación:

1.  Abre el notebook en un entorno con Python y las librerías necesarias instaladas (por ejemplo, Google Colab, Jupyter Notebook).
2.  Asegúrate de tener acceso a internet para descargar el archivo JSON.
3.  Ejecuta las celdas del notebook secuencialmente.

## Autor

[Joel Hernández Robledo]
