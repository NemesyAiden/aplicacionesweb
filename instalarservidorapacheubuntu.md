## INSTALAR EN UBUNTU 18.04 UN APACHE

## introduccion Servidor Apache


```$ sudo apt install apache2```

**en caso de error**
---

```sudo fuser -vki /var/lib/dpkg/lock```

```sudo ufw app list```

```sudo ufw allow 'nombreaplicacion'```

```sudo ufw status```

```sudo ufw enable```


ejercicio 1.
estamos en la empresa guru.com y nos han pedido que creemos una pequeña pagina web en un servidor apache para probar el servidor web, pero la interfaz grafica no funciona y hay que hacerlo desde la consola.
