# Hello-World Nodejs con docker
Dockerizando un Node.js web app - Hola Mundo

# Especificaciones DockerFile
* NodeJs version 8 - Alpine (version ligera solo pruebas)



## Para construir la imagen de Docker

    $ docker build -t frankyjquintero/node-web-app .

## Para ver la imagen creada

    $ docker images

    # Example
    REPOSITORY                      TAG        ID              CREATED
    node                            argon      539c0211cd76    3 weeks ago
    frankyjquintero/node-web-app    latest     d64d3505b0d2    1 minute ago


## Para correr la imagen

    $ docker run -p 49160:8080 -d frankyjquintero/node-web-app

## Y para ver el log de la imagen corriendo

    # Get container ID
    $ docker ps

    # Print app output
    $ docker logs <container id>

    # Example
    Running on http://localhost:8080

## Si necesitas ir dentro del contenedor usa:

    # Enter the container
    $ docker exec -it <container id> /bin/bash

## Para hacer Test

    $ docker ps

    # Example
    ID            IMAGE                                COMMAND    ...   PORTS
    ecce33b30ebf  frankyjquintero/node-web-app:latest  npm start  ...   49160->8080


## Para pinchar la app funcionando

    $ curl -i localhost:49160

    HTTP/1.1 200 OK
    X-Powered-By: Express
    Content-Type: text/html; charset=utf-8
    Content-Length: 12
    Date: Sun, 02 Jun 2013 03:53:22 GMT
    Connection: keep-alive

## O bien desde el navegador

    $ localhost:49160

## Si estas usando Docker en Mac OS o Windows reemplaza el localhost por la ip que da en un comienzo.
