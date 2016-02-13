# Contenedores Docker

### containers_for_redmine

Realiza la instalación de:

* MySQL
* Un ambassador de MySQL
* Redmine
* Un ambassador de Redmine

En el script se deja parado el container que corresponde a MySQL debido a que, por norma general, no debería ser necesario acceder desde fuera jamás a la base de datos.

Para acceder al servidor de redmine será necesario acceder con

* usuario: admin
* contraseña: admin

> Es altamente recomendable cambiar la contraseña del usuario administrador.

> Nota: En la ejecución del script se hace un `sleep` de 20 segundos para dar tiempo al servidor a iniciar MySQL debido a que, en las pruebas, redmine se iniciaba más rápido de lo que tardaba MySQL en estar operativo, dando fallo. Los `sleep` mostrarán cinco mensajes graciosos, no hay de que alarmarse :P
