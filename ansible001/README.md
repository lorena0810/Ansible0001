# Cofiguración de Ansible

## Despliegue de plataforma Moodle

Se instalaran  y configuraran estos  3 servicios : 
<ul>
  <li>Apache</li>
  <li>MySQL</li>
  <li>Redis</li>
</ul>

<h3>Primer paso, instalación de los servidores web y de archivos.</h3>

### -Intalamos Munin en los 3 servidores

Usamos el siguiente comando: 

ansible-playbook -i ../hosts inicial.yml

### -luego instalamos el servidor web en el server01

Usamos el siguiente comando: 

ansible-playbook -i ../hosts webserver.yml

<h3>Segundo paso, instalación del servidor Mysql.</h3>

### -Intalamos el servidor mysql en el server02

Usamos el siguiente comando: 

ansible-playbook -i ../hosts sqlserver.yml

<h3>Tercer paso, instalación de Redis.</h3>

### -Intalamos Redis en el server03

Usamos el siguiente comando: 

ansible-playbook -i ../hosts redis.yml


## -Solo faltaria instalar Moodle

Ir a Ansible002
