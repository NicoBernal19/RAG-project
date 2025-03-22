# RAG-project

## Hecho por: Nicolas Bernal

Este repositorio contiene un cuaderno en Colab que implementa un RAG utilizando bibliotecas como langchain, pinecone y OpenAI. El proyecto está diseñado para guiar al usuario a través de la configuración del entorno, la carga y procesamiento de datos, y la construcción de un modelo RAG para tareas de respuesta a preguntas.

## Estructura del Proyecto

1. Configuración del Entorno

Se instalan las bibliotecas necesarias, como langchain, pinecone O OpenAI.

![image](https://github.com/user-attachments/assets/eb8a0fac-b80d-447e-b8de-7cdb8c637ba2)

![image](https://github.com/user-attachments/assets/9873e974-29eb-4d7c-8ef4-4ea418f2947c)

Se configuran las claves de API para OpenAI y Pinecone.

![image](https://github.com/user-attachments/assets/4c021e7e-8b0a-4764-bbce-3a9b39ee2d11)

![image](https://github.com/user-attachments/assets/072bba74-51ab-4c1d-b038-201746dfeffd)

2. Carga y Procesamiento de Datos
   
Se utiliza WebBaseLoader para cargar contenido de un blog y dividirlo en fragmentos manejables utilizando RecursiveCharacterTextSplitter.

Los fragmentos se indexan en una base de datos vectorial para permitir búsquedas eficientes.

![image](https://github.com/user-attachments/assets/0a5b9096-9b4f-4409-afc0-d6300d3cd5d4)

3. Construcción del Modelo RAG
   
Se define un flujo de trabajo que combina la recuperación de información relevante y la generación de respuestas utilizando un modelo de lenguaje en este caso gpt-4.

4. Interacción con el Modelo

El usuario puede hacer preguntas, y el sistema recupera información relevante de la base de datos vectorial para generar respuestas precisas.

## Arquitectura

![image](https://github.com/user-attachments/assets/24188afc-c4db-49a9-9142-e262aba3844d)

## Instalacion y Ejecucion

Toma el archivo .ipynb y usalo para cargar el notebook en colab.

### Instala las dependencias:

- pip install --quiet --upgrade langchain-text-splitters langchain-community langgraph
- pip install -qU "langchain[openai]"
- pip install -qU langchain-pinecone
- pip install -qU langchain-pinecone pinecone-notebooks

### Configura la API de OpenAI

Necesitas configurar tu clave API de OpenAI, en este caso nosotros recibimos la clave de parte del profesor.

### Registrarse en pinecone para obtener la clave

Debes registrarte en pinecone para poder obtener la clave que va a ser necesaria.

### Sigue las instrucciones del Notebook

Ejecuta el resto de celdas del notebook para que el programa funcione correctamente.

## Ejemplo en accion

![image](https://github.com/user-attachments/assets/ee536f32-caec-47ca-9f0d-63d0dbd54e2b)


![image](https://github.com/user-attachments/assets/8515f2d8-3ecf-4597-85d5-e002fd8a9304)

![image](https://github.com/user-attachments/assets/3c9ef20e-2615-4128-88a4-dad679d90eb9)

![image](https://github.com/user-attachments/assets/800f0a77-2595-424e-8a82-3162c796eaac)


