---
title: "Personalizar pantalla de login Gnome"
date: 2023-06-01T14:03:27-06:00
draft: false
---

# COMO PERSONALIZAR LA PANTALLA DE INICIO DE SESION EN UBUNTU

Este post sirve para poder modificar el fondo de la pantalla de inicio de sesión en sistema Ubuntu con Gnome.

1. Lo primero que se necesita es ejecutar en consola el siguiente comando:
~~~
sudo apt install libglib2.0-dev-bin
~~~

2. Nos dirigimos al repositorio [gdm-set-background](https://github.com/PRATAP-KUMAR/ubuntu-gdm-set-background) y de ahi obtenemos un par de comandos utiles para obtener el script necesario.

~~~
$ wget -q https://raw.githubusercontent.com/PRATAP-KUMAR/ubuntu-gdm-set-background/main/ubuntu-gdm-set-background && chmod +x ubuntu-gdm-set-background

$ curl -fL 'https://raw.githubusercontent.com/PRATAP-KUMAR/ubuntu-gdm-set-background/main/ubuntu-gdm-set-background' -o ubuntu-gdm-set-background && chmod +x ubuntu-gdm-set-background
~~~

3. Se obtiene y se ubica dentro de nuestro equipo la imagen que vamos a utilizar.

4. Abrimos una nueva terminal y nos posicionamos en la carpeta donde tenemos la imagen, ahí ejecutamos cualquiera de los comandos del punto anterior y se genera un nuevo script.

![](../image1.png)

5. En la misma terminal ejecutamos el script que acabamos de generar usando las instrucciones:

~~~
sudo ./ubuntu-gdm-set-background --image 'ubicacion de la imagen'
~~~

Al terminar de ejecutar nos debe mostrar un mensaje de operacion exitosa.

![](../image2.png)