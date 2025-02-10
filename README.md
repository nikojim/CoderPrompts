# Entrega Generación de prompts
Nicolás Pereira

## Resumen
EL objetivo de este proyecto es poder generar un chatbot sobre un contexto determinado dado por el usuario a partir de documentos PDFs.

## 1.Introducción

Explicación del problema, justificación y alcance del proyecto.

## 2.Objetivos
EL objetivo de este proyecto es entrenar un modelo para luego poder generar un chatbot sobre un contexto determinado dado por el usuario a partir de documentos PDFs.

## 3.Metodología
En concreto este  proyecto se pretenden realizar tres pasos:
 -  Paso 1: realizar un fine tuning y entrenamiento de un modelo con ciertas preguntas y respuestas frecuentes sobre el contexto dado.
 - Paso 2: a partir de los PDFs de los documentos que determinan el contexto seleccionado, generar chunks que alimenten una base de datos vectorial.
 -  Paso 3: Luego mediante embedings y RAG poder generar preguntas y respuestas sobre ese contexto determinado.
 - Implementar Langchain para generar un seguimiento de las preguntas y respuestas realizadas.
 - Paso 4: Generara una interfaz con Gradio para poder acceder al prompt desde una url o genera un API para el consumo mediante REST.
 

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

## 6.Propuesta para la entrega final
Se realizarán los pasos 1 y 4 de la metodología descrita en el punto 3 que quedaron pendientes.
Se probará sobre otro modelo -chatGPT de OPENAI - para comparar performance y correctitud de las respuestas.
