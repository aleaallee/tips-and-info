# Tips e información útil de tecnologías, lenguajes y librerías

Usar mysql-client para conectarse a un servidor mysql que esté dentro de un contenedor de Docker.

```console
foo@bar:~$ mysql -h { IP } -P { puerto } -u{usuario (todo junto tras -u)} -p
```

-h es el parámetro de Host <br/>
-P es el parámetro de puerto <br/>
-u es el parámetro de usuario, el usuario va junto <br/>
-p es el parámetro de contraseña, que se introducirá tras apretar enviar el comando <br/>

Comandos mysql una vez estemos conectados al servidor sql:

Mostrar las bases de datos existentes:

```SQL
SHOW DATABASES;
```
