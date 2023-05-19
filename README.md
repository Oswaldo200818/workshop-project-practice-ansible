Proyecto de Tareas con Ansible
author: oquinteros

Este proyecto utiliza Ansible para automatizar tareas relacionadas con la instalación y configuración de PostgreSQL en servidores.

Requisitos

Ansible: Asegúrate de tener Ansible instalado en el sistema desde el cual ejecutarás las tareas.

PostgreSQL: PostgreSQL es un sistema de gestión de bases de datos relacionales (RDBMS) orientado a objetos.

Estructura del proyecto

playbooks/: Contiene el playbook principal main.yml con las tareas específicas
dentro de la carpeta tasks.

roles/: Contiene el rol bdd_simple para las tareas relacionadas con PostgreSQL
y su llamada es por el site.yml.

vars/: Contiene los archivos YAML con las variables utilizadas.
---
database_name: bd_example
database_user: admin


Ejecución

ansible-playbook site.yml -i inventory.ini


Licencia
Este proyecto está licenciado bajo la Licencia MIT. ('-')
