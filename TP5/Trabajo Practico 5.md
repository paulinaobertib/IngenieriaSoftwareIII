5.1. Crear una cuenta en Azure
![](imagenes/1.png)

5.2. Crear un recurso Web App en Azure Portal y navegar a la url provista
![](imagenes/2.png)
![](imagenes/3.png)
![](imagenes/4.png)
![](imagenes/5.png)
![](imagenes/6.png)
![](imagenes/7.png)
![](imagenes/8.png)
![](imagenes/9.png)
![](imagenes/10.png)

5.3. Actualizar Pipeline de Build para que use tareas de DotNetCoreCLI@2 como en el pipeline clásico, luego crear un Pipeline de Release en Azure DevOps con CD habilitada
![](imagenes/11.png)
![](imagenes/12.png)
![](imagenes/13.png)
![](imagenes/14.png)
![](imagenes/15.png)
![](imagenes/16.png)
![](imagenes/17.png)
![](imagenes/18.png)
![](imagenes/19.png)

5.4. Optimizar Pipeline de Build
![](imagenes/11.png)

5.5. Verificar el deploy en la url de la WebApp /weatherforecast
![](imagenes/20.png)
![](imagenes/21.png)
![](imagenes/22.png)

5.6. Realizar un cambio al código del controlador para que devuelva 7 pronósticos, realizar commit, evaluar ejecución de pipelines de build y release, navegar a la url de la webapp/weatherforecast y corroborar cambio
![](imagenes/23.png)
![](imagenes/24.png)
![](imagenes/25.png)
![](imagenes/26.png)

5.7. Clonar la Web App de QA para que contar con una WebApp de PROD a partir de un Template Deployment en Azure Portal y navegar a la url provista para la WebApp de PROD.
![](imagenes/27.png)
![](imagenes/28.png)
![](imagenes/29.png)
![](imagenes/30.png)
![](imagenes/31.png)

5.8. Agregar una etapa de Deploy a Prod en Azure Release Pipelines 
![](imagenes/32.png)
![](imagenes/33.png)
![](imagenes/34.png)

5.9.  Realizar un cambio al código del controlador para que devuelva 10 pronósticos, realizar commit, evaluar ejecución de pipelines de build y release, navegar a la url de la webapp/weatherforecast y corroborar cambio, verificar que en la url de la webapp_prod/weatherforecast se muestra lo mismo.
![](imagenes/35.png)
![](imagenes/36.png)
![](imagenes/37.png)
![](imagenes/38.png)
![](imagenes/39.png)

5.10. Modificar pipeline de release para colocar una aprobación manual para el paso a Producción.
![](imagenes/40.png)

5.11. Realizar un cambio al código del controlador para que devuelva 5 pronósticos, realizar commit, evaluar ejecución de pipelines de build y release, navegar a la url de la webapp/weatherforecast y corroborar cambio, verificar que en la url de la webapp_prod/weatherforecast aun se muestra la versión anterior.
![](imagenes/41.png)
![](imagenes/42.png)
![](imagenes/43.png)

5.12. Aprobar el pase ya sea desde el release o desde el mail recibido. 
![](imagenes/44.png)
![](imagenes/45.png)

5.13. Esperar a la finalización de la etapa de Pase a Prod y luego corroborar que en la url de la webapp_prod/weatherforecast se muestra la nueva versión coinicidente con la de QA.
![](imagenes/46.png)

5.14. Realizar un pipeline (no release) que incluya el deploy a QA y a PROD con una aprobación manual. El pipeline debe estar construido en YAML sin utilizar el editor clásico de pipelines ni el editor clásico de pipelines de release.
![](imagenes/47.png)
![](imagenes/48.png)
![](imagenes/49.png)
![](imagenes/50.png)