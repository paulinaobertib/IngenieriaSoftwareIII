Prerequisitos:
node
![](imagenes/1.png)
npm
![](imagenes/2.png)
angular
![](imagenes/3.png)
.NET Core 8
![](imagenes/4.png)

4.1 Creación de una BD SQL Server para nuestra App
![](imagenes/5.png)
![](imagenes/6.png)
![](imagenes/7.png)
![](imagenes/8.png)

4.2 Obtener nuestra App
![](imagenes/9.png)
![](imagenes/10.png)
![](imagenes/11.png)

4.3 Crear Pruebas Unitarias para nuestra API
![](imagenes/12.png)
![](imagenes/13.png)
![](imagenes/14.png)
![](imagenes/15.png)
![](imagenes/16.png)
Modificacion y perdida de acceso a la bd
![](imagenes/17.png)
![](imagenes/18.png)
![](imagenes/19.png)
Modicacion y correcto acceso a la bd
![](imagenes/20.png)

4.4 Creamos pruebas unitarias para nuestro front de Angular
![](imagenes/21.png)
![](imagenes/22.png)
![](imagenes/23.png)

4.5 Agregamos generación de reporte XML de nuestras pruebas de front
![](imagenes/24.png)
![](imagenes/25.png)

4.6 Modificamos el código de nuestra API y creamos nuevas pruebas unitarias
Modificaciones en el codigo:
- La longitud máxima del nombre y apellido del empleado debe ser de 100 caracteres.
![](imagenes/26.png)
- Validar que el nombre tenga un número mínimo de caracteres, por ejemplo, al menos dos caracteres para evitar entradas inválidas como "A".
![](imagenes/27.png)
- Verificar que el nombre no contenga números, ya que no es común en los nombres de empleados.
![](imagenes/28.png)
- Prohibir el uso de nombres triviales o genéricos como "Empleado", "N/A", "Nombre", etc.
![](imagenes/29.png)
- Evitar que se ingresen caracteres repetidos de forma excesiva, como "Juuuuaannnn".
![](imagenes/30.png)
![](imagenes/31.png)

Pruebas unitarias:
- La longitud máxima del nombre y apellido del empleado debe ser de 100 caracteres.
![](imagenes/32.png)
- Validar que el nombre tenga un número mínimo de caracteres, por ejemplo, al menos dos caracteres para evitar entradas inválidas como "A".
![](imagenes/33.png)
- Verificar que el nombre no contenga números, ya que no es común en los nombres de empleados.
![](imagenes/34.png)
- Prohibir el uso de nombres triviales o genéricos como "Empleado", "N/A", "Nombre", etc.
![](imagenes/35.png)
- Evitar que se ingresen caracteres repetidos de forma excesiva, como "Juuuuaannnn".
![](imagenes/36.png)

Ejecucion:
![](imagenes/37.png)

4.7 Modificamos el código de nuestro Front y creamos nuevas pruebas unitarias
Instalamos la libreria de toast
![](imagenes/38.png)
![](imagenes/39.png)
Modificamos app.config.ts
![](imagenes/40.png)
Creamos toast.css
![](imagenes/41.png)
Agregamos validaciones a addemployee.component.ts
- La longitud máxima del nombre y apellido del empleado debe ser de 100 caracteres.
![](imagenes/44.png)
- Validar que el nombre tenga un número mínimo de caracteres, por ejemplo, al menos dos caracteres para evitar entradas inválidas como "A".
![](imagenes/45.png)
- Verificar que el nombre no contenga números, ya que no es común en los nombres de empleados.
![](imagenes/46.png)
- Prohibir el uso de nombres triviales o genéricos como "Empleado", "N/A", "Nombre", etc.
![](imagenes/47.png)
- Evitar que se ingresen caracteres repetidos de forma excesiva, como "Juuuuaannnn".
![](imagenes/48.png)
Modificamos addemployee.component.spec.ts
- La longitud máxima del nombre y apellido del empleado debe ser de 100 caracteres.
![](imagenes/49.png)
- Validar que el nombre tenga un número mínimo de caracteres, por ejemplo, al menos dos caracteres para evitar entradas inválidas como "A".
![](imagenes/50.png)
- Verificar que el nombre no contenga números, ya que no es común en los nombres de empleados.
![](imagenes/51.png)
- Prohibir el uso de nombres triviales o genéricos como "Empleado", "N/A", "Nombre", etc.
![](imagenes/52.png)
- Evitar que se ingresen caracteres repetidos de forma excesiva, como "Juuuuaannnn".
![](imagenes/53.png)
Realizamos las pruebas
![](imagenes/42.png)
![](imagenes/43.png)