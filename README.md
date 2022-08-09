# Universidad ORT
## Obligatorio Taller de Servidores Linux

---
### - Matías Landoni (261816)

---
## Objetivo del Obligatorio.
El objetivo del obligatorio es automatizar el despliegue en servidores Ubuntu y RedHat(Rocky) de los servicios Tomcat 9 y MariaDB/MySQL mediante el uso de ansible.

Este repositorio contiene lo necesario para que un usuario despliegue de forma automatizada dichos servicios.

## Descripción de la función de cada servicio.

Se cuenta con 2 playbooks diferentes, uno para la instalacion de MariaDB y otro para Tomcat, ambos pueden ser utilizados en los SO mencionados previamente.

Tareas realizadas por cara PlayBook

MariaDB

  -Implementacion del repositorio de MariaDB version 10.8
  
  -Instalacion de paquetes necesarios
  
  -Inicio automatico del servicio
  
  -Importacion de archivo de configuracion, base de datos y usuario

Tomcat
  -Instalacion de paquetes necesarios
  -Creacion de directorios y usuario
  -Descarga e instalacion de Tomcat 9
  -Inicio automatico del servicio
  -Importacion de archivos de configuracion

## Requerimientos necesarios para poder desplegar la infraestructura.
  -Servidor bastion
    -Ansible 
    -Keys SSH de servidores destino
    -Git
  -Servidor destino:
    -Usuario ansible con permisos sudo sin contraseña
    -SSH

## Guia para lograr un despliegue correcto.
**A continuacion detallamos el paso a paso para poder desplegar la Web Online Boutique aplicando este repositorio**

**Entendemos en este punto que los requerimientos detallados anteriormente se cumplen**

1-Clonar repositorio de GitHub
  *Situarse en directorio desde el cual ejecutar los playbooks y ejecutar el siguiente comando: git clone https://github.com/matiaslandoni/Obligatorio_Taller2022.git
  *Extraer los archivos contenidos dentro del ZIP

2-Configuracion y ejecucion de PlayBook

  * Modificar el archivo hosts con las IPs de los servidores destino
  
  * Situarse en el directorio en el que se encuentra el archivo .yaml que se desea desplegar (mariadb o tomcat).
  
  * Ejecutar el siguiente comando en equipo bastion: "ansible-playbook -i hosts $.yaml" (sin comillas, reemplazar $ por playbook a ejecutar)

Una vez finalizado el proceso de instalacion, los servicios se encontraran desplegados y disponibles para su uso.

