## Prerequisitos:
- Azure CLI instalado:
![](imagenes/1.png)

## Actividades
1. Modificar nuestro pipeline para construir imágenes Docker de back y front y subirlas a ACR
    - Crear archivos DockerFile para nuestros proyectos de Back y Front
    ![](imagenes/2.png)
    ![](imagenes/3.png)
    - Crear un recurso ACR en Azure Portal
    ![](imagenes/4.png)
    - Modificar nuestro pipeline en la etapa de Build y Test
    ![](imagenes/5.png)
    ![](imagenes/6.png)
    - En caso de no contar en nuestro proyecto con una ServiceConnection a Azure Portal para el manejo de recursos, agregar una service connection a Azure Resource Manager
    ![](imagenes/7.png)
    - Agregar a nuestro pipeline variables
    ![](imagenes/8.png)
    - Agregar a nuestro pipeline una nueva etapa que dependa de nuestra etapa de Build y Test
    ![](imagenes/9.png)
    - Ejecutar el pipeline y en Azure Portal acceder a la opción Repositorios de nuestro recurso Azure Container Registry. Verificar que exista una imagen con el nombre especificado en la variable backImageName asignada en nuestro pipeline
    ![](imagenes/10.png)
    ![](imagenes/11.png)
    - Agregar a nuestro pipeline una nueva etapa que dependa de nuestra etapa de Construcción de Imagenes Docker y subida a ACR
    ![](imagenes/16.png)
    ![](imagenes/17.png)
    ![](imagenes/18.png)
    Configuramos el archivo Program.cs para que utilice la variable configurada
    ![](imagenes/19.png)
    Otorgamos permisos desde Azure CLI
    ![](imagenes/20.png)
    ![](imagenes/21.png)
    - Ejecutar el pipeline y en Azure Portal acceder al recurso de Azure Container Instances creado. Copiar la url del contenedor y navegarlo desde browser. Verificar que traiga datos.
    ![](imagenes/22.png)
    ![](imagenes/22A.png)
    ![](imagenes/22B.png)

# Desafios
1. Agregar tareas para generar imagen Docker de Front
    - ![](imagenes/12.png)
    - ![](imagenes/13.png)
    - ![](imagenes/14.png)
    - ![](imagenes/15.png)
2. Agregar tareas para generar en Azure Container Instances un contenedor de imagen Docker de Front.
    - Creamos la variable
    - ![](imagenes/23.png)
    - Instalamos lo necesario
    - ![](imagenes/31.png)
    - Modificamos el código del FrontEnd
    - ![](imagenes/24.png)
    - ![](imagenes/24A.png)
    - ![](imagenes/25.png)
    - ![](imagenes/26.png)
    - ![](imagenes/32.png)
    - Modificamos el pipeline
    - ![](imagenes/27.png)
    - ![](imagenes/28.png)
    - Corremos el pipeline
    - ![](imagenes/29.png)
    - Comprobamos
    - ![](imagenes/30.png)
    - ![](imagenes/33.png)
3. Agregar tareas para correr pruebas de integración en el entorno de QA de Back y Front creado en ACI.

4. Agregar etapa que dependa de la etapa de Deploy en ACI QA y genere contenedores en ACI para entorno de PROD.
