##############
Servidor Cargo
##############



*******************
Supported platforms
*******************

It is currently supported and maintained for the following platforms and architectures


+-----------------------------------+------------------------+
| Operative System                  | Architecture           |
+===================================+========================+
| Linux 2.6.23 or later with glibc  | amd64, 386, arm, arm64 |
+-----------------------------------+------------------------+


************
Installation
************

On Premise
==========

The following steps are required to install the On Premise version:

1. Environment creation and configuration

2. Cargo Server Installation

3. Apache or Nginx web server installation and configuration 

4. Enabling the corresponding ports in the Firewall


These tasks must be performed by the solution implementer and are included with the purchase of the on-premise license.


Cloud
=====

The Cloud version is installed by deploying the Cargo Server image.


********************
Global Configuration
********************

Cargo Server has global configuration parameters and client-specific parameters. The global configuration parameters allow you to set limits on the number of simultaneous connections and the total bandwidth used. These configuration parameters prevail more than the client-specific parameters.

Global Parameters
=================

- **Global Upload Bandwidth**: Total upload bandwidth assigned to the server
- **Global Download Bandwidth**: Total download bandwidth assigned to the server.
- **Private IP**: Private IP of the interface to be used
- **Public IP**: Public IP of the link to be used.
- **Initial Port**: Port on which the first connection will be established. The range of ports used will be given by the Initial Port + Total connections count.
- **Total connections**: Global number of simultaneous connections enabled.


*************
User Creation
*************

Within the User ABM section, it is possible to manage the credentials for new clients and specify the connection parameters for each one, allowing greater granularity in the use of the available bandwidth.


Client Parameters
=================

- **Username**: Client's user name.
- **Password**: Client's password.
- **Path**: Absolute path where the client's root directory will be found.
- **Upload Speed**: Default upload speed of the transfers.
- **Download Speed**: Default download speed of the transfers.
- **Upload Bandwidth**: Total upload bandwidth assigned to the client.
- **Download Bandwidth**: Total download bandwidth assigned to the client.
- **Enable**: Enable or disable a client



