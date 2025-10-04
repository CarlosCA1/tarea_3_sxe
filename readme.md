## Tarea 03

1. Descarga la imagen "alpine" sin arrancarla y comprueba que está en tu equipo.

Una vez instalado Docker, descargamos la última versión estable de Alpine Linux desde el registro oficial de Docker Hub (el repositorio público de imágenes Docker) con "pull":

````
docker pull alpine
````

Ejemplo en terminal:

![Imagen](images/1.png)

2. Crea un contenedor sin ponerle nombre. ¿está arrancado? Obtén el nombre

Creamos un nuevo contenedor basado en la imagen Alpine Linux (docker run alpine), lo ejecutamos en segundo plano y lo preparamos para que pueda usarse de forma interactiva.

-d: el contenedor se ejecuta en segundo plano.

-i: mantiene la entrada estándar abierta. Esto permite que luego puedas ejecutar comandos dentro del contenedor.

-t: asigna una terminal al contenedor.
````
docker run -dit alpine
````

Para ver los contenedores en ejecución:
````
docker ps
````

Para obtener solo el nombre de los mismos:
````
docker ps
````


Ejemplo en terminal:

![Imagen](images/2.png)