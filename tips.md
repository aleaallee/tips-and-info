Usar mysql-client para conectarse a un servidor mysql que esté dentro de un contenedor de Docker.

```bash
mysql -h { IP } -P { puerto } -u{usuario (todo junto tras -u)} -p
```
-h es el parámetro de Host
-P es el parámetro de puerto
-u es el parámetro de usuario, el usuario va junto
-p es el parámetro de contraseña, que se introducirá tras apretar enviar el comando