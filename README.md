# docker-gcp-deployment
Infraestructura se configura la imagen ubuntu LTS, ip estatica (no es necesario Prueba), permite http
#CREACION DE LLAVES SSH, ejecute powershell como administrador
ssh-keygen -t rsa -b 4096 -C "sosasjose.01@gmail.com"
#Abrir en la consola
cat ~/.ssh/id_rsa.pub
#Copiamos la ip publica al servidor
#conectamos al servidor
ssh -i C:\Users\usuario\.ssh\id_rsa sosasjose.01@34.176.249.207
#Usuario con previlegios
sudo su 
snap install docker
# lista la imagenes que se tiene
docker ps
#lista de comandos de la instruccion docker
docker help
docker version
#Ahora generar las claves SSH y agregarlas GITHUB, pero en el servidor
ssh-keygen -t rsa -b 4096 -C "sosasjose.01@gmail.com"
Extraemos la clave publica 
cat ~/.ssh/id_rsa.pub
Esa clave se pega en GITHUB Setting ssh
Luego probar al conexion 
ssh -T git@github.com
Tener en el repositorio los codigos backend y fontend
Luego crear el dockerfile para la aplicacion del backend

Ahora crear un docker compose para este archivo

Ahora seguimos los pasos para generar un dockerfile para la aplicacion frontend

Ahora el archivo de configuracion de nginx
creacion del docker-compose.yml
creamos al red de docker en el servidor
docker network create demo_deploy
clonar el proyecto en el servidor
git clone 
cd docker-gcp-deployment
git pull
docker compose up -d
docker ps
---------------
docker compose down
docker compose up -d --build
