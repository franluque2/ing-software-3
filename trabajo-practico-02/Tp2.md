# Segundo Trabajo de Ingenieria de Software 3 - Introducción a Docker

Este trabajo fue hecho para realizar la segunda asignatura de la materia.

### 4- Desarrollo:

#### 1- Instalar Docker Community Edition

Ya tenía Docker en mi maquina virtual. 

![Screenshot](Imagenes/imagen1.png)


#### 2- Explorar DockerHub
  - Me registré en Dockerhub y me familiarizé con el sitio.
  
  ![Screenshot](Imagenes/imagen2.png)
  

#### 3- Obtener la imagen BusyBox
  - Se bajo la imagen BusyBox de Dockerhub
  
  ![Screenshot](Imagenes/imagen3.png)
  
  - Y se reviso su peso y version
  
  ![Screenshot](Imagenes/imagen4.png)

#### 4- Ejecutando contenedores
  - Se corrio docker run busybox  
  No obtenemos ningun resultado, ya que por defecto al correr Busybox solo crea el contenedor, ejecuta la shell de linux y al no tener ningun otro comando sale sin hacer nada mas. 
  - Al realizar docker run busybox echo "Hola Mundo!" si obtenemos un resultado, ya que ejecuta el comando que le pasamos.
  ![Screenshot](Imagenes/imagen6.png)
  - Al realizar docker ps no obtenemos nada, porque no hay contenedores en ejecución. Al realizar docker ps -a, se listan todos loq contenedores aunque no esten en ejecucion actual.
  ![Screenshot](Imagenes/imagen7.png)
  

#### 5- Ejecutando en modo interactivo
  ![Screenshot](Imagenes/imagen8.png)

#### 6- Borrando contendores terminados
  ![Screenshot](Imagenes/imagen9.png)
  
  No se ejecuto docker prune a fin de no borrar otro docker si utilizado, una base de mysql.

#### 7- Montando volúmenes

 ![Screenshot](Imagenes/imagen10.png)
 ![Screenshot](Imagenes/imagen11.png)
 
 
#### 8- Publicando puertos

 ![Screenshot](Imagenes/imagen12.png)
 ![Screenshot](Imagenes/imagen13.png)
 ![Screenshot](Imagenes/imagen14.png)
 ![Screenshot](Imagenes/imagen15.png)
 ![Screenshot](Imagenes/imagen16.png)
 
#### 9- Utilizando una base de datos
 ![Screenshot](Imagenes/imagen17.png)
 ![Screenshot](Imagenes/imagen18.png)
 
 Con el Docker Run creamos un contenedor nuevo. Docker Exec nos permite ejecutar comandos en un contenedor que ya este corriendo.