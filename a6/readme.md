# Servicio VoIP
## Introducción
En esta actividad instalaremos un servicio de llamadas con la herramienta **PBX 3CX**, comprobando el envío y recepción de llamadas.

---

# 1. BX 3CX Phone System
## 1.1. Instalación
Comenzamos instalando el software de administración **PBX 3CX Phone System**. Vemos los requerimientos que nos exige.
<p align="center"><img src="img/1.png"></p>

Establecemos la ruta de instalación
<p align="center"><img src="img/4.png"></p>

Comenzamos la instalación
<p align="center"><img src="img/5.png"></p>

Tendremos que instalar también el complemento **Microsoft Visual C++**
<p align="center"><img src="img/7.png"></p>

Completamos la instalación
<p align="center"><img src="img/9.png"></p>

Además, tendremos que instalar otro complemento aparte
<p align="center"><img src="img/11 (2).png"></p>

Seguimos la instalación colocando el código de licencia que se nos ha sido enviado a nuestro correo
<p align="center"><img src="img/13.png"></p>

## 1.2. Configuración
Iniciamos sesión con el usuario administrador para acceder a su panel
<p align="center"><img src="img/14.png"></p>

Confirmamos que usaremos esa IP Pública
<p align="center"><img src="img/15.png"></p>

Indicamos que sea estática
<p align="center"><img src="img/16.png"></p>

Elegimos un nombre de subdominio
<p align="center"><img src="img/17.png"></p>

Visualizamos los puertos de acceso por defecto
<p align="center"><img src="img/18.png"></p>

Seleccionamos el adaptador de red predeterminado
<p align="center"><img src="img/19.png"></p>

También tendremos que elegir la longitud de las extensiones
<p align="center"><img src="img/20.png"></p>

Introducimos un correo para posibles notificaciones del sistema
<p align="center"><img src="img/21.png"></p>

Elegimos el país y zona horaria correspondiente
<p align="center"><img src="img/22.png"></p>

Vamos a crear el primer usuario por defecto con todos sus datos: número de extensión, nombre, correo electrónico...
<p align="center"><img src="img/23.png"></p>

Tenemos la posibilidad de elegir a que región del planeta podemos hacer llamadas. Elegimos Europa.
<p align="center"><img src="img/24.png"></p>

Seleccionamos el idioma de nuestra preferencia
<p align="center"><img src="img/25.png"></p>

Confirmamos los datos de registro
<p align="center"><img src="img/26.png"></p>

Una vez hemos terminado esto, recargamos la página y volvemos a acceder al panel de administración
<p align="center"><img src="img/27.png"></p>

Vemos como ya tenemos creada una extensión con el usuario creado anteriormente
<p align="center"><img src="img/28.png"></p>

Crearemos otros usuarios con una extensión distinta
<p align="center"><img src="img/29.png"></p>

<p align="center"><img src="img/30.png"></p>

## 1.3. Comprobación
Para comprobar que la configuración realizada es correcta, descargaremos un software cliente para realizar llamadas, en este caso, usaremos **SIP softphone 3CX Phone**
<p align="center"><img src="img/31.png"></p>

Iniciamos sesión con uno de los usuarios creados en pasos anteriores
<p align="center"><img src="img/32.png"></p>

Vemos como se ha creado
<p align="center"><img src="img/33.png"></p>

También tendremos que instalar el mismo programa en una máquina cliente para hacer/recibir llamadas
<p align="center"><img src="img/01.png"></p>

Completamos la instalación
<p align="center"><img src="img/03.png"></p>

Visualizamos la interfaz del programa
<p align="center"><img src="img/04.png"></p>

Iniciamos sesión también con otro de los usuarios diferente al del servidor
<p align="center"><img src="img/06.png"></p>

Comprobamos que se ha creado
<p align="center"><img src="img/07.png"></p>

Ya podemos realizar y recibir llamadas mediante las extensiones. Llamamos desde el servidor al cliente
<p align="center"><img src="img/34.png"></p>

Recibimos la llamada desde el servidor
<p align="center"><img src="img/08.png"></p>

Y establecemos la llamada correctamente
<p align="center"><img src="img/09.png"></p>

Llamamos inversamente en esta ocasión
<p align="center"><img src="img/10.png"></p>

Recibimos la llamada en el servidor proveniente del cliente
<p align="center"><img src="img/35.png"></p>

Y establecemos la llamada
<p align="center"><img src="img/36.png"></p>

Comprobamos las llamadas realizadas
<p align="center"><img src="img/37.png"></p>
