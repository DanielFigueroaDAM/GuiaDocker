# Práctica Docker - Gestión de contenedores Alpine

## Tarea 1: Descargar imagen Alpine sin arrancarla

![MaquinaDescargarSinArrancar](img.png)

Con este comando descargamos la imagen de Alpine sin arrancar ningún contenedor.

![imagenes](img_1.png)

La captura muestra que la imagen se ha descargado correctamente.

## Tarea 2: Arrancar un contenedor de Alpine sin nombre

![arrancarContenedor](img_2.png)

Con este comando arrancamos un contenedor de Alpine sin nombre.

![nombreImagen](img_3.png)

Para obtener el nombre del contenedor usamos el comando `docker ps -a`, ahí nos muestra los diferentes datos del contenedor, entre ellos el nombre.

## Tarea 3: Crear un contenedor Alpine con nombre dam_alp1

![creadaDam_alp1](img_4.png)

Con el comando `docker run -it --name dam_alp1 alpine` creamos un contenedor Alpine con el nombre dam_alp1 y accedemos a su terminal.

# Tarea 4: Acceder a internet desde el contenedor dam_alp1

![accediendoAGoogle](img_5.png)

Hacemos ping a google.com para comprobar que tenemos acceso a internet, y a 8.8.8.8 que es un servidor DNS de Google.
(En ese momento fallaba la conexión a internet)

![ipDam_alp1](img_6.png)

Dentro de la terminal del alpine "dam_alp1" usamos el comando `ip a` para ver la IP que tiene asignada el contenedor (172.17.0.2).

## Tarea 5: Crear un contenedor Alpine con nombre dam_alp2

Creamos el contenedor dam_alp2 con el comando `docker run -it --name dam_alp2 alpine`, y usamos el comando `ip a` para ver su IP (172.17.0.3).

![crear_alp2](img_9.png)

Al adquirir las IPs ya podemos hacer ping entre los dos contenedores.

![pingAlp1Alp2](img_10.png)

![pingAlp2Alp1](img_11.png)

