# hello-world-nodejs-docker
Dockerizing a Node.js web app

# Especificaciones DockerFile
* NodeJs version 8 - Alpine (version ligera solo pruebas)



# Pasos para construir
 * docker build -t frankyjquintero/node-web-app-docker-alpine .
 * docker run -p 49160:8080 -d frankyjquintero/node-web-app-docker-alpine
