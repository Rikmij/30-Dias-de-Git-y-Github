Github te permite subir el código que tengas en git. Actúa como repositorio central para que todos puedan compartir.
Puedes empujar unos cambios (push) y obtener cambios (pull) que hayan hecho otros.
Lo primero es crear una cuenta de github, y una vez la tengas, añadir tu nombre de usuario en git con
`git config --global user.username <elNombreQueTengas>` (contando mayúsculas) (puedes verificar lo que escribiste con
el comando `git config --global user.username`)

Al subir algo a github, se guarda en sus servidores, convirtiéndolo en un repositorio remoto, y empujando tus 
cambios locales (pushing) lo vas actualizando. Otras personas podrán tener lo más reciente tirando (pulling) de los
cambios desde un remoto (el ordenador de otro)

Los archivos README, .gitignore y license son comunes en proyectos de código abierto (Github te da opción para crearlos
por tí).
Un README describe qué es el proyecto, cómo usarlo y a veces cómo contribuir (o puede estar en un CONTRIBUTING.md)
Un .gitignore es una lista de archivos a los que Git NO debe hacer seguimientos.
Un license describe qué licencia tiene el proyecto, que permite saber a otros cómo puede usar el proyecto

A Git hay que especificarle la dirección de la versión remota en github. Puedes tener varios remotos en tu local, pero hay que especificar el principal, que será el origin.
Para agregar un remoto origin usamos `git remote add origin <URLdegithub>` y ya el repo local sabrá dónde está el de github.

Para añadir cambios hay que hacer **push**. Git trabaja con ramas (branches), y su principal es _main_.
Para "empujar" una rama se usa `git push origin main`

Otros comandos a conocer son:
- Añadir conexiones remotas: `git remote add <NOMBREDELREMOTO> <URL>`
- Modificar URL de un remoto: `git remote set-url <NOMBREDELREMOTO> <URL>`
- Tirar de los cambios: `git pull <NOMBREDELREMOTO> <NOMBREDELBRANCH>`
- Ver direcciones remotas: `git remote -v`
- Empujar cambios: `git push <NOMBREDELREMOTO> <BRANCH>`

Además de crear repositorios, éstos se pueden clonar o bifurcar (fork). Los forks se usan para crear una versión propia del proyecto o contribuir con cambios al repositorio original.
Al hacer fork, esta copia está en tu github, en tu repositorio remoto, no en tu ordenador. Para tenerla en tu ordenador, hay que clonar el proyecto.
Al clonar el proyecto se crea una carpeta automáticamente (no clonar dentro de una carpeta con repositorio Git).
Una vez hecho el fork, se puede clonar con `git clone <URLdelFrok>` y ya entramos a la carpeta con `cd` para hacer lo que tengamos que hacer.
Podemos comprobar las direcciones del fork con `git remote -v`
