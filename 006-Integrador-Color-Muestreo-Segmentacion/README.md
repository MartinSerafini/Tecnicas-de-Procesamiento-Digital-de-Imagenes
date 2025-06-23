# Integrador - Procesamiento de Imágenes

Este cuaderno de Google Colab contiene un ejercicio integrador que aplica varias técnicas de procesamiento de imágenes utilizando la biblioteca OpenCV. El ejercicio permite a los usuarios experimentar con el filtrado de imágenes, la detección de bordes y la segmentación de color.

## Autor

Martin Nicolas Serafini

## Funcionalidades

El cuaderno incluye las siguientes funcionalidades:
  * Filtrado de Imagen: Permite aplicar filtros de suavizado a la imagen, como el filtro Gaussiano, para reducir el ruido.
  * Detección de Bordes: Implementa el algoritmo de Canny para detectar los bordes en la imagen filtrada.
  * Segmentación de Color: Permite segmentar la imagen por color, aislando regiones que coinciden con un rango de color definido por el usuario.
  * Control Interactivo: El cuaderno proporciona controles interactivos (sliders y desplegables) para ajustar los parámetros de cada una de estas funcionalidades en tiempo real.

## Cómo Utilizar

Se debe correr el cuaderno desde el entorno de Google Colab. 

  * Acceder al Cuaderno: Puedes abrir el cuaderno directamente en Google Colab usando este enlace: [Enlace al Cuaderno de Colab] (Reemplazar con el enlace real si está disponible). Si tienes el archivo `.ipynb` (como  "TPDI_Ejercicio_Integrador.ipynb"), sube el archivo a tu Google Drive. Luego, abre Google Colab y sube el archivo desde tu Google Drive.
    
  * Ejecutar las Celdas: Una vez que el cuaderno está abierto en Google Colab, puedes ejecutar las celdas de código una por una presionando `Shift` + `Enter`, o puedes ejecutar todas las celdas a la vez usando la opción "Ejecutar todo" en el menú "Entorno de ejecución".
    
  * Interactuar con los Controles: Utiliza los controles interactivos para experimentar con los diferentes parámetros de procesamiento de imágenes. Los resultados se mostrarán en tiempo real en el cuaderno.
   
## Requisitos
  * Python implementation: CPython
  * Python version       : 3.11.12
  * IPython version      : 7.34.0
  * skimage   : 0.25.2
  * google    : 2.0.3
  * numpy     : 2.0.2
  * cv2       : 4.11.0
  * matplotlib: 3.10.0
  * PIL       : 11.1.0
  * ipywidgets: 7.7.1

## Instrucciones Adicionales
* Asegúrate de tener una imagen cargada en el cuaderno para poder experimentar con las funcionalidades.
* El cuaderno está diseñado para ser interactivo, así que no dudes en jugar con los controles para ver cómo afectan los resultados.
