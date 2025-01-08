# Prediccion_de_serie_temporal_para_pedidos_de_taxi
Este es un proyecto que nos predice la cantidad de pedidos de taxi para la hora siguiente con un RMSE menor a 48, con diferentes modelos de machien learning
# Introducción
La compañía Sweet Lift Taxi ha recopilado datos históricos sobre pedidos de taxis en los aeropuertos.
Necesitamos atraer a más conductores durante las horas pico para predecir la cantidad de pedidos de taxis para la próxima hora. Construiremos un modelo para dicha predicción.

La métrica RECM en el conjunto de prueba no debe ser superior a 48.

## Instrucciones del proyecto.

1. Descargaremos los datos y haremos el remuestreo por una hora.
2. Analizaremos los datos
3. Entrenaremos diferentes modelos con diferentes hiperparámetros. La muestra de prueba debe ser el 10% del conjunto de datos inicial.
4. Probaremos los datos usando la muestra de prueba y proporcionaremos una conclusión.
# Descripción de los datos
- Los datos se almacenan en el archivo `taxi.csv`. 	
- El número de pedidos está en la columna `'num_orders'`.
# Conclusión
- Realizamos un EDA y preprocesamos los datos como agregando nuevas caracteristicas a nuestro modelo reduciendo fluctuaciones y poniendo nuestra serie temporal en intervalos de una hora 

- Eliminamos los valores ausentes que se generaron

- Definimos nuestras caracteristicas y el objetivo a predecir, dividimos nuestro conjunto de datos en un conjunto de entrenamiento del 90% y de prueba del 10% de manera ordenada haciendo que el 10% fueran los ultimos datos de nuestra serie temporal!!

- Finalmente creamos una tabla con sus respectivas métricas para comparar los modelos, quedando como el mejor modelo:
**Regresion Lineal con un RECM de 19.4219, seguido de LightGBM de 30.34250**

