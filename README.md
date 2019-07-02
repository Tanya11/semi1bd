# semi1bd
#Express.js usando MySQL DB 

Herramientas: 
Editor de texto:Visual Studio Code 
Node.js

Instalación: 
https://nodejs.org/en/download/
Creando la primera API de Node.js (Express):

#Crea una carpeta para la aplicacion

$ mkdir aplicacion 
En el terminal / línea de comandos, vaya a la carpeta creada en el paso anterior
$ cd aplicacion 
Inicializar proyecto de nodo:
$ npm init	 
Para evitar el uso de banderas de preguntas;
$ npm init –yes 
Install Express framework, mySql y body-parser
$ npm install express –save (Express Framework)
$ npm install mysql –save (para conectarse a la base de datos)
$ npm install body-parser 
o Este es un middleware node.js para el manejo de datos de formato JSON, Raw, Text y URL codificados. 

Configuración del servidor: 
nodemon nos ayudará a realizar un seguimiento de los cambios en nuestra aplicación al ver los archivos modificados y reiniciar automáticamente el servidor. 

$ npm install --save-dev nodemon
Crear un archivo server.js

$ touch server.js
Abrir el archivo server.js y escribir el código a continuación: 
var express = require ('express'), 
app = express (), 
port = process.env.PORT || 3000;
app.listen (puerto);

console.log ('el servidor de la API RESTful de la lista  en:' + puerto);

esto ejecutará su aplicación en el puerto que proporcionó cuando inicia el servidor

#Para crear la imagen con el contenedor seguir los siguientes pasos:


imagen/contenedor para base de datos
Pasos a seguir
1. crear una carpeta para el proyecto
cd ~
mkdir proyecto
2. se entra a la carpeta
cd miProyectoDocker
3.crear un archivo dockerfile y agregar las instrucciones para construir
nano dockerfile
4. copiar los archivos para construir la base de datos
5. Crear la imagen de docker con docker build

docker build -t [nombreBD] [dockerfile]
docker build -t my-mysql /home/user/carpeta/
docker build -t my-mysql .
6. entrar al contenedor
docker exec -it [nombreBD] bash
