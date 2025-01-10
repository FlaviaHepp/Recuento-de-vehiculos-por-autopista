# Recuento-de-vehiculos-por-autopista
Análisis de series temporales utilizando datos del recuento horario de vehículos en una autopista durante 1995. 

**Desarrollo**
El conjunto de datos incluye recuentos horarios de vehículos durante aproximadamente 70 días, a partir de agosto de 1995.
Se agregan los recuentos por día para simplificar el análisis.
**Análisis exploratorio**
Se visualizan estadísticas descriptivas y patrones generales en la serie temporal:
Media y mediana de los recuentos diarios.
Gráficas de series temporales y descomposiciones aditiva y multiplicativa (tendencia, estacionalidad y residuo).
**Modelos utilizados**
Regresión lineal :

Relación entre el tiempo (días) y los recuentos de vehículos.
Resultados evaluados con el RMSE en datos de prueba.
Suavizado exponencial simple (SES) :

Modelo básico para datos sin tendencia o estacionalidad.
Evaluación del RMSE en datos de prueba.
Suavizado exponencial doble (DES) :

Incluye tendencias lineales.
Se optimizan los parámetros de suavizado (
alfa
alfay
𝛽
β) para minimizar el RMSE.
Triple exponencial suavizado (TES) :

Considere tendencias y estacionalidad.
Se optimizan
alfa
alfa,
𝛽
βy
gamma
gammapara lograr predicciones más precisas.
Método de Holt-Winters :

Versión avanzada del TES para analizar patrones aditivos y multiplicativos.
Optimización de hiperparámetros :

Se realiza una búsqueda exhaustiva de los mejores valores de
alfa
alfa,
𝛽
βy
gamma
gammamediante un enfoque de búsqueda en cuadrícula.
Resultados y comparaciones
Los modelos fueron evaluados utilizando el RMSE en datos de prueba.
Holt-Winters (TES) fue el modelo con el mejor rendimiento, logrando el menor RMSE.
Se generaron gráficos comparativos que muestran predicciones junto con los datos de entrenamiento y prueba.
Conclusión
Este análisis ofrece una comprensión de los patrones en los datos de tráfico vehicular y demuestra cómo se pueden usar diversos modelos para predecir recuentos futuros. El enfoque combina técnicas de regresión y series temporales para encontrar la mejor estrategia predictiva.
