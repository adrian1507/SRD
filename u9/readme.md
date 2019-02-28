# Instalación y configuración de un servidor Multimedia
## Introducción
En esta actividad montaremos un servicio de streaming multimedia, accediendo al mismo desde el propio servidor y cliente, comprobando sus funcionalidades.

---

# 1. Icecast2
Comenzamos a instalar y configurar `icecast2`
<p align="center"><img src="img/1.png"></p>

Especificamos el nombre del dominio
<p align="center"><img src="img/2.png"></p>

Establecemos la contraseña para controlar el acceso a los repetidores de emisión
<p align="center"><img src="img/3.png"></p>

También tendremos que establecer la contraseña para administrar la herramienta
<p align="center"><img src="img/4.png"></p>

A continuación, vamos a editar el fichero */etc/icecast/icecast2.xml*, modificando una serie de líneas del mismo para configurarlo a nuestro interés
<p align="center"><img src="img/5.png"></p>

Además, editaremos el fichero */etc/default/icecast* y modificaremos la línea `ENABLE=true`
<p align="center"><img src="img/6.png"></p>

Una vez hecho esto, iniciamos el servicio de `icecast` con `systemctl start icecast2` y consultamos su estado
<p align="center"><img src="img/7.png"></p>

# 2. Codificador Vorbis Ices2
Por otro lado, tendremos que instalar el codificador vorbis con `apt install ices2`
<p align="center"><img src="img/8.png"></p>

Lo siguiente sería copiar el fichero de configuración por defecto desde */usr/share/doc/ices2/examples/ices-playlist.xml* a */etc/ices2*
<p align="center"><img src="img/9.png"></p>

Editamos dicho fichero a nuestro parecer, cambiando algunas etiquetas
<p align="center"><img src="img/10.png"></p>

Modificamos las líneas correspondientes al puerto, la contraseña y el punto de montaje
<p align="center"><img src="img/11.png"></p>

Teniendo esto configurado, descargaremos dos ficheros de audio en formato **.ogg**
<p align="center"><img src="img/12.png"></p>

Generamos la lista de reproducción, introduciendo la ruta de los ficheros de audio en el fichero *playlist.txt*
<p align="center"><img src="img/13.png"></p>

Creamos el directorio */var/log/ices2* y ejecutar el codificador en segundo plano */etc/ices2/ices-playlist.xml &*
<p align="center"><img src="img/14.png"></p>

Accedemos desde un navegador al servidor de audio con la IP y el puerto corrrespondiente
<p align="center"><img src="img/15.png"></p>

También accedemos al entorno de administración
<p align="center"><img src="img/16.png"></p>

Comprobamos que el punto de montaje funciona correctamente
<p align="center"><img src="img/17.png"></p>

Vemos el reproductor del punto de montaje accediendo a `localhost:8000/radiostation`
<p align="center"><img src="img/18.png"></p>

Es momento de comprobar el funcionamiento desde una máquina cliente. Para ello, accedemos mediante la IP al servicio: `172.19.99.125:8000`
<p align="center"><img src="img/19.png"></p>

Vamos a comprobar el entorno de administración desde el cliente
<p align="center"><img src="img/20.png"></p>

Vemos el panel de administración
<p align="center"><img src="img/21.png"></p>

Por último, accedemos al punto de montaje utilizando el software reproductor multimedia que contiene
<p align="center"><img src="img/22.png"></p>
