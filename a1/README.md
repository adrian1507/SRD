# Instalación y configuración de LDAP
* Instalamos el paquete LDAP junto con sus librerias

![Captura1](img/Screenshot_1.png)

![Captura2](img/Screenshot_2.png)

* Realizamos la configuración LDAP

![Captura1](img/Screenshot_8.png)

![Captura1](img/Screenshot_3.png)

![Captura1](img/Screenshot_4.png)

![Captura1](img/Screenshot_5.png)

![Captura1](img/Screenshot_6.png)

![Captura1](img/Screenshot_7.png)

* Reiniciamos el servidor LDAP

![Captura1](img/Screenshot_9.png)

## Administración LDAP

### JXplorer

* Instalamos JXplorer

![Captura1](img/Screenshot_10.png)


* Conexión con el servidor LDAP

JXplorer conectará con el servidor LDAP y mostrará el directorio:

![Captura1](img/Screenshot_11.png)

### Organización del directorio LDAP

* Creación de las unidades organizativas

![Captura1](img/Screenshot_12.png)

![Captura1](img/Screenshot_13.png)

### Usuarios y grupos

* Creación de grupos

![Captura1](img/Screenshot_14.png)
![Captura1](img/Screenshot_15.png)

* Creación de usuarios

![Captura1](img/Screenshot_16.png)
![Captura1](img/Screenshot_17.png)

![Captura1](img/Screenshot_18.png)
![Captura1](img/Screenshot_19.png)

![Captura1](img/Screenshot_20.png)
![Captura1](img/Screenshot_21.png)

![Captura1](img/Screenshot_22.png)
![Captura1](img/Screenshot_23.png)

![Captura1](img/Screenshot_24.png)
![Captura1](img/Screenshot_25.png)

## Instalación y Configuración de Carpetas Privadas en Apache con autenticación LDAP:

* Habilitar módulos Apache2 LDAP  *a2enmod ldap; a2enmod
authnz_ldap*.

![Captura1](img/Screenshot_26.png)

* Crear carpeta privada en /var/www con fichero index.html.

![Captura1](img/Screenshot_27.png)

* Creamos nuevos sitios virtuales en /etc/apache2/sites-available/default  con  configuración  de autenticación  LDAP. Un sitio virtual privado de usuario y otro de acceso para grupo.

![Captura1](img/hosts.png)

Sitio de usuario:

![Captura1](img/user-config.png)

![Captura1](img/Screenshot_27.png)

![Captura1](img/acceso-usuario.png)

![Captura1](img/usermiempresa.png)


Sitio de grupo:

![Captura1](img/groups.png)

![Captura1](img/contraseña-grupos.png)

![Captura1](img/acceso-miempresa.png)

![Captura1](img/miempresa.png)
