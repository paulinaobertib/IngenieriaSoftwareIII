## Actividad
1. Modificar nuestro pipeline para incluir el deploy en QA y PROD de Imagenes Docker en Servicio Azure App Services con Soporte para Contenedores
![](imagenes/1.png)
![](imagenes/2.png)
![](imagenes/3.png)
![](imagenes/4.png)
![](imagenes/5.png)
![](imagenes/6.png)
![](imagenes/7.png)
## Desafios
1. Agregar tareas para generar Front en Azure App Service con Soporte para Contenedores
![](imagenes/8.png)
![](imagenes/9.png)
![](imagenes/10.png)
![](imagenes/11.png)
![](imagenes/12.png)
2. Agregar variables necesarias para el funcionamiento de la nueva etapa considerando que debe haber 2 entornos QA y PROD para Back y Front.
![](imagenes/13.png)
3. Agregar tareas para correr pruebas de integración en el entorno de QA de Back y Front creado en Azure App Services con Soporte para Contenedores.
![](imagenes/14.png)
4. Agregar etapa que dependa de la etapa de Deploy en QA que genere un entorno de PROD.
![](imagenes/15.png)
![](imagenes/16.png)
![](imagenes/17.png)
![](imagenes/18.png)
![](imagenes/19.png)
![](imagenes/20.png)
![](imagenes/21.png)
![](imagenes/22.png)
![](imagenes/23.png)
5. Entregar un pipeline que incluya:
- Etapa Construcción y Pruebas Unitarias y Code Coverage Back y Front
- Construcción de Imágenes Docker y subida a ACR
- Deploy Back y Front en QA con pruebas de integración para Azure Web Apps
- Deploy Back y Front en QA con pruebas de integración para ACI
- Deploy Back y Front en QA con pruebas de integración para Azure Web Apps con Soporte para contenedores
- Aprobación manual de QA para los puntos C,D,E
- Deploy Back y Front en PROD para Azure Web Apps
- Deploy Back y Front en PROD para ACI
- Deploy Back y Front en PROD para Azure Web Apps con Soporte para contenedores
**El pipeline se encuentra en mi cuenta de AzureDevOps en el proyecto AngularCRUDAPI, el id es c5165829**
![](imagenes/25.png)
![](imagenes/24.png)
![](imagenes/26.png)
![](imagenes/27.png)
![](imagenes/28.png)
![](imagenes/29.png)
![](imagenes/30.png)
![](imagenes/31.png)