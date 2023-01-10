# Nginx: Ajustes Basicos
## Introducción:
Es un servidor web de código abierto que puede ser usado como alternativa a Apache que desde su éxito inicial como servidor web, ahora también es usado como proxy inverso, cache de HTTP y balanceador de carga.

## Comparativa con Apache:
1. Respecto a su sistema operativo, encontramos que ambos funcinan bien con sistemas como UNIX,Linux y variaciones, pero Apache tiene una mejor performance que Nginx.
2. En cuanto a Administracion y Mantenimiento encontramos que el soporte de Apache está respaldado por una comunidad de desarrolladores de todo el mundo mientras que por parte de Nginx, todo su soporte lo realiza la empresa que lo creó.
3. En rendimiento Apache solo tiene un solo hilo asociado a una sola conexión  mientras que Nginx es capaz de manejar miles, haciendo que la memoria dismiuya y aumente la velocidad y rendimiento.
4. Por el lado de la escalabilidad, Nginx está basada en eventos que permiten tener un rendimiento mayor incluso si se trata de un tráfico pesado. Esto no es posible con Apache ya que tiene una arquitectura de subprocesos múltiples que hacen difícil que esta escalabilidad se pueda lograr. 
5. Finalmente, desde el procesamiento de contenido dinamico encontramos que Apache procesa contenido dinámico de forma nativa dentro del propio servidor web, lo cual Nginx es incapaz de realizar ya que depende de los procesos que se puedan realizar de forma externa.

## Instalación:
1. Primero actualizaremos los repositorios e instalaremos el paquete de nginx, comprobando su estado.

![1](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura.PNG)
![2](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura2.PNG)
![3](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura3.PNG)
![2.5](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura2.5.PNG)

2. Instalar el firewall ufw, comprobar su esatdo y habilitar el perfil de Nginx HTTP

![5](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura5.PNG)
![4](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura4.PNG)

3. Comprobar en un navegador que nginx funciona.

![6](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura6.PNG)

4. Crear las carpetas y archivos donde alojar nuestro servidor nginx.

![7](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura7.PNG)
![8](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura8.PNG)
![9](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura9.PNG)
![10](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura10.PNG)

5. Habilitaremos el archivo creando un enlace entre él y sites-enabled.

![11](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura11.PNG)

6. Añadimos o descomentamos esta linea en el fichero de configuracion de nginx para evitar problemas de memoria.

![12](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura12.PNG)

7. Nos aseguramos de que todo este correctamente y visitamos nuestra pagina nginx.

![13](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura13.PNG)


## Casos Practicos:
a. Versión de Nginx

![ver](https://github.com/lmrs-06/nginx/blob/main/nginx/version.PNG)

b. Ficheros de configuración

![fich](https://github.com/lmrs-06/nginx/blob/main/nginx/ficheros.PNG)

c. Personalización de la pagina

![14](https://github.com/lmrs-06/nginx/blob/main/nginx/Captura14.PNG)

d. Balanco de carga

![1](https://github.com/lmrs-06/nginx/blob/main/nginx/1.PNG)

![2](https://github.com/lmrs-06/nginx/blob/main/nginx/2.PNG)
![3](https://github.com/lmrs-06/nginx/blob/main/nginx/3.PNG)
![4](https://github.com/lmrs-06/nginx/blob/main/nginx/4.PNG)
![5](https://github.com/lmrs-06/nginx/blob/main/nginx/5.PNG)

## Referencias:
[Pagina de Referencia 1](https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-20-04-es)

[Pagina de Referencia 2](https://www.ochobitshacenunbyte.com/2020/02/24/nginx-balanceo-de-carga-http-en-linux/)


## Licencia:
![lic](https://github.com/lmrs-06/nginx/blob/main/nginx/licencia.png)
