## Detección y conteo de piñas de pino en la especie arbórea Pinus Pinea mediante modelos de redes neuronales profundas utilizando imágenes RGB


<img src="/docs/piña.JPG" alt="fruto piña de pino"/>

En este repositorio se encuentran desarrollados dos algoritmos enfocados en la deteccion del pino piñonero, cada implementacion se realiza en el entorno colab en formato .ipynb con una guia paso a paso, con el fin de poder adaptar y entrenar para una base de datos propia.

Todos los conceptos vistos en este trbajo de grado estan explicados de forma detallada en [link]

## Objetivos

Objetivo General:

Desarrollar un sistema para la detección automática y conteo de piñas en la especie arbórea Pinus Pinea (comúnmente llamado Pino Piñonero) del Centro Tecnológico Forestal de Cataluña (CTFC), a partir de imágenes RGB adquiridas desde suelo, utilizando técnicas de aprendizaje profundo.

Objetivos Específicos:
 * Realizar el análisis y etiquetado manual de la base de datos adquirida desde suelo utilizando una cámara convencional RGB.
 * Estudiar, caracterizar e implementar arquitecturas de redes neuronales profundas apropiadas para el entrenamiento y validación en la detección y conteo de los piñas.
 * Realizar la comparación y validación de las redes neuronales profundas utilizando métricas de validación según la arquitectura de la red implementada.
 * Diseñar una estrategia de visualización de resultados de la red neuronal profunda para los investigadores del CTFC y otros usuarios.

## Metodologia 

El desarrollo de los detectores se realizaron bajo la siguiente estructura

<img src="/docs/metodologia.png" alt="Metodologia"/>

## Antes de empezar 

Es necesario familiarizarse con la plataforma - [Labelbox](https://labelbox.com/) 

Labelbox es el etiquetador online (pago) recomendado que se utilizo para el manejo de la base de datos, en especial para la limpieza, trabajo colaborativo y anotaciones.

Este anotador permite automaticar la importacion de la base de datos y para esto se debe obtener el ID del proyecto o el API key

![image](https://user-images.githubusercontent.com/58084716/186775756-c9b8d903-9c1d-40a6-bac9-d01b7cea6df5.png)



