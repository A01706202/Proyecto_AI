# Proyecto_AI

## Descripción

Este proyecto consta de una red neuronal que pueda identificar imágenes con estética Vaporwave y Synthwave


## dataset

El dataset de este proyecto son imágenes divididas en dos clases (Vaporwave y Synthwave) y fueron sacadas de Google, blogs, tiendas virtuales y Pinterest


## Red Neuronal

La arquitectura usada fue la VGG16, una red neuronal que tiene 16 capas de profundidad conectadas sequencialmente entre ellas 

Fue presentada en el paper "Very Deep Convolutional Networks for Large Scale Image Recognition" por Simonyan y Zisserman en 2014, donde tomaron métricas como la exactitud (accuracy) y la pérdida de información (loss) para ver su predicción, el cuál fue de aproximadamente 71.3%	(top-1 accuracy) y 90.1% (top-5 accuracy).

Gracias a que es una arquitectura simple de modificar y entender, fue la que se usó en este proyecto.


## Versiones de cambios

1° Cambio: Al principio se trató de implementar ResNet50, pero al ser muy compleja de modificar, se cambió a VGG16.
2° Cambio: Se implementó VGG16, pero no daba un buen resultado al identificar imágenes vaporwave. Se agregó más imágenes a la base de datos para mejorarla y dio un mejor resultado.
2° Cambio: Para tratar de mejorar el modelo, se hicieron otras dos versiones del modelo. Una con más capa y la otra cambiando el optimizador a Adam y se subieron el número de epochs.


## Resultados

EL modelo VGG16 original (el primero que se implementó) fue el que obtuvo una mejor predicción. El modelo con más capas tuvo una menor pérdida, pero también la peor predicción de los tres, esto es por el overfitting. Y el modelo con el optimizador Adam y el aumento de épocas (Epochs) tuvo casi la misma exactitud que el primero, pero una mayor pérdida, por que que su predicción fue un poco más bajo. 
