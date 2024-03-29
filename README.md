# Creacion de API en NodeJS y MongoDB
Inicializamos el proyecto con `git init`, llenando los campos requeridos.

## Dependencias
1. Instalación de nodemon den modo desarrollador `npm install nodemon --save-dev`
2.  Instalacion de Express y dotenv `npm install express dotenv`
3. Instalacion de Mogoose para modelado de mongo `npm install mongoose`
4. se requiere el bodyParser para parsear cuando se reciba un post `npm i body-parser	`

## Crear volumen y levantar Docker
Se debe crear un archivo llamado `docker-compose.yml`, con las siguientes indicaciones:
`version: '3.8'
services:
mongo-db:
image: mongo:6.0.13
restart: always
environment:
MONGO_INITDB_ROOT_USERNAME: ${MONGO_USER}
MONGO_INITDB_ROOT_PASSWORD: ${MONGO_PASS}
ports:
- 27017:27017`

Para evidenciar el orden, configuracion y espaciado visitar la documentación:
`https://hub.docker.com/_/mongo` : Example `docker-compose.yml` for `mongo`:
