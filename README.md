## Detección y conteo de piñas de pino en la especie arbórea Pinus Pinea mediante modelos de redes neuronales profundas utilizando imágenes RGB


<img src="/docs/piña.JPG" alt="fruto piña de pino"/>

En este repositorio se encuentran desarrollados dos algoritmos enfocados en la deteccion del pino piñonero, cada implementacion se realiza en el entorno colab en formato .ipynb con una guia paso a paso, con el fin de poder adaptar y entrenar para una base de datos propia.

Todos los conceptos vistos en este trbajo de grado estan explicados de forma detallada en [link]

## Objetivo general

Desarrollar un sistema para la detección automática y conteo de piñas en la especie arbórea Pinus Pinea (comúnmente llamado Pino Piñonero) del Centro Tecnológico Forestal de Cataluña (CTFC), a partir de imágenes RGB adquiridas desde suelo, utilizando técnicas de aprendizaje profundo.


## Metodologia 

El desarrollo de los detectores se realizaron bajo la siguiente estructura

<img src="/docs/metodologia.png" alt="Metodologia"/>

## Antes de empezar 

Es necesario familiarizarse con la plataforma - [Labelbox](https://labelbox.com/) 
Labelbox es el etiquetador online (pago) que se utilizo para el manejo de la base de datos, en especial la limpieza, trabajo colaborativo y anotaciones. 

Para ello seguir los sigueintes pasos:

1. Crear un nuevo poyecto
![image](https://user-images.githubusercontent.com/58084716/186775967-96fb58bb-a49e-4f13-9d99-e1ec6cdfa045.png)

2. Agrear titulo, descripcion y tipo de dato, en este caso se seleccionan imagenes. 
3.
![image](https://user-images.githubusercontent.com/58084716/186776305-4f90a0d2-e738-49d5-a586-a6d82fa7bc45.png)

3. Buscar la seccion labels para empezar a etiquetar
4.
![image](https://user-images.githubusercontent.com/58084716/186776478-4b028a45-a17f-4cc7-acde-9de72d8b4bd3.png)

4. Crear la clase a tratar, en este caso pina, etiquetar y guardar

![image](https://user-images.githubusercontent.com/58084716/186776970-ac354398-2785-4206-8632-28849c1f0156.png)

5. De manera colaborativa es posible aprobar o no las etiquetas

![image](https://user-images.githubusercontent.com/58084716/186777070-2c8236d2-fa41-495f-ad83-4507ba77ca75.png)

6. Para poder vincular la base de datos con el entorno Colab es necesario tener :
 
 * La API del proyecto 
![image](https://user-images.githubusercontent.com/58084716/186777353-e523ce28-41e0-4f7c-ab18-600375e09e3d.png)

 * La API de la base de datos
![image](https://user-images.githubusercontent.com/58084716/186777443-663abbc5-d2aa-490d-bed2-e5e47cec0ea2.png)

 * Finalmente la API KEY

![image](https://user-images.githubusercontent.com/58084716/186777601-04ef7a27-00af-4896-a246-07ccfcd07e88.png)
![image](https://user-images.githubusercontent.com/58084716/186777763-3695acd3-6516-4be7-bea4-c4b104664afb.png)

## implementacion de modelos

Teniendo todas las API'S es posible seguir los modelos ubicados en la carpeta [Detectores](https://github.com/Tesis-deteccion-y-conteo-de-pinas/Detectores-pina-de-pino/tree/main/Detectores)

Para ejecuatar el detectron, deben abir el notebook en colab 





