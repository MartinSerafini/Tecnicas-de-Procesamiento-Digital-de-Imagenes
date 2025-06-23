# Segmentación de Imágenes por Color
Este cuaderno de Google Colab permite realizar una segmentación de imágenes basada en el color. El objetivo es aislar objetos o regiones de una imagen que tengan un color similar al seleccionado.

## Autor
Martin Nicolas Serafini

## Funcionalidades
El cuaderno incluye las siguientes funcionalidades:
* Selección de Color Base: Permite elegir un color base para la segmentación utilizando tres deslizadores para ajustar los pesos de los canales Rojo, Verde y Azul.
* Ajuste de Tolerancia: Permite controlar el rango de colores que se considerarán similares al color base, mediante un deslizador de tolerancia.
* Visualización de la Máscara: Muestra una máscara binaria que indica qué píxeles de la imagen original se consideran parte del segmento de color.
* Superposición de Máscara: Permite visualizar la máscara superpuesta sobre la imagen original para resaltar la región segmentada.
* Segmentación con Borde: Permite visualizar la imagen segmentada con un borde de color alrededor de la región segmentada.
* Control de Color del Borde: Permite seleccionar el color del borde que se dibuja alrededor de la región segmentada.

## Cómo Utilizar
1 Correr el cuaderno en ul entorno de Google Colab
2 Cargar la Imagen: Asegúrate de cargar la imagen que deseas segmentar en el cuaderno de Colab.
3 Interactuar con los Controles: Utiliza los controles interactivos para ajustar los parámetros de la segmentación.
  * Los deslizadores "peso_rojo", "peso_verde" y "peso_azul" permiten seleccionar el color base para la segmentación.
  * Seleccionar los valores de cada canal para realizar la segmentacion
  * El deslizador "Tolerancia" permite ajustar la tolerancia del color.
  * El desplegable "Color Borde" permite seleccionar el color del borde.
4 Observar los Resultados: El cuaderno mostrará la imagen original, la máscara binaria y la imagen segmentada con el borde, permitiéndote evaluar el resultado de la segmentación.

## Requisitos
* Python implementation: CPython
* Python version       : 3.11.12
* IPython version      : 7.34.0
* ipywidgets: 7.7.1
* numpy     : 2.0.2
* re        : 2.2.1
* IPython   : 7.34.0
* matplotlib: 3.10.0
* cv2       : 4.11.0
