## Detección y conteo de piñas de pino en la especie arbórea Pinus Pinea mediante modelos de redes neuronales profundas utilizando imágenes RGB

<img src="/docs/piña.JPG" alt="fruto piña de pino" width="450" height="350" >

En este repositorio se encuentran desarrollados dos algoritmos enfocados en la detección del pino piñonero, cada implementación se realiza en el entorno Colab en formato .ipynb con una guía paso a paso, con el fin de poder adaptar y entrenar una base de datos propia.
Todos los conceptos necesarios para poder entender la arquitectura y funcionamiento de los algoritmos se encuentran explicados de forma detallada en el [Trabajo de Grado](https://drive.google.com/file/d/1-GCklux25KECxikIuyw51cOWCI7xg_bT/view?usp=sharing)

# Objetivo general

Desarrollar un sistema para la detección automática y conteo de piñas en la especie arbórea Pinus Pinea (comúnmente llamado Pino Piñonero) del Centro Tecnológico Forestal de Cataluña (CTFC), a partir de imágenes RGB adquiridas desde suelo, utilizando técnicas de aprendizaje profundo.


## Metodología
El desarrollo de los detectores se realizó bajo la siguiente estructura

<img src="/docs/metodologia.png" alt="Metodología" width="600" height="500">

## Estado del proyecto

Los objetivos del proyecto se encuentran abordados en su totalidad, por lo tanto, los archivos adjuntos están actualizados.

## Requisitos del entorno de desarrollo

1.) Contar con la base de datos adecuada.

2.) Estar registrado en el software Labelbox (de pago) o Roboflow (gratuito).

3.) Entorno Colab de Google para el uso de una GPU externa.

## Guía de Funcionamiento

Para empezar, es necesario familiarizarse con la plataforma [Labelbox](https://labelbox.com/), es el etiquetador online que se utilizó para el manejo de la base de datos, en especial para:

* La limpieza de datos
* El trabajo colaborativo  
* Las anotaciones. 

Para ello, seguir los estos pasos:

1. Crear un nuevo proyecto
![image](https://user-images.githubusercontent.com/58084716/186775967-96fb58bb-a49e-4f13-9d99-e1ec6cdfa045.png)

2. Agregar título, descripción y tipo de dato, en este caso se seleccionan imágenes. 

![image](https://user-images.githubusercontent.com/58084716/186776305-4f90a0d2-e738-49d5-a586-a6d82fa7bc45.png)

3. Buscar la sección Labels para empezar a etiquetar

![image](https://user-images.githubusercontent.com/58084716/186776478-4b028a45-a17f-4cc7-acde-9de72d8b4bd3.png)

4. Crear la clase a tratar, en este caso pina, etiquetar y guardar

![image](https://user-images.githubusercontent.com/58084716/186776970-ac354398-2785-4206-8632-28849c1f0156.png)

5. De manera colaborativa es posible aprobar o no las etiquetas

![image](https://user-images.githubusercontent.com/58084716/186777070-2c8236d2-fa41-495f-ad83-4507ba77ca75.png)

6. Para poder vincular la base de datos con el entorno Colab es necesario tener:
 
 * La API del proyecto 
 
![image](https://user-images.githubusercontent.com/58084716/186777353-e523ce28-41e0-4f7c-ab18-600375e09e3d.png)

 * La API de la base de datos
 
![image](https://user-images.githubusercontent.com/58084716/186777443-663abbc5-d2aa-490d-bed2-e5e47cec0ea2.png)

 * Finalmente la API KEY

![image](https://user-images.githubusercontent.com/58084716/186777601-04ef7a27-00af-4896-a246-07ccfcd07e88.png)

![image](https://user-images.githubusercontent.com/58084716/186777763-3695acd3-6516-4be7-bea4-c4b104664afb.png)

## implementación de modelos

Teniendo la API Key y los ID's del proyecto y de la base de datos, es posible seguir los modelos ubicados en la carpeta [Detectores.](https://github.com/Tesis-deteccion-y-conteo-de-pinas/Detectores-pina-de-pino/tree/main/Detectores) Cada algoritmo está organizado paso a paso con pequeños comentarios guías que permiten entenderlo un poco más a profundidad.

* Para ejecutar *Detectron2*, se debe abrir el [Notebook](https://github.com/Tesis-deteccion-y-conteo-de-pinas/Detectores-pina-de-pino/blob/main/Detectores/Detectron2.ipynb) en Colab.

* Para ejecutar el *YOLOv5*, se debe abrir el [Notebook](https://github.com/Tesis-deteccion-y-conteo-de-pinas/Detectores-pina-de-pino/blob/main/Detectores/YOLOv5.ipynb) en Colab y seguir el paso a paso 

## Derechos de autor 
Elaborado por:

* Vanesa Valentina Gómez De la Barrera

* Santiago Cortes Cabrera

En dirección de:

* PhD Ing. José Armando Fernández

Universidad de Ibagué -2022
