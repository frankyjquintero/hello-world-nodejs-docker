# Hello-World Nodejs con docker
Dockerizing a Node.js web app

# Especificaciones DockerFile
* NodeJs version 8 - Alpine (version ligera solo pruebas)



# Pasos para construir imagen
  ## docker build -t frankyjquintero/node-web-app-docker-alpine .
# Iniciar imagen
  ## docker run -p 49160:8080 -d frankyjquintero/node-web-app-docker-alpine
