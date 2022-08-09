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
  -Servidor destino:
    -Usuario ansible con permisos sudo sin contraseña
    -SSH

## Guia para lograr un despliegue correcto.
**A continuacion detallamos el paso a paso para poder desplegar la Web Online Boutique aplicando este repositorio**

**Entendemos en este punto que los requerimientos detallados anteriormente se cumplen**

**En este repositorio tenemos en la carpeta OB el árbol de la solución completa con los distintos archivos que sustentan el despliegue automatizado de la aplicación**

**En el siguiente enlace podemos pararnos en dicha carpeta y recorrer cada uno de los archivos [OB](/OB/)**

1-Clonar repositorio de GitHub
  -Situarse en 

## A modo de conclusión:
### Comentar el plan de trabajo realizado. (Trabajo grupal – Aporte individual)

La forma de trabajo fue reuniéndonos en forma presencial o por Microsoft Team en video llamada, compartiendo pantalla, viendo los distintos temas y realizando los distintos pasos del obligatorio, queremos destacar que cada tarea se trató de hacer en conjunto y en línea.

Se trato generalmente de estar involucrados en todas las tareas del obligatorio y trabajar en conjunto.
