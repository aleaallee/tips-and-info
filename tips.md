# Tips e información útil de tecnologías, lenguajes y librerías

## Docker

Ejecutar un contenedor de docker:

```shell
docker container run --publish {puertoLocal:puertoContenedor} --detach --name {nombre} --env MYSQL_RANDOM_ROOT_PASSWORD=yes mysql
```

--publish permite abrir los puertos del contenedor a la red local mediante el equipo que está ejecutando el contenedor


## MySQL

Usar mysql-client para conectarse a un servidor mysql que esté dentro de un contenedor de Docker.

```shell
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
