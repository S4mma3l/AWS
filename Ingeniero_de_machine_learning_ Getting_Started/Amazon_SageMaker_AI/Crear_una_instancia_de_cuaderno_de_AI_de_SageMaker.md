Crear una instancia de cuaderno de SageMaker AI
En esta demostración, aprenderás cómo crear una Instancia de Notebook de SageMaker AI, que proporciona un entorno preconfigurado de Jupyter Notebook para trabajar con tareas de ML. Este es un primer paso importante para usar SageMaker AI porque la Instancia de Notebook sirve como tu entorno de desarrollo para construir, entrenar e implementar modelos de ML.


En esta demostración, aprenderá cómo crear una instancia de cuaderno de SageMaker AI.

En la Consola de administración de AWS, navegue hasta el servicio Amazon SageMaker AI.

En el panel de navegación izquierdo, elija Notebooks.

Luego, elija Crear instancia de notebook.

En el campo Nombre de la instancia de notebook, introduzca un nombre descriptivo para su instancia. Luego, elija un tipo de instancia. Para esta demostración, puede elegir ml.t3.medium.

Desplácese hacia abajo y elija Crear rol para crear un nuevo rol de IAM para su instancia de Notebook. Aquí puede elegir conceder acceso a todos sus buckets de S3, a un bucket específico, a objetos que coincidan con un criterio específico y más. Para esta demostración, elija Cualquier bucket de S3 y elija Crear rol.

Desplácese hasta la parte inferior y elija Crear instancia de notebook.

Espere a que el estado de su instancia de Notebook cambie a InService. Esto puede tardar unos minutos.


