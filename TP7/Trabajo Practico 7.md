4.1 Agregar Code Coverage a nuestras pruebas unitarias de backend y front-end e integrarlas junto con sus resultados en nuestro pipeline de build.
- 4.1.1 En el directorio raiz de nuestro proyecto Angular instalar el siguiente paquete:
![](imagenes/1.png)
- 4.1.2 Editar nuestro archivo karma.conf.js para que incluya reporte de cobertura:
![](imagenes/2.png)
- 4.1.3 En el dir raiz del proyecto EmployeeCrudApi.Tests ejecutar:
![](imagenes/3.png)
- 4.1.4 Agregar a nuestro pipeline ANTES del Build de Back la tarea de test con los argumentos especificados y la de publicación de resultados de cobertura:
![](imagenes/4.png)
- 4.1.5 Agregar a nuestro pipeline ANTES del Build de front la tarea de test y la de publicación de los resultados:
![](imagenes/5.png)
- 4.1.6 Ejecutar el pipeline y analizar el resultado de las pruebas unitarias y la cobertura de código:
![](imagenes/6.png)
![](imagenes/7.png)

4.2 Agregar Análisis Estático de Código con SonarCloud.
![](imagenes/8.png)
![](imagenes/9.png)
![](imagenes/10.png)

El informe de SonarCloud ha destacado varios aspectos clave para mejorar el proyecto en términos de calidad, seguridad y mantenibilidad. Entre los principales hallazgos se incluyen:
- Code smells: Se detectaron indicios de código que no afectan el funcionamiento inmediato, pero sugieren mejoras para facilitar su comprensión y modificación. Por ejemplo, se recomienda convertir ciertos métodos en estáticos para optimizar el uso de memoria y mejorar la claridad del código.
- Referencias nulas: Se encontraron riesgos de fallos en tiempo de ejecución debido a variables o métodos que pueden ser nulos, lo que requiere una mejor gestión para evitar problemas inesperados en la aplicación.
- Seguridad: El informe señala la presencia de valores sensibles, como contraseñas, incrustados en el código, lo que representa una vulnerabilidad significativa. Se recomienda mover estos valores a entornos más seguros.
- Vulnerabilidades críticas: Se identificaron fallos de seguridad que deben corregirse para evitar posibles ataques que comprometan la estabilidad del sistema y la protección de los datos de los usuarios.
- Prácticas ineficientes: Se observó el uso de técnicas como "RunSync", que puede afectar el rendimiento de la aplicación. Optimizar estos aspectos mejoraría la eficiencia y escalabilidad del código.