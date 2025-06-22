# Muestreo y Cuantización de Imágenes

Este cuaderno de Google Colab permite explorar los efectos del muestreo y la cuantización en imágenes digitales.  A través de controles interactivos, se puede ajustar la resolución de la imagen y la cantidad de niveles de color para observar cómo estos parámetros afectan la calidad visual.

## Autor 

Martin Nicolas Serafini

## Funcionalidades

El cuaderno incluye las siguientes funcionalidades:

* **Selección de Canal de Color:** Permite elegir entre los canales Rojo, Verde y Azul de la imagen para aplicar el muestreo y la cuantización.
* **Ajuste de Muestreo:** Permite controlar la tasa de muestreo de la imagen, determinando cuántos píxeles se retienen. Se puede seleccionar entre factores de muestreo de 1, 2, 4, 8, 16 y 32.* **Ajuste de Cuantización:** Permite controlar la cantidad de niveles de cuantización, lo que afecta la cantidad de colores distintos que pueden representarse en la imagen. Se puede seleccionar entre 1, 2, 4, 8, 16, 32, 64 y 128 niveles.
* **Aplicación Combinada:** Ofrece la opción de aplicar muestreo y cuantización simultáneamente para observar el efecto combinado de ambos procesos.
* **Visualización de Resultados:** Muestra la imagen original y la imagen procesada (muestreada y/o cuantizada) para comparar los resultados.

## Cómo Utilizar

1.  Correr el cuaderno en el entorno de Google Colab.
2.  **Cargar la Imagen:** Asegúrate de cargar la imagen que deseas procesar en el cuaderno de Colab.
3.  **Interactuar con los Controles:** Utiliza los desplegables y el checkbox para ajustar los parámetros:
    * **Canal:** Selecciona el canal de color a procesar (Rojo, Verde o Azul).
    * **Muestreo (p):** Elige el factor de muestreo.
    * **Cuantific. (q):** Elige la cantidad de niveles de cuantización.
    * **Muestreo + Cuantificación:** Activa esta opción para aplicar ambos procesos simultáneamente.
4.  **Observar los Resultados:** El cuaderno mostrará la imagen original y la imagen resultante después de aplicar el muestreo y/o la cuantización, permitiéndote evaluar el impacto de los parámetros seleccionados.

## Requisitos

* Python implementation: CPython
* Python version       : 3.11.12
* IPython version      : 7.34.0
* ipywidgets: 7.7.1
* matplotlib: 3.10.0
* cv2       : 4.11.0
* re        : 2.2.1
* numpy     : 2.0.2
