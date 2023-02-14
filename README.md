<h1>Docker + Python</h1>
En esta tarea, vamos a hacer un contenedor de docker con Python. Para empezar, vamos a probar este código:

```docker run -it --rm --name my-running-script -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python your-daemon-or-script.py```
## Explicación del código

``` docker``` Es el comando básico para ejecutar Docker.  

``` run ``` Es el comando para ejecutar el contenido.

`-it` Dos opciones que valen para interactuar con el terminal del contenedor.

`--rm` Borra el contenedor después de ejecutarlo.

`-v` Define el mapeo del volumen que está a continuación.

`"PWD"` El directorio donde estamos.

`/usr/src/myapp` El directorio del contenedor.

`-w` Es el directorio de trabajo.

`python:3` Imagen de la que se creara el contenedor.

`"python your-daemon-or-script.py"` Es el contenido para ejecutar dentro del contenedor.