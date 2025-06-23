# Interfaz Multimodelo para Generación de Imágenes con Stable Diffusion

## Autor: 

Martin Nicolas Serafini

## Descripción

Este proyecto implementa una interfaz gráfica de usuario (GUI) interactiva utilizando la librería Gradio, diseñada para facilitar la interacción con múltiples modelos pre-entrenados de generación de imágenes basados en la arquitectura Stable Diffusion. La aplicación permite a los usuarios seleccionar entre diferentes pipelines (actualmente configurados para "Openjourney" y "Dreamlike Diffusion 1.0") y ajustar parámetros clave para generar imágenes a partir de prompts textuales.

El enfoque se centra en proporcionar una herramienta accesible para experimentar con distintos estilos de generación de imágenes ofrecidos por modelos de difusión, optimizando el proceso de inferencia mediante el uso de hardware GPU y técnicas como `torch_dtype=torch.float16` y la asignación explícita al dispositivo CUDA.

## Funcionalidad

La interfaz permite:

*   **Seleccionar el Modelo de Generación:** Elegir entre los pipelines de Stable Diffusion disponibles (ej. Openjourney, Dreamlike Diffusion 1.0).
*   **Definir Prompts:** Especificar un prompt textual principal para guiar la generación de la imagen.
*   **Definir Prompt Negativo:** Opcionalmente, especificar un prompt negativo para indicar conceptos o características a evitar en la imagen generada.
*   **Controlar el Guidance Scale:** Ajustar la influencia del prompt en el proceso de difusión. Un valor más alto generalmente resulta en una imagen más cercana al prompt.
*   **Configurar el Número de Pasos de Inferencia:** Definir la cantidad de iteraciones del proceso de difusión. Un mayor número de pasos puede mejorar la calidad pero aumenta el tiempo de generación.
*   **Establecer una Semilla Aleatoria (Seed):** Asegurar la reproducibilidad de las imágenes generadas al fijar la semilla del generador aleatorio.
*   **Visualizar la Imagen Generada:** Mostrar la imagen resultante directamente en la interfaz.

## Requisitos

*   Python 3.7 o superior.
*   Entorno con acceso a una GPU compatible con CUDA (recomendado para un rendimiento óptimo). Google Colab con aceleración por hardware (GPU) es un entorno ideal.

## Instalación y Uso

### 1. Clonar el Repositorio
Clona este repositorio en tu entorno local o en Google Colab:
### 2. Ejecutar el Código
Si estás utilizando Google Colab o un entorno Jupyter Notebook, simplemente ejecuta las celdas del notebook en secuencia.
Si estás ejecutando el código como un script Python (`.py`), ejecuta el archivo desde tu terminal:
Asegúrate de que tu script contenga el código proporcionado en el proyecto.
### 3. Interfaz de Usuario
Una vez que el script se ejecute y los modelos se carguen, Gradio lanzará la interfaz de usuario. Si estás en Colab, te proporcionará un enlace local y, opcionalmente, un enlace público. Si estás ejecutando localmente, abrirá una pestaña en tu navegador por defecto o te proporcionará una URL local.
Interactúa con la interfaz seleccionando el modelo, ingresando los prompts y ajustando los parámetros. Haz clic en el botón "Generar Imagen" para iniciar el proceso de inferencia y visualizar el resultado.

## Estructura del Código

El código está organizado en las siguientes secciones clave:

*   **Instalación de Dependencias:** Comandos pip para instalar las librerías requeridas.
*   **Importación de Librerías:** Importación de módulos como `torch`, `gradio`, `PIL`, y `diffusers`.
*   **Verificación de GPU:** Código para asegurar que una GPU esté disponible, crucial para el rendimiento.
*   **Carga de Modelos:** Carga de los pipelines de Stable Diffusion ("Openjourney" y "Dreamlike Diffusion 1.0") desde Hugging Face Hub, utilizando optimizaciones para GPU (`float16`, `.to("cuda")`).
*   **Función de Generación de Imágenes:** Definición de la función `generar_imagen` que toma los parámetros de la interfaz y realiza la inferencia con el modelo seleccionado. Incluye manejo de semillas para reproducibilidad.
*   **Configuración de la Interfaz Gradio:** Definición de los componentes de la interfaz (textboxes, sliders, dropdown, botón, imagen de salida) y la lógica para vincular los eventos del botón con la función de generación.
*   **Lanzamiento de la Interfaz:** Inicio del servidor Gradio para hacer que la interfaz sea accesible.

## Modelos Utilizados

*   **Openjourney:** Un modelo de Stable Diffusion entrenado para generar imágenes con un estilo similar a las creaciones de Midjourney.
*   **Dreamlike Diffusion 1.0:** Un modelo que tiende a generar imágenes con un estilo detallado y onírico.

Ambos modelos son cargados desde el Hugging Face Hub, optimizados para inferencia en GPU.
