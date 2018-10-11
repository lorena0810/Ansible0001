# Cofiguración de Ansible

## Primer paso, instalación de los servidores web y de archivos.

-Intalamos Munin en los 3 servidores
Usamos el siguiente comando:

ansible-playbook -i ../hosts inicial.yml

-luego instalamos el servidor web en el server01
Usamos el siguiente comando:

ansible-playbook -i ../hosts webserver.yml

Segundo paso, instalación del servidor Mysql.
-Intalamos el servidor mysql en el server02
Usamos el siguiente comando:

ansible-playbook -i ../hosts sqlserver.yml

Tercer paso, instalación de Redis.
-Intalamos Redis en el server03
Usamos el siguiente comando:

ansible-playbook -i ../hosts redis.yml

