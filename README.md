# Métodos de Predicción Económica
## Artem Urlapov Sedova (Universidad Autónoma de Madrid)

<p align="justify">

### I - Análisis Univariante de Series Temporales (Tasa de Desempleo en Alemania, Enero 1994 - Septiembre 2024)

Se consigue un buen ajuste paramétrico mediante ARIMA (1, 1, 2). Planteamos un 3-step-ahead point forecast.


### I - Análisis Univariante de Series Temporales mediante Deep Learning (Euribor, Enero 1994 - Octubre 2024)

Elaborar un TSA del Euríbor en clave paramétrica supone una evidente dificultad, en tanto que un quiebre estructural observable de 74 meses del euríbor en territorio negativo (desde 02/2016 hasta 03/2022).

Adicionalmente, cuando el euríbor vuelve a entrar en territorio positivo, sólo disponemos de 31 muestras que, si quisiésemos analizar por separado, no sería un número estadísticamente robusto al separar el dataset en "train" y "test".

Por estos motivos, planteamos dos modelos de Deep Learning (Long Short-Term Memory y Gated Recurrent Units), dentro de Redes Neuronales Recurrentes, que pueden explotar mejor las particularidades previamente descritas.

Conseguimos un buen ajuste, con un RMSE de algo más de > 2, y realizamos un 3-step-ahead point forecast.

El conocimiento del contexto económico nos sugiere que el modelo LSTM (Long Short-Term Memory) es el más apropiado.

</p>
