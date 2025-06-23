# Detección de Rostros y Landmarks Faciales

## Autor: 

Serafini, Martin Nicolas

## Descripción
Este cuaderno de Google Colab demuestra la aplicación de técnicas de visión por computadora para la detección de rostros y la identificación de puntos faciales clave (landmarks). El cuaderno combina dos métodos principales:

Detección de Rostros: Utiliza el método de Haar Cascades para localizar múltiples rostros dentro de una imagen.

Detección de Landmarks Faciales: Aplica el algoritmo LBF (Local Binary Features) para identificar 68 puntos clave específicos en cada rostro detectado (ojos, cejas, nariz, boca, mandíbula).

Además, el cuaderno incluye una funcionalidad para la detección de bostezo basada en el análisis de los puntos faciales detectados.

## Objetivo
El objetivo de este cuaderno es proporcionar una guía práctica para implementar la detección de rostros y puntos faciales clave, y mostrar cómo estas técnicas se pueden utilizar en una aplicación como la detección de bostezo.

## Funcionalidades
El cuaderno incluye las siguientes funcionalidades:

* Detección de Rostros: Utiliza Haar Cascades para detectar la ubicación de rostros en una imagen.
* Detección de Puntos Faciales Clave: Identifica 68 puntos faciales clave en cada rostro detectado utilizando el algoritmo LBF.
* Detección de Bostezo: Calcula el Mean Aspect Ratio (MAR) de los ojos y utiliza un umbral para determinar si una persona está bostezando.
* Visualización: Muestra la imagen original con los rostros detectados y los puntos faciales clave superpuestos. También indica si se detecta bostezo.

## Cómo utilizar
Requisitos
* Google Colab
* OpenCV (cv2)
* Matplotlib
* dlib

## Instalación
* Instalar OpenCV: El cuaderno incluye comandos para desinstalar cualquier versión existente de OpenCV e instalar la versión que incluye los módulos contrib, necesarios para la detección de landmarks faciales.
* Instalar dlib: El cuaderno incluye un comando para instalar la librería dlib, necesaria para la detección de landmarks faciales con el algoritmo LBF.
* Descargar recursos: El cuaderno descarga los siguientes archivos necesarios:
  * Clasificador Haar para la detección de rostros (haarcascade_frontalface_default.xml).
  * Modelo pre-entrenado LBF para la detección de landmarks faciales (lbfmodel.yaml).

## Instrucciones
* Abrir en Google Colab:
* Si tienes el archivo .ipynb, súbelo a tu Google Drive. Luego, abre Google Colab y sube el archivo desde tu Google Drive.
* Ejecutar las celdas:
* Después de ejecutar la celda de instalación de OpenCV, REINICIA EL ENTORNO DE EJECUCIÓN (Entorno de ejecución -> Reiniciar entorno de ejecución...). Luego, vuelve a ejecutar todas las celdas desde el principio.
* Visualizar los resultados:
  * El cuaderno cargará una imagen de ejemplo y aplicará la detección de rostros y puntos faciales clave.
  * Los resultados se mostrarán utilizando Matplotlib, mostrando la imagen original con los rostros detectados y los puntos faciales clave superpuestos, e indicando si se detecta bostezo.
  * El cuaderno también procesa una serie de imágenes de prueba para demostrar la detección de bostezo en diferentes escenarios.

## Notas importantes
* Reinicio del entorno de ejecución: Es crucial reiniciar el entorno de ejecución después de instalar OpenCV para que los cambios se apliquen correctamente.
* Descarga de recursos: El modelo LBF para landmarks faciales es un archivo grande y puede tardar un poco en descargarse.
* Uso de la GPU: Si tienes acceso a una GPU en Google Colab, puedes habilitarla para acelerar el procesamiento, especialmente la detección de landmarks faciales.
