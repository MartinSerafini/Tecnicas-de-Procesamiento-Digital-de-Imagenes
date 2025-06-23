# Detección de Bordes y Objetos / Comparativa: Scikit-Image, Sobel, Prewitt y YOLOv5

Este cuaderno de Google Colab compara diferentes métodos de detección de bordes en imágenes, incluyendo los métodos clásicos de Sobel y Prewitt, las funcionalidades de detección de bordes de Scikit-Image y un enfoque basado en un modelo de detección de objetos (YOLOv5).

## Autor

Martin Nicolas Serafini

## Funcionalidades

El cuaderno incluye las siguientes funcionalidades:
* Carga de Imagen: Permite cargar una imagen para realizar la detección de bordes.
* Detección de Bordes con Sobel: Aplica el operador Sobel para detectar bordes en la imagen.
* Detección de Bordes con Prewitt: Aplica el operador Prewitt para detectar bordes en la imagen.
* Detección de Bordes con Scikit-Image: Utiliza las funciones de detección de bordes de la biblioteca Scikit-Image.
* Detección de Bordes con YOLOv5: Utiliza un modelo YOLOv5 pre-entrenado para detectar objetos y sus contornos en la imagen.
  * Se prueba la funcionalidad de reconocimiento óptico de caracteres (OCR) sobre una imagen, con el objetivo de extraer y retornar una cadena de texto correspondiente a la patente vehicular detectada. 
* Visualización Comparativa: Muestra los resultados de cada método de detección de bordes uno al lado del otro para facilitar la comparación visual.
* Control Interactivo: El cuaderno proporciona controles interactivos para ajustar los parámetros de los diferentes métodos de detección de bordes.

## Cómo Utilizar
* Usar en Google Colab
* Acceder al Cuaderno: Si tienes el archivo Deteccion_de_Bordes_Comparativo_Scikit_Image,_Sobel_Prewitt_YOLOv5_Martin_Nicolas_Serafini.ipynb", sube el archivo a tu Google Drive. Luego, abre Google Colab y sube el archivo desde tu Google Drive.
* Ejecutar las Celdas: Una vez que el cuaderno está abierto en Google Colab, puedes ejecutar las celdas de código una por una presionando `Shift` + `Enter`, o puedes ejecutar todas las celdas a la vez usando la opción "Ejecutar todo" en el menú "Entorno de ejecución".
* Interactuar con los Controles: Utiliza los controles interactivos para experimentar con los diferentes métodos de detección de bordes y sus parámetros. Los resultados se mostrarán en tiempo real en el cuaderno.

## Descargar el Cuaderno
* Descargar desde Google Colab: Si estás viendo el cuaderno en Google Colab, puedes descargarlo yendo al menú "Archivo" y seleccionando "Descargar" -> "Descargar el archivo .ipynb".
* Descargar desde GitHub: Si el cuaderno está alojado en un repositorio de GitHub, puedes descargarlo directamente desde allí. Haz clic en el archivo `.ipynb` y luego en el botón "Descargar".

## Requisitos
* Google Colab
* OpenCV (cv2)
* Scikit-image
* Pillow
* YOLOv5
* Torch
* pytesseract
  
Instrucciones Adicionales
* Asegúrate de cargar una imagen en el cuaderno para poder experimentar con las funcionalidades.
* El cuaderno está diseñado para ser interactivo, así que no dudes en jugar con los controles para ver cómo afectan los resultados.
* Ten en cuenta que la detección de bordes con YOLOv5 requiere la descarga de un modelo pre-entrenado, lo que puede llevar algún tiempo, en caso de que las funcionalidades del cuaderno se detengan, interrumpir la sesion y volver a ejecutarlo desde el inicio.
