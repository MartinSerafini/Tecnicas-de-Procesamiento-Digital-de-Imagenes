# Análisis de Imágenes a Color con OpenCV

Este cuaderno de Google Colab permite realizar un análisis interactivo de imágenes a color utilizando la biblioteca OpenCV. Proporciona herramientas para explorar las propiedades de los canales de color, realizar conversiones de espacio de color y aplicar procesamiento de imágenes como la detección de bordes de Canny.

## Autor

Martin Nicolas Serafini

## Funcionalidades

El cuaderno incluye las siguientes funcionalidades:

* **Visualización de Recortes de Imagen:** Permite seleccionar una región rectangular de la imagen mediante sliders para analizar una porción específica[cite: 1].
* **Conversión a RGB:** Convierte la imagen al espacio de color RGB, útil para asegurar la compatibilidad con otras bibliotecas o para visualizar la imagen en este espacio de color[cite: 1].
* **Análisis de Canales de Color:** Calcula y muestra los valores mínimo, máximo y promedio de los canales de color (Azul, Verde y Rojo) de la imagen[cite: 32].
* **Aplicación de Mapas de Color:** Aplica diferentes mapas de color a la imagen para realzar ciertas características o para visualización[cite: 1].
* **Detección de Bordes con Canny:** Implementa el algoritmo de Canny para la detección de bordes en la imagen, con controles para ajustar los umbrales[cite: 1].
* **Filtro Gaussiano:** Permite aplicar un filtro Gaussiano para suavizar la imagen antes de la detección de bordes, reduciendo el ruido[cite: 1].
* **Control de Bordes:** Ofrece la opción de modificar el tipo de borde utilizado al aplicar el filtro Gaussiano[cite: 1].

## Cómo Utilizar

1.  Correr el cuaderno en el entorno de Google Colab 
2.  **Cargar la Imagen:** Asegúrate de cargar la imagen que deseas analizar en el cuaderno de Colab.
3.  **Interactuar con los Controles:** Utiliza los sliders y checkboxes para ajustar los parámetros de las diferentes funcionalidades.
    * Los sliders `x1`, `y1`, `x2`, `y2` permiten seleccionar la región de interés de la imagen.
    * El checkbox "Convertir a RGB" activa la conversión de la imagen a RGB.
    * El checkbox "Mapas de Color" aplica un mapa de color a la imagen.
    * El checkbox "Aplicar Canny" activa la detección de bordes de Canny, y los sliders "Umbral\_Inf" y "Umbral\_Sup" ajustan los umbrales del algoritmo.
    * El checkbox "Aplicar Gauss" activa el filtro Gaussiano, y los sliders "kernel" y "sigma" ajustan el tamaño del kernel y la desviación estándar del filtro.
    * El dropdown "Border Type" permite seleccionar el tipo de borde para el filtro Gaussiano.
4.  **Observar los Resultados:** Los resultados del procesamiento y análisis se mostrarán en la salida del cuaderno, incluyendo la imagen procesada y las estadísticas de los canales de color[cite: 32].

## Requisitos

* Python implementation: CPython
* Python version       : 3.11.12
* ipywidgets: 7.7.1
* numpy     : 2.0.2
* re        : 2.2.1
* IPython   : 7.34.0
* matplotlib: 3.10.0
* cv2       : 4.11.0
