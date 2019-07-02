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
