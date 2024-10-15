Predicción de Vivienda

Este proyecto tiene como objetivo predecir el precio de las viviendas utilizando distintos 
modelos de Machine Learning. A través de este análisis, se busca comprender cómo 
las variables disponibles influyen en el precio y evaluar la precisión de las predicciones 
realizadas.

Contenido del Proyecto

1. Importación de Librerías
Se importan todas las librerías necesarias para la exploración, limpieza y modelado de 
los datos. Esto incluye librerías para la manipulación de datos, visualización y 
construcción de modelos de Machine Learning.

3. Importación y Exploración de Datos
Los datos se cargan y se realiza una exploración inicial para comprender mejor las 
variables disponibles. Se identifican variables numéricas como price, bedrooms, 
bathrooms, sqft_living, entre otras, y variables categóricas como street, city, statezip y 
country. Además, se genera un resumen estadístico de las variables y se analizan 
valores nulos y distribuciones.

5. Limpieza de Datos y Manejo de Outliers
Se lleva a cabo la limpieza de duplicados y el tratamiento de outliers utilizando el rango 
intercuartílico (IQR). Los outliers se identifican y eliminan para las variables price, 
sqft_living, sqft_lot, sqft_above y sqft_basement con el objetivo de asegurar una 
distribución de datos adecuada. Algunos outliers también se eliminan de forma manual 
para mejorar la calidad del modelo.

7. Visualización de Datos
Se crean gráficos exploratorios para analizar la relación entre las variables y determinar 
las posibles variables predictoras. El uso de gráficos de dispersión y mapas de calor 
permite identificar patrones y correlaciones entre las variables, ayudando a seleccionar 
las más relevantes para el modelado.

9. Modelado de Machine Learning
Se desarrollan diferentes modelos de Machine Learning para predecir el precio de la 
vivienda:
• Modelo 1: Utiliza variables numéricas con alta correlación con el precio y baja 
correlación entre sí, para reducir el ruido y mejorar la precisión del modelo.
• Modelo 2: Incluye variables numéricas adicionales, incluso aquellas con 
correlación entre sí, para observar el impacto del ruido en las predicciones.
• Modelo 3: Prueba únicamente con variables categóricas para predecir el precio, 
pero se encuentra que estas no son suficientemente predictivas por sí solas.
• Modelo 4: Combina variables categóricas seleccionadas (city, condition, zip) con 
variables numéricas para mejorar la predicción del precio de la vivienda.

11. Escalamiento de Variables
Para mejorar el rendimiento del modelo, se escala la variable price debido a su amplia 
variación en el rango de valores. Este proceso de normalización ayuda a que los 
modelos de Machine Learning converjan más rápidamente y de manera efectiva.

13. Validación del Modelo
Cada modelo se valida utilizando métricas de rendimiento, como el Mean Squared 
Error (MSE), tanto en el conjunto de entrenamiento como en el de prueba. Esto permite 
evaluar el grado de ajuste del modelo y su capacidad de generalización.

15. Conclusiones
Los gráficos de calor y las correlaciones entre las variables son esenciales para 
identificar qué variables utilizar en la predicción. Es preferible evitar variables altamente 
correlacionadas para minimizar el ruido y evitar el sobreajuste. Además, se observó 
que las variables categóricas con menos variedad son más útiles para la predicción del 
precio. En resumen, un buen preprocesamiento y la selección adecuada de variables 
son cruciales para obtener un modelo robusto y preciso.
