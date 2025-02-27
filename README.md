# Entrega FINAL Generación de prompts
Nicolás Pereira

## Resumen
EL objetivo de este proyecto es poder generar un chatbot sobre un contexto determinado dado por el usuario a partir de documentos PDFs.

## 1.Introducción

Explicación del problema, justificación y alcance del proyecto.

## 2.Objetivos
EL objetivo de este proyecto es entrenar un modelo para luego poder generar un chatbot sobre un contexto determinado dado por el usuario a partir de documentos PDFs.

## 3.Metodología
En concreto este  proyecto se pretenden realizar tres pasos:
  - Paso 1: a partir de los PDFs de los documentos que determinan el contexto seleccionado, generar chunks que alimenten una base de datos vectorial.
 -  Paso 2: Luego mediante embedings y RAG poder generar preguntas y respuestas sobre ese contexto determinado.
 - Implementar Langchain para generar un seguimiento de las preguntas y respuestas realizadas.
 - Paso 3: Generara una interfaz con Gradio para poder acceder al prompt desde una url o genera un API para el consumo mediante REST.
 

## 4.Herramientas
 - Python
 -  OpenAI GPT-4 API
 - llama3.2
 - Langchain
 - RAG
 - Faiss
 - Embeddings
 - Gradio

## 5.Caso de prueba
Se generarán un chatbot sobre documentos de factura electrónica en PDF proporcionados por la DGI (Dirección general de impositiva).
Se realizarán consultas pertinentes al tema de facturación electrónica.
Se adjunto un jupyter notebook - chat_sobrePDF.ipynb con el caso de prueba.
El modelo sobre el que se realiza el chatbot es un llama3.2:1b - bajado de Ollama - que corre de forma local en la PC.

## 6.Entrega final
Para la entrega final se realizan pruebas con RAG sobre un modelo llama3.2:1b corriendo en modo local y con el modelo GPT-4 de OPENAI para realizar una comparativa.
Se agrega una interfaz gradio para interactuar con el prompt y además se prueban las urls de la interfaz en modo local y también la de acceso público que brinda GRADIO por 72 hs.

## 7.Comparativas de modelos
Se muestran imágenes con los tiempos y las respuestas del RAG sobre los diferentes modelos probados.
Claramente la calidad y performance de las respuestas son mejores con el modelo GPT-4 de OPENAI.

![RAG con Ollama](/rag_ollama.jpg)


