## INSTALAR EN UBUNTU 18.04 UN APACHE

## introduccion Servidor Apache


```$ sudo apt install apache2```

**en caso de error**
---
```sudo fuser -vki /var/lib/dpkg/lock```


Firewall de windows
===

```sudo ufw app list```

```sudo ufw allow 'nombreaplicacion'```

```sudo ufw status```

```sudo ufw enable```

**ejercicio 1.
estamos en la empresa guru.com y nos han pedido que creemos una pequeña pagina web en un servidor apache para probar el servidor web, pero la interfaz grafica no funciona y hay que hacerlo desde la consola.**
===

***estos son los comandos usados para el ejercicio 1***

-para añadir una pagina web al servidor de apache se debe crear un documento .html dentro de la ruta /var/www/html

-para activar el servidor apache debes poner el comando ```systemctl start apache2```

-para ver si el comando se ha ejecutado correctamente y el estado del servidor ponemos en comando ```systemctl status apache2```

-el comando ```hostname -I``` te da las direcciones ip del equipo

-si usas el comando curl con la direccion de alguna web o tu propia ip te saldra el codigo html de esa pagina, por ejemplo ```curl www.google.es```


crear dos carpetas con el comando ```mkdir``` en /var/www para incluir ahi los archvos html que queramos visualizar en nuestra pagina.

copiamos el archivo 000-default.com incluido dentro de las carpetas de apache2 en su instalacion y lo copiamos en la misma ruta en la que se encuentra cambiando su nombre a example.com.conf con el comando

```cp /etc/apache2/sites-available/000-default.conf /etc/apache2/sites-available/example.com.conf```
