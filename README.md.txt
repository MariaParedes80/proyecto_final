# Reporte de Análisis del Dataset del Titanic con Agente IA (Local LLM)

Este repositorio contiene la arquitectura de código completa para el informe interactivo del Titanic. El proyecto implementa una solución híbrida de análisis estadístico tradicional asistida por Inteligencia Artificial en un entorno privado.

##  Enlace del Proyecto de Entrega
* **Aplicación en Vivo en la Nube:** [https://streamlit.app](https://streamlit.app)

##  Tecnologías y Arquitectura
* **Frontend y Tableros:** `Streamlit` para la orquestación de la interfaz gráfica y filtros automáticos.
* **Procesamiento de Datos:** `Pandas` para la carga y cálculos en caliente sobre la matriz del archivo `dataset.csv`.
* **Gráficos Estadísticos:** `Matplotlib` enfocado en la distribución dinámica de variables cuantitativas y cualitativas.
* **Motor del Agente de IA:** Integración local mediante **`Ollama`**, asegurando un procesamiento semántico de consultas en lenguaje natural con total privacidad de datos comerciales (sin consumo de APIs externas de terceros).

##  Estructura Principal del Proyecto
* `app.py`: Archivo core de la aplicación que administra las métricas de la interfaz, lógicas `if/elif` prioritarias para la segmentación de prompts y gráficos interactivos.
* `dataset.csv`: Base de datos origen que almacena la matriz de 891 registros de pasajeros del Titanic.
* `requirements.txt`: Archivo de configuración que contiene las dependencias del ecosistema Python necesarias para el correcto despliegue del servidor.

##  Capacidades del Modelo Evaluadas en el Video de Entrega
El agente de IA responde eficientemente y de forma parametrizada a consultas críticas de negocio, tales como:
1. **Auditoría de Dimensiones:** Extracción en vivo del tamaño exacto de la matriz (891 registros × 12 columnas).
2. **Cálculo de Tasa Macroeconómica/Supervivencia:** Análisis dinámico del porcentaje general de personas rescatadas (38.38%).
3. **Análisis Demográfico:** Correlación estadística basada en políticas de evacuación por variables de género.
