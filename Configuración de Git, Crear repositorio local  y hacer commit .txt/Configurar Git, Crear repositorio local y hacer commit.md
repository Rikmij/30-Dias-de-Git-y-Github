## Configuración de Git

Puedes descargar Git desde su [web oficial](https://git-scm.com/) o instalando [Github for desktop](https://desktop.github.com/).  
Puedes comprobar si tienes git instalado ya en la terminal con el comado `git --version`  

Empezamos configurando git ingresando el usuario y un e-mail, para ello usaremos los siguientes comandos:
- `git config --global user.name "nombre que sea"` para el nombre
- `git config --global user.email "el email"` para el correo electrónico

## Crear repositorio

--> Un repositorio es una colección de elementos que tienen una relación, como los archivos que constituyen un proyecto.  

Ya está configurado. Ahora podemos crear un repositorio git local. Para ello podemos crear la carpeta como siempre, o por terminal (como vamos a hacer aquí, que se trata
de aprender a usar git y github, que son programas que funcionan tambié por terminal).  
Para crear este repositorio seleccionas la dirección donde quieras crear la carpeta (te mueves a carpetas internas con `cd "nombre de la carpeta` y hacia carpetas superiores
con `cd ..` (y si quieres ver qué hay dentro de cada carpeta `ls`)) y creas la carpeta con `mkdir "nombre para la carpeta"`. En la carpeta hacer `git init` desde terminal.  

## Crear un commit

--> Un commit es cada punto de guardado de un archivo que hay que comentar. Cada vez que haces un cambio en un archivo, comentas qué cambios has hecho  

Ya creado el repositorio local, podemos empezar a trabajar en él. Con nuestro editor de texto (VSCode por ejemplo) creamos algún archivo y lo guardamos.  
En este punto hacemos un `git status` y saldrá que hay cambios sin guardar, para lo cual debemos añadir los cambios con `git add <nombre del archivo que hayamos añadido>` si lo
estamos creando. Si es un cambio a un archivo existente, podemos hacer los cambios con `git add .`.
Podemos ver los cambios realizados con `git diff` y para hacer efectivos los cambios, hay que hacerles el commit con `git commit -m "descripción de los cambios"`
