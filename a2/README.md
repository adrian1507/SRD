# Servicio SMTP Windows 2016 Server

## Instalación de SMTP

* Instalar Servicio SMTP en Windows 2016 Server



## Configuración de SMTP

* Configuración de servicio SMTP a través del administrador de aplicaciones (IIS) 6.0. Realizar las siguientes acciones de configuración:

  - Establecer como IP todas las asignadas.
  - Limitar el número de conexiones a 50.
  - Habilitar el registro en formato W3C, diario y en una carpeta determinada.

![Captura](img/Captura.PNG)

![Captura](img/Captura1.PNG)

  - Configurar envío de mensajes dentro de nuestra red local: Aceptar la conexión al servidor y la retransmisión de mensajes a todos los equipos menos los que aparecen en la lista.

![Captura](img/Captura2.PNG)

![Captura](img/Captura3.PNG)

  - Establecer autenticación anónima

  ![Captura](img/Captura4.PNG)

  - Echar un vistazo al resto de opciones de configuración del servidor. Aplicar cambios y reiniciar servicio.
  - Comprobar la existencia del dominio AD predeterminado. Crea un dominio de tipo alias para disponer de cuentas en otro dominio.

  ![Captura](img/Captura5.PNG)

  ![Captura](img/Captura6.PNG)

  ![Captura](img/Captura7.PNG)

  - Comprueba carpetas de correo creados en C:\Inetpub\mailroot.

  ![Captura](img/Captura.PNG)

### Cliente Windows:

* Comprobar acceso al nuevo nombre DNS creado en el servidor.

* Configurar el cliente de correo Live mail agregando dos cuentas de correo cualesquiera (usuarios AD -dominio- y no AD). Se deberá especificar: usuario / buzón, contraseña,  servidor SMTP.

* Enviar varios correos desde / hacia las diferentes cuentas y comprobar envío (real o ficticio) y carpetas mailroot. Las carpetas existentes en mailroot alojan mensajes en cola (Queue), mensajes para destinatarios desconocidos (Badmail) y mensajes entregados (Drop).

### Servidor SMTP:

* Nueva configuración de servicio SMTP a través del administrador de aplicaciones (IIS) 6.0. Establecer autenticación básica de Windows. Probar diferentes configuraciones de dominio predeterminado, cifrado TLS, etc.

### Cliente Windows:

* Configurar las cuentas según los parámetros especificados en el servidor. Enviar varios correos desde / hacia las diferentes cuentas y comprobar envío y carpetas mailroot. En este caso sólo tendrán acceso al servidor SMTP cuentas del dominio y correspondientes a usuarios de AD.
