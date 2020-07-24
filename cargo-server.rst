##############
Servidor Cargo
##############



**********************
Plataformas Soportadas
**********************

Actualmente esta soportado y mantenido para las siguientes plataformas y arquitecturas

+-----------------------------------+------------------------+
| Sistema Operativo                 | Arquitectura           |
+===================================+========================+
| Linux 2.6.23 or later with glibc  | amd64, 386, arm, arm64 |
+-----------------------------------+------------------------+


***********
Instalación
***********

On Premise
==========
Para la instalación de la versión On Premise se requiere realizar los siguientes pasos:
1. Creación y configuración del entorno de python.
2. Seteo del proyecto de Django.
3. Instalación y configuración del servidor web Apache o Nginx. 

Estas tareas deben ser realizadas por el implementador de la solución.

Cloud
=====
La instalación de la versión cloud se realiza mediante el deploy de la imagen de Cargo Server.


********************
Configuración Global
********************
Cargo Server cuenta con parametros de configuraciones globales y parametros específicos para cada cliente. Los parametros de configuracion globales pemiten establecer límites en la cantidad de conextiones simultaneas y el ancho de banda total utilizado. Estos parametros tiene mayor preponderancia que los seteados en el cliente.

Parametros Globales
===================
- **Global Upload Bandwidth**: Ancho de banda total de subida asignado al servidor.
- **Global Download Bandwidth**: Ancho de banda total de descarga asignado al servidor.
- **Private IP**: IP privada de la interface a utilizar.
- **Public IP**: IP pública del enlace a utilizar.
- **Initial Port**: Puerto en el cual se establecerá la primera conexión. El rango de puertos utilizado estará dado por la cuenta **Initial Port** + **Total connections**
- **Total connections**: Número global de conexiones simultáneas habilitadas.


********************
Creacion de Usuarios
********************
Dentro de la sección de ABM de usuarios es posible gestionar las credenciales para nuevos clientes y especificar los parametros específicos de conexión de cada uno, permitiendo mayor granularidad en la utilización del ancho de banda disponible. 

Parametros del Cliente
======================
- **Username**: Nombre de usuario del cliente.
- **Password**: Contraseña del cliente.
- **Path**: Ruta absoluta donde se encontrará el directorio raíz del cliente.
- **Upload Speed**: Velocidad de subida por default de las transferencias.
- **Download Speed**: Velocidad de descarga por default de las transferencias.
- **Upload Bandwidth**: Ancho de banda total de subida asignado al cliente.
- **Download Bandwidth**: Ancho de banda total de descarga asignado al cliente.
- **Enable**: Habilitar o deshabilitar un cliente



