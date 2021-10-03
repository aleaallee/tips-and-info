# Tips e información útil de tecnologías, lenguajes y librerías

## Docker

### Ejecutar un contenedor de docker:

```shell
docker container run --publish { puertoLocal:puertoContenedor } --detach --name { nombre } --env MYSQL_RANDOM_ROOT_PASSWORD=yes mysql
```

--publish permite abrir los puertos del contenedor a la red local mediante el equipo que está ejecutando el contenedor.
--detach permite ejecutar el contenedor en segundo plano.
--name permite establecer el nombre del contenedor

### Listar los procesos de un contenedor

```shell
docker container top { contenedor }
```

### Inspeccionar la configuración de un contenedor

```shell
docker container inspect { contenedor }
```

### Mostrar el estado de todos los contenedores

```shell
docker container stats
```

## MySQL

Usar mysql-client para conectarse a un servidor mysql que esté dentro de un contenedor de Docker.

```shell
foo@bar:~$ mysql -h { IP } -P { puerto } -u{usuario (todo junto tras -u)} -p
```

-h es el parámetro de Host.
-P es el parámetro de puerto.
-u es el parámetro de usuario, el usuario va junto.
-p es el parámetro de contraseña, que se introducirá tras apretar enviar el comando.

Comandos mysql una vez estemos conectados al servidor sql:

Mostrar las bases de datos existentes:

```SQL
SHOW DATABASES;
```
