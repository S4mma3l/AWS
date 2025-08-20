# Introducción a Amazon Bedrock

## ¿Qué es Amazon Bedrock?

**Amazon Bedrock** es un servicio completamente gestionado de AWS que proporciona acceso a **modelos fundacionales (FM)** de los principales proveedores de IA a través de una API unificada. Permite crear y escalar aplicaciones de **IA generativa** sin necesidad de gestionar la infraestructura subyacente.

---

## Funcionalidad Principal de Amazon Bedrock

### Acceso a Modelos
Amazon Bedrock ofrece un acceso integral a modelos de IA desarrollados por AWS y otros proveedores líderes.

* **Modelos de AWS**:
    * **Amazon Nova**: Serie de modelos multimodales y de texto con diferentes capacidades:
        * _Nova Micro_: Modelo de solo texto para respuestas de baja latencia.
        * _Nova Lite_: Modelo multimodal rentable para entradas de imagen, video y texto.
        * _Nova Pro_: Modelo multimodal que equilibra precisión, velocidad y costo.
        * _Nova Premier_: El modelo multimodal más avanzado para tareas complejas.
        * _Nova Canvas_: Generador de imágenes rentable con funciones de edición.
        * _Nova Reel_: Generador de videos a partir de texto e imágenes.
        * _Nova Sonic_: Modelo de voz de baja latencia para conversaciones en tiempo real.
    * **Amazon Titan**: Familia de modelos entrenados en conjuntos de datos seleccionados por AWS.
* **Modelos de Terceros**: Acceso a modelos de empresas como **Anthropic**, **AI21 Labs**, **Cohere**, **Meta** y **Stability AI**.

### Personalización del Modelo
Amazon Bedrock facilita la personalización de modelos sin necesidad de conocimientos profundos en ML.

* **Ajuste Fino**: Adapta modelos al estilo y terminología de su organización.
* **Generación Aumentada por Recuperación (RAG)**: Mejora las respuestas de los modelos al recuperar información relevante de fuentes de datos propietarias.

---

## Conceptos Técnicos Clave

| Concepto Técnico | Descripción |
| :--- | :--- |
| **Modelo de Fundación (FM)** | Modelos de IA a gran escala, versátiles, que sirven como base para aplicaciones de IA generativa. Pueden ser de texto, imagen o embeddings. |
| **Tokens y Límites de Tokens** | Los tokens son las unidades de texto que procesan los modelos. Cada modelo tiene un límite de tokens para las entradas y salidas, lo que afecta los costos y el diseño de los _prompts_. |
| **Ingeniería de Prompts** | El arte de crear instrucciones efectivas para los modelos. La calidad de la respuesta depende de la estructura y formulación del _prompt_. |
| **Parámetros de Inferencia** | Ajustes que controlan cómo los modelos generan respuestas, como _temperatura_ (aleatoriedad) y _top-p_ (selección de tokens). |
| **RAG** | Técnica que mejora los resultados de los modelos al incorporar información de fuentes de conocimiento externas, sin necesidad de reentrenamiento. |
| **Evaluación del Modelo** | Proceso para evaluar sistemáticamente el rendimiento de los modelos en dimensiones como precisión, relevancia y seguridad. |
| **Flujos (Bedrock Flows)** | Herramienta visual sin código para orquestar flujos de trabajo de IA complejos, combinando modelos y fuentes de datos. |
| **Agentes** | Asistentes de IA que combinan modelos y acciones personalizadas para realizar tareas específicas y complejas. |
| **Seguridad** | Controles de seguridad empresariales que incluyen políticas de IAM, cifrado, puntos de conexión VPC y registros de CloudTrail. |
| **Gobernanza y Barandillas** | Mecanismos de control para gestionar el uso de modelos de IA, como restricciones de acceso, filtros de contenido y reglas de validación de _prompts_. |

---

## Características y Capacidades Clave

* **Acceso Multimodelo**: Cartera de modelos de diversos proveedores a través de una API unificada.
* **Opciones de Personalización**: Soporte para _ajuste fino_ y _RAG_ para adaptar los modelos a necesidades específicas.
* **Marco de Agentes**: Herramienta para crear asistentes de IA que razonan en múltiples pasos y utilizan herramientas externas.
* **Seguridad Empresarial**: Medidas de seguridad integrales que garantizan la privacidad de los datos y el cumplimiento de normativas.
* **Arquitectura Sin Servidor**: Servicio totalmente gestionado que se escala automáticamente, reduciendo la carga operativa.
* **Herramientas de IA Responsable**: Herramientas integradas para _filtrado de contenido_, _barreras de protección_ y _evaluación de modelos_.

---

## Aplicaciones Prácticas Empresariales

* **Generación de Contenido**: Acelera la creación de contenido para marketing (redacción, imágenes).
* **Servicio al Cliente**: Impulsa asistentes de IA para responder consultas rutinarias y mejorar la satisfacción.
* **Análisis de Datos**: Extrae conocimientos de grandes colecciones de documentos.
* **Asistencia en Desarrollo**: Ayuda a ingenieros y gestores de producto con generación de código, documentación y análisis de _feedback_.
* **Sistemas de Gestión del Conocimiento**: Crea sistemas internos de conocimiento accesibles a través de lenguaje natural.

