# AI TOMATE - Proyecto de Identificación de Enfermedades en Plantas Tomateras

![AITomate](tomate.png)

<iframe width="560" height="315" src="https://www.youtube.com/embed/-hkiuVaWwbY?si=_9lvvgQti4krj1Ro" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Descripción General

**AI TOMATE** AI TOMATE: Innovación en la Agricultura del Futuro

AI TOMATE es un proyecto revolucionario que se sitúa en la intersección de la Industria 4.0 y la agricultura. Utilizando tecnologías de vanguardia como drones, visión artificial y técnicas de aprendizaje automático, AI TOMATE está redefiniendo la forma en que cuidamos y protegemos nuestras plantas de tomate.

Visión General del Proyecto

El objetivo principal de AI TOMATE es la identificación temprana de enfermedades en las plantas de tomate. Para lograr esto, el proyecto utiliza una combinación de visión por computadora y técnicas de aprendizaje automático para analizar imágenes de plantas de tomate y diagnosticar posibles enfermedades.

## El sistema se compone de varios componentes clave:

Aplicación web para la captura de imágenes: Esta aplicación permite a los usuarios capturar y subir imágenes de sus plantas de tomate para su análisis.

## API para el procesamiento de imágenes: Una vez que las imágenes son capturadas, son procesadas a través de esta API, que utiliza algoritmos avanzados de visión por computadora para analizar las imágenes.

## Red neuronal para la detección de enfermedades: Las imágenes procesadas son luego analizadas por una red neuronal, que ha sido entrenada para detectar una variedad de enfermedades comunes en las plantas de tomate.

### LLM (Lifelong Learning Machines): Este componente se utiliza para obtener una descripción más detallada de la planta afectada, permitiendo un diagnóstico más preciso y una intervención más temprana.

## AI TOMATE representa un avance significativo en la agricultura del futuro. Al combinar la tecnología de drones con la inteligencia artificial, este proyecto ofrece una solución innovadora y eficaz para el cuidado y la protección de las plantas de tomate. Con AI TOMATE, el futuro de la agricultura es más brillante y más sostenible que nunca.

## Instalación

1. Clona el repositorio:

    ```sh
    git clone https://github.com/FernanMoreno/AITomato.git
    cd tomato
    ```

2. Instala las dependencias:

    ```sh
    pip install -r requirements.txt
    ```

3. Configura Git LFS para manejar archivos grandes:

    ```sh
    git lfs install
    git lfs pull
    ```

4. Instala Ollama y el modelo llava-phi3:

    ```sh
    ollama run llava-phi3
    ```

## Uso

1. Ejecuta la API:

    ```sh
    uvicorn app:app --reload
    ```

2. Captura una imagen con el dron:

    ```sh
    streamlit run capture_streamlit.py
    ```

3. La imagen se enviará automáticamente a la API y el resultado de la detección se mostrará en la webapp.

## Estructura del Proyecto

- `app.py`: API de FastAPI que conecta con el modelo para procesar las imágenes.
- `best_model.weights.h5`: Archivo de pesos del modelo entrenado.
- `resnet50_model.h5`: Archivo del modelo.
- `capture_streamlit.py`: Script de streamlit para poder visualizar las detecciones en las imágenes con el dron.
- `modeloTomates_version2.ipynb`: Notebook de Jupyter con el modelo de detección de enfermedades.
- `llm_multimodal.py`: Ruta de la API al LLM multimodal.
- `model_predict.py`: Ruta de la API al modelo de las predicciones.
- `upload.py`: Ruta de la API para subir las imagenes.
- `dataset-optimizado.zip`: El dataset con el que se entreno el modelo de deteccion de enfermedades.

## Documentación directa de nuestro proyecto:

Puede entender mas sobre nuestro proyecto leyendo la documentación hecha: [AITomate Documentation](https://www.notion.so/Documentaci-n-AITomate-85595b4da73b471ba6943edbed4daa41?pvs=4)

## Contribuciones

Las contribuciones son bienvenidas. Por favor, crea un fork del proyecto y envía un pull request con tus mejoras.


## Contacto

Para preguntas o sugerencias, por favor abre un issue en el repositorio o contacta a fernandojosemolinamore@gmail.com, isaacripoll@gmail.com, susana-aranda@outlook.es, jquijado@gmail.com y victor.arbiol@gmail.com.
