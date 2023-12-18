# MGP-CGAN

Repositorio de proyecto del Curso "Modelos generativos profundos"

En este repositorio se encuentran 2 notebooks que guian de forma intuitiva al proceso de entrenamiento de un modelo generativo CGAN: 

1. En `CGAN_FashionMNIST.ipynb` se trabaja con el dataset Fashion MNIST, el cual son imagenes 1x28x28 de prendas de vestir con 10 diferentes tipos de prendas, en este entrenamiento se utilizaron estructuras Fully Connected.

2. En `CGAN_CREMAD.ipynb` se trabaja con el dataset [CREMA-D](https://github.com/CheyneyComputerScience/CREMA-D), el cual son videos y audios de diferentes actores, tanto masculinos como femeninos, además de distintas etnias, el cual expresan 6 diferentes emociones mediante frases y expresiones faciales. La estructura de los modelos generativos como discriminativos se basaron de los implementados en el paper [Athanasiadis et al., 2019](https://doi.org/10.1016/j.neucom.2019.09.106), además de tambien incluir variantes Fully Connected.

Si bien el proceso de procesamiento de datos y entrenamiento de las CGANs está bien explicado, tambien se encuentran disponibles modelos ya entrenados en la carpeta *models* para poder generar imágenes tanto de prendas de vestir (imágenes 1x28x28 con generador Fully Connected) como tambien para caras expresando emociones (imágenes 3x144x144 y 1x28x28 con generador Encoder-Decoder). Estos pueden ser cargados y usados para samplear usando el notebook `Sample_images.ipynb`, el cual guía de forma intuitiva al usuario para poder samplear de su modelo.