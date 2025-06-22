# Interpolación de Imágenes con PIL

Este cuaderno de Google Colab explora diferentes métodos de interpolación de imágenes usando la biblioteca PIL (Pillow). Permite a los usuarios experimentar con cómo se redimensionan las imágenes y cómo se ven afectadas por los distintos algoritmos de interpolación.

## Autor

Martin Nicolas Serafini

## Funcionalidades
El cuaderno incluye las siguientes funcionalidades:
* Rotación de Imagen: Permite rotar la imagen cargada un ángulo específico.
* Selección de Método de Interpolación: Permite elegir entre tres métodos de interpolación diferentes para la rotación:
  * NEAREST: Interpolación de vecino más cercano.
  * BILINEAR: Interpolación bilineal.
  * BICUBIC: Interpolación bicúbica.
* Visualización de Resultados: Muestra la imagen original y la imagen rotada con el método de interpolación seleccionado para comparar los resultados.
* Control Interactivo: El cuaderno proporciona controles interactivos (un deslizador y un menú desplegable) para ajustar el ángulo de rotación y el método de interpolación en tiempo real.

## Cómo Utilizar
* Usar en Google Colab
* Acceder al Cuaderno: Si tienes el archivo `.ipynb` (como "INTERPOLACION_CON_PIL_Martin_Nicolas_Serafini.ipynb"), sube el archivo a tu Google Drive. Luego, abre Google Colab y sube el archivo desde tu Google Drive.
* Ejecutar las Celdas: Una vez que el cuaderno está abierto en Google Colab, puedes ejecutar las celdas de código una por una presionando `Shift` + `Enter`, o puedes ejecutar todas las celdas a la vez usando la opción "Ejecutar todo" en el menú "Entorno de ejecución".
* Interactuar con los Controles: Utiliza los controles interactivos para experimentar con los diferentes métodos de interpolación.
  * El deslizador "Ángulo (°)" permite ajustar el ángulo de rotación de la imagen.
  * El menú desplegable "Método Rot:" permite seleccionar el método de interpolación a utilizar.
* Los resultados se mostrarán en tiempo real en el cuaderno.

## Descargar el Cuaderno
* Descargar desde Google Colab: Si estás viendo el cuaderno en Google Colab, puedes descargarlo yendo al menú "Archivo" y seleccionando "Descargar" -> "Descargar el archivo .ipynb".
* Descargar desde GitHub: Si el cuaderno está alojado en un repositorio de GitHub, puedes descargarlo directamente desde allí. Haz clic en el archivo `.ipynb` y luego en el botón "Descargar".

## Requisitos
* Google Colab
* PIL (Pillow)
* ipywidgets
* skimage
* matplotlib
* numpy
* pandas

## Instrucciones Adicionales
* Asegúrate de cargar una imagen en el cuaderno para poder experimentar con las funcionalidades.
* El cuaderno está diseñado para ser interactivo, así que no dudes en jugar con los controles para ver cómo afectan los resultados.
* Puedes modificar el código en las celdas para personalizar aún más el procesamiento de imágenes.

