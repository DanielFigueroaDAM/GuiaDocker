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



