# Comandos de git

Breve descripción de los comandos que hemos estado usando para familiarizarnos con git (y github!)

## Creando repositorios desde cero

Cuando queremos comenzar a añadir el control de versiones en un directorio existente debemos inicializar el repositorio git con:

>git init

Una vez inicializado ya tenemos el repositorio preparado y podemos pasar al [ciclo de vida normal de uso de git](#Ciclo-de-vida-del-desarrollo-con-git-Untracked-staging-commit-y-remoto)


## Importando repositorios existentes

También se puede partir de un repositorio existente en remoto, para ello obtendremos la URL de este repositorio y usaremos git clone. Por ejemplo, este repositorio está alojado en github, podemos clonarlo con:

> git clone https://github.com/jojelupipa/repo02.git


## Ciclo de vida del desarrollo con git: Untracked, staging, commit y remoto

Una vez dispongamos de un directorio y nos situemos dentro de él, podemos comenzar a trabajar directamente en nuestro repositorio de git. Podremos crear archivos, añadirlos a la zona de staging, realizar el commit y, si queremos hacer uso de un repositorio remoto, subirlo a algún repositorio como github, gitlab o bitbucket.

### Añadiendo archivos a nuestro commit

> git add <nombre de archivo>

Permite añadir un archivo al commit que estemos preparando, para añadirlo a una "versión" del producto en desarrollo.

### Cerrando el commit, creando una nueva versión

> git commit -m "Mensaje del commit"

Finalizamos los cambios que queramos añadir a la nueva versión y le añadimos un comentario para conseguir que tenga una descripción sin tener que entrar a ver qué se ha hecho exactamente.

### Subiendo y descargando de repositorios remotos

Asumiendo que se han configurado un origen remoto (con `git remote add <url>`) y se ha establecido alguna rama upstream (por ejemplo master) se puede usar:

> git push
> git pull

Para enviar o recuperar el estado actual del repositorio local al remoto o viceversa.

*Nota: Cuando clonas un repositorio con git clone, el origen remoto y la configuración del upstream se establece por defecto a la rama master*.

¡Muchas gracias por su atención!

![Pato](https://th.bing.com/th/id/OIP.tCgvRG-qYasp4ZsFn9zZDgHaHa?pid=ImgDet&rs=1)
