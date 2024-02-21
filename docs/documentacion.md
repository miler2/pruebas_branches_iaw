# IAW
En este repositorio tengo todas las actividadess de IAW.

## Primer trimestre:
### - [practica01-01](practica01-01)
Instalación de la pila LAMP en una instancia EC2 de AWS con Ubuntu Server.

### - [practica01-02](practica01-02)
Instalación de la pila LAMP en una instancia EC2 de AWS con RHEL.

Esto es lo mismo que la primera práctica, pero con una máquina de red hat.

### - [practica01-03](practica01-03)
Despliegue de una aplicación web LAMP sencilla.

### - [practica01-04](practica01-04)
HTTPS. Configuración de un certificado SSL/TLS autofirmado en Apache.

### - [practica01-05](practica01-05)
TTPS con Let’s Encrypt y Certbot.

### - [practica01-06](practica01-06)
Instalación de WordPress en una instancia EC2 de AWS.

### - [practica01-07](practica01-07)
Administración de Wordpress con la utilidad WP-CLI.

### - [practica01-08](practica01-08)
Instalación de PrestaShop en AWS.

### - [practica01-09](practica01-09)
Arquitectura de una aplicación web LAMP en dos niveles.

### - [practica01-10](practica01-10)
Balanceador de carga con Apache.

### - [practica01-11](practica01-11)
Arquitectura de una aplicación web LAMP en tres niveles.

### - [practica02-01](practica02-01)
Instalación de la pila LEMP en una instancia EC2 de AWS.

En esta práctica vamos a instalar la pila LEMP que es una variación de la pila LAMP. La única diferencia es que usa el servidor Nginx en lugar de Apache.

## Segundo trimestre:
### - [practica03-01](practica03-01)
Implantación de WordPress en Amazon Web Services (AWS) mediante Ansible.

### - [practica04-01](practica04-01)
AWS CLI (Command Line Interface).

Esto nos permite manejar las máquinas de aws desde una sola máquina. Podríamos crear, eliminar, y modificar instancias, además de crear grupos de seguridad e ips elásticas.

### - [practica04-05](practica04-05)
Terraform.

En esta práctica vamos a aprender cómo usar terraform, una plataforma que hace lo mismo que aws-cli, pero de una forma universal para todos los distribuidores, como openstack y aws, no solo para aws.

## Cosas a tener en cuenta

### - .gitignore
Este archivo me está dando la posibilidad de ignorar ciertos archivos que se crean dentro de este directorio que no quiero que se clonen cuando uso el comando git.

### Documentación de Terraform
Explicación extensa sobre cómo funciona terraform está en la [práctica04-05](practica04-05/README.md)


# Practicas enseñadas y terminadas (primer trimestre)
/ = entregada  
x = no entregada

- practica01-01 (/)
- practica01-02 (x)
- practica01-03 (x) - Hecho
- practica01-04 (x) - Hecho (entregado?)
- practica01-05 (x)
- practica01-06 (/)
- practica01-07 (/)
- practica01-08 (x)
- practica01-09 (/)
- practica01-10 (/)
- practica01-11 (/)


# Preguntas que tengo:
## Pregunta 1
Para qué hace falta crear un alias para el comando certbot para hacer un certificado lets encrypt?

> sudo ln -fs /snap/bin/certbot /usr/bin/certbot

## Pregunta 2
No hace falta poner esta línea en la instalación con ansible??

> chown -R www-data:www-data /var/www/html

## Pregunta 3
Qué demonios pasa que no consigo ejecutar esto en la práctica01-03 (000-default.con)
```
    RewriteEngine On
    RewriteCond %{HTTPS} off
    RewriteRule ^ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301]
```

# Notas en clase:
WSL2

Una aplicacion para windows para poder usar docker correctamente.