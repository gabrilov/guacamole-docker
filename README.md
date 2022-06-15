# Implementación de Guacamole con Docker

1. Levantar los contenedores.
   
   ```shell
   docker-compose up -d
   ```
   
2. Ejecutar el script para crear las tablas.
   ```shell
   docker exec mysql_guac mysql -u root -p guacamole < guac_initdb.sql
   ```

3. Acceder a la página de Guacamole con la dirección de red del host en el puerto `8080` con credenciales `guacadmin:guacadmin`.