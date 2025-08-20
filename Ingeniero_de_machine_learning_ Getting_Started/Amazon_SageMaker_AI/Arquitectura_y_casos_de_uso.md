# Amazon SageMaker AI: Una guía completa

## Objetivos de la lección

En esta lección, aprenderás a:

* Reconocer la **relación entre Amazon SageMaker AI** y otros **componentes de AWS Cloud**.
* Identificar el **significado de los conceptos técnicos** de SageMaker AI.
* Reconocer **casos de uso típicos** para SageMaker AI.

## ¿Cómo se utiliza Amazon SageMaker AI para diseñar una solución en la nube?

SageMaker AI es un servicio de *machine learning* (ML) de AWS que se integra con varios servicios para diseñar soluciones en la nube.

### Componentes de la solución en la nube

* **VPC del cliente**: Contiene subredes privadas que albergan recursos como las **instancias de cuadernos de SageMaker AI**. Estas subredes garantizan que los recursos no se conecten directamente a internet, aumentando la seguridad.
* **Instancia de notebook**: Es donde se escribe, ejecuta y prueba el código. Se encuentra en una subred privada y se conecta a otros servicios de AWS de forma segura a través de **puntos de conexión de VPC**.
* **Puntos de conexión de VPC**: Permiten la conexión segura de los cuadernos a servicios de AWS sin exponerlos a la internet pública. Hay puntos de conexión para:
    * **Amazon S3**: Almacenamiento y recuperación de datos.
    * **Amazon CloudWatch Logs**: Recopilación y supervisión de registros.
    * **SageMaker Runtime y API**: Interacción con modelos y servicios de SageMaker.
* **Plataforma SageMaker**: Infraestructura gestionada por AWS que incluye:
    * **Servicio de proxy de autenticación**: Gestiona el acceso de usuarios autorizados.
    * **Backend de notebook**: Realiza el cálculo y procesamiento del código.
* **Salida a Internet**: Si es necesario, el tráfico de internet se enruta a través de la VPC de la plataforma SageMaker de manera controlada y segura.

---

## ¿Qué servicios de AWS se integran con Amazon SageMaker AI?

SageMaker AI se integra con las siguientes categorías de servicios de AWS:

| Servicio de AWS | Descripción | Ejemplos de uso |
| :--- | :--- | :--- |
| **IAM** | Gestión de permisos y seguridad. | Un rol de IAM permite que un notebook acceda a Amazon S3; las políticas de IAM controlan los permisos de los usuarios. |
| **Amazon EC2** | Proporciona la capacidad de cómputo subyacente. | Entrenamiento de modelos con instancias de alto rendimiento; alojamiento de modelos para predicciones en tiempo real. |
| **AWS Step Functions** | Orquesta flujos de trabajo de ML. | Automatización de canalizaciones de entrenamiento, ajuste e implementación; combinación de trabajos de SageMaker con otros servicios. |
| **SageMaker Ground Truth** | Servicio de etiquetado de datos. | Generación de conjuntos de datos anotados para el aprendizaje supervisado; integración con flujos de trabajo de etiquetado personalizados. |
| **CloudWatch** | Supervisión y registro del rendimiento. | Métricas en tiempo real para trabajos de entrenamiento; registros para depurar errores; configuración de alarmas. |
| **Amazon VPC** | Asegura la comunicación entre recursos. | Alojamiento de instancias de notebook en subredes privadas; acceso seguro a Amazon S3 y otros recursos mediante puntos de conexión de VPC. |

---

## Conceptos técnicos básicos de Amazon SageMaker AI

SageMaker AI es un servicio de ML gestionado que abstrae la complejidad de la infraestructura. Incluye múltiples componentes:

* **Amazon SageMaker Studio**: Entorno de desarrollo integrado (IDE) para ML, basado en la web.
* **Cuadernos de Amazon SageMaker Studio**: Cuadernos de Jupyter preconfigurados para exploración de datos, entrenamiento de modelos y despliegue.
* **Entrenamiento de Amazon SageMaker**: Servicio de entrenamiento distribuido para modelos de ML en varias instancias de cómputo, incluidas las GPU.
* **Inferencia de SageMaker**: Sistema para desplegar modelos entrenados como servicios alojados para predicciones en tiempo real o por lotes.
* **SageMaker Ground Truth**: Servicio para etiquetar datos y crear conjuntos de datos de entrenamiento de alta calidad.

---

## Casos de uso típicos para Amazon SageMaker AI

SageMaker AI se puede utilizar para diversas tareas de IA/ML en diferentes sectores.

### Casos de uso y ejemplos

* **Análisis predictivo**: Previsión de tendencias para la toma de decisiones.
    * **Ejemplo**: Una cadena minorista pronostica ventas para optimizar el inventario.
* **Reconocimiento de imágenes**: Identificación de objetos, rostros o escenas en imágenes.
    * **Ejemplo**: Un hospital utiliza el reconocimiento de imágenes para detectar tumores en resonancias magnéticas.
* **Procesamiento de Lenguaje Natural (PNL)**: Comprensión y generación de lenguaje humano.
    * **Ejemplo**: Un *chatbot* de servicio al cliente responde a consultas de usuarios como "¿Dónde está mi pedido?".
* **Detección de fraude**: Identificación de patrones y actividades fraudulentas.
    * **Ejemplo**: Un banco monitorea transacciones con tarjetas de crédito en tiempo real para marcar actividades inusuales.
* **Sistemas de recomendación**: Desarrollo de motores de recomendación personalizados.
    * **Ejemplo**: Un servicio de *streaming* sugiere películas basadas en el historial de visualización del usuario.
* **Pronóstico de series temporales**: Predicción de valores futuros basados en datos con marca de tiempo.
    * **Ejemplo**: Una compañía energética pronostica la demanda de electricidad para ajustar la generación.

---

## Consideraciones adicionales

* **Administrar acceso y permisos**: Utiliza **AWS Identity and Access Management (IAM)** para conceder permisos mínimos necesarios a usuarios, roles o aplicaciones.
* **Monitoreo**: Usa **CloudWatch** para supervisar el rendimiento, configurar alarmas y habilitar el registro detallado de tus operaciones.
* **Integración**: Integra SageMaker AI con otros servicios de AWS, como **Amazon S3**, **Lambda** y **Amazon API Gateway** para resolver problemas empresariales de manera efectiva.
* **Rendimiento**: Sigue las mejores prácticas de AWS para garantizar un rendimiento óptimo, seguridad y rentabilidad. Esto incluye usar tipos de instancia adecuados y optimizar el almacenamiento y la transferencia de datos.

Para empezar, consulta la [Guía para configurar Amazon SageMaker AI](https://docs.aws.amazon.com/sagemaker/latest/dg/gs.html).