# Agente-Inteligente-Carrarurqu-a-RAG-Web-Search-
Este proyecto fue desarrollado en el marco de la Inmersión IA Dev, utilizando como base los documentos proporcionados durante el curso para la empresa ficticia "Carrarurquía".
El sistema consiste en un agente de inteligencia artificial que emplea una arquitectura de enrutamiento dinámico mediante LangGraph, lo que le permite decidir en tiempo real qué fuente de información utilizar según el tipo de consulta:

RAG (Retrieval-Augmented Generation): Para responder preguntas relacionadas con información interna de la empresa, como paquetes turísticos o políticas, utilizando una base de datos vectorial local.

Búsqueda Web: Para consultas generales o información actualizada, redirigiendo la pregunta hacia internet a través de SerpAPI.

🏆 Desafío Final y Experiencia de Usuario (UX)

Como parte del reto final de la inmersión, el proyecto incorpora mejoras que van más allá de una simple salida en consola:

Exportación automática en dos formatos: Las respuestas generadas se procesan y se descargan automáticamente en archivos Markdown (.md) y PDF (.pdf), listos para su uso y distribución.

Interfaz interactiva: Se implementó una experiencia de usuario dinámica mediante una interfaz de línea de comandos (CLI), donde el usuario puede ingresar preguntas en lenguaje natural. Además, el sistema genera nombres de archivo seguros y limpios a partir de cada consulta (sanitización de strings).

🚀 Características Principales

Ruteo inteligente con LangGraph: Clasifica automáticamente las consultas para decidir entre base de datos local o búsqueda web.

Procesamiento de documentos: Permite cargar archivos PDF, analizarlos y dividirlos semánticamente para mejorar la recuperación de información.

Control de alucinaciones: Uso de técnicas de prompt engineering para asegurar que las respuestas se basen estrictamente en los documentos disponibles, evitando la invención de datos.

🛠️ Stack Tecnológico

Lenguaje: Python 3

Modelo LLM: Google Gemini 2.5 Flash

Orquestación: LangChain y LangGraph

Base vectorial: FAISS (Facebook AI Similarity Search)

Embeddings: Google Generative AI (gemini-embedding-001)

Procesamiento y exportación: pypdf, fpdf2, markdown

💻 Cómo ejecutar el proyecto

Haz clic en "Open in Colab" en la parte superior del documento.

Dentro de Colab, abre el panel lateral y selecciona la sección de Secrets / userdata.

Configura tus credenciales de forma segura (no se expondrán en el código):

GEMINI_API_KEY: Clave de Google AI Studio

SERPAPI_API_KEY: Clave de SerpAPI

Sube los archivos PDF correspondientes a la inmersión de "Carrarurquía".

Ejecuta todas las celdas en orden.

En la última celda, podrás interactuar con el agente mediante el prompt.

👨‍💻 Autor

L9TDeveloper
