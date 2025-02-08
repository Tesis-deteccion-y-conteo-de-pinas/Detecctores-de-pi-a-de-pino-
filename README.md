## Detection and counting of pine cones in the tree species Pinus Pinea by means of deep neural network models using RGB images.

<img src="/docs/piña.JPG" alt="fruto piña de pino" width="450" height="350" >

In this repository are developed two algorithms focused on the detection of stone pine, each implementation is done in the Colab environment in .ipynb format with a step by step guide, in order to adapt and train an own database.
All the concepts necessary to understand the architecture and operation of the algorithms are explained in detail in the [paper](https://drive.google.com/file/d/1-GCklux25KECxikIuyw51cOWCI7xg_bT/view?usp=sharing) and in the step-by-step guide [Tutorial](https://www.youtube.com/watch?v=yPtMvMDRWPs&ab_channel=SANTIAGOCORTESCABRERA)

# General Objective

To develop a system for the automatic detection and counting of pine cones in the tree species Pinus Pinea (commonly called Pinus Piñonero) at the Forestry Technology Center of Catalonia (CTFC), from RGB images acquired from the ground, using deep learning techniques.


## Methodology
The development of the detectors was carried out under the following structure:

<img src="/docs/metodologia.png" alt="Metodología" width="600" height="500">

## Project status

The project objectives are fully addressed, therefore, the attached files are up to date.

## Development environment requirements

1.) To have the appropriate database.

2.) Be registered in the Labelbox (paid) or Roboflow (free) software.

3.) Google Colab environment for the use of an external GPU.

## Operation Guide

To begin with, it is necessary to familiarize yourself with the platform. [Labelbox](https://labelbox.com/), is the online tagger that was used for database management, in particular for:

*  Data cleaning
* Collaborative work 
* Annotations. 

To do this, follow these steps:

1. Create a new project

![image](https://user-images.githubusercontent.com/58084716/186775967-96fb58bb-a49e-4f13-9d99-e1ec6cdfa045.png)

2. Add title, description and data type, in this case images are selected.

![image](https://user-images.githubusercontent.com/58084716/186776305-4f90a0d2-e738-49d5-a586-a6d82fa7bc45.png)

3. Find the Labels section to start labeling

![image](https://user-images.githubusercontent.com/58084716/186776478-4b028a45-a17f-4cc7-acde-9de72d8b4bd3.png)

4. Create the class to edit, in this case pineapple, label and save.

![image](https://user-images.githubusercontent.com/58084716/186776970-ac354398-2785-4206-8632-28849c1f0156.png)

5. Collaboratively it is possible to approve or not the labels.

![image](https://user-images.githubusercontent.com/58084716/186777070-2c8236d2-fa41-495f-ad83-4507ba77ca75.png)

6. To be able to link the database with the Colab environment it is necessary to have:
 
 * The project API
 
![image](https://user-images.githubusercontent.com/58084716/186777353-e523ce28-41e0-4f7c-ab18-600375e09e3d.png)

 * The database API
 
![image](https://user-images.githubusercontent.com/58084716/186777443-663abbc5-d2aa-490d-bed2-e5e47cec0ea2.png)

 * Finally the API KEY

![image](https://user-images.githubusercontent.com/58084716/186777601-04ef7a27-00af-4896-a246-07ccfcd07e88.png)

![image](https://user-images.githubusercontent.com/58084716/186777763-3695acd3-6516-4be7-bea4-c4b104664afb.png)

## Model implementation

Having the API Key and the ID's of the project and database, it is possible to follow the models located in the folder [Detectors.](https://github.com/Tesis-deteccion-y-conteo-de-pinas/Detectores-pina-de-pino/tree/main/Detectores) Each algorithm is organized step by step with small commentary guides that allow you to understand it a little more in depth.

* To run *Detectron2*, you must open the [Notebook](https://github.com/Tesis-deteccion-y-conteo-de-pinas/Detectores-pina-de-pino/blob/main/Detectores/Detectron2.ipynb) in Colab and follow the step by step.

* To run the *YOLOv5*, you must open the [Notebook](https://github.com/Tesis-deteccion-y-conteo-de-pinas/Detectores-pina-de-pino/blob/main/Detectores/YOLOv5.ipynb) in Colab and follow the step by step.

## Visualization of results

To visualize the results of the detectron, TensorBoard is used to monitor the metrics, in this case the Average precision (AP, AP50, AP75).

![image](https://user-images.githubusercontent.com/70868955/186993319-f220a6da-e20c-4eda-a634-6eb1ab4efe33.png)

YOLOv5 makes use of the Weights & Biases tool, a dashbord that stores each of the training sessions with the predictions made and the corresponding metrics.

![image](https://user-images.githubusercontent.com/70868955/186992031-03586818-0c72-40fa-9765-f3d77849601e.png)

![image](https://user-images.githubusercontent.com/70868955/186994576-438935dc-cf76-412a-92cf-8c1fa86dddd2.png)


## Copyrights
Prepared by:

* Vanesa Valentina Gomez De la Barrera (2420171072@estudiantesunibague.edu.co)

* Santiago Cortes Cabrera (2420171013@estudiantesunibague.edu.co)

Addressed to:

* PhD Ing. Jose Armando Fernández

Universidad de Ibague -2022
