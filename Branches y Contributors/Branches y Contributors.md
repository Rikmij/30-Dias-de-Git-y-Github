Los repositorios de git trabajan con ramas para separar el trabajo.
Normalmente en un proyecto grupal cada persona crea una branch (rama), trabaja en ella (y la rama principal (main) se mantiene estable), y ya cuando acabas fusionas tu rama con la main.

Al crear una rama, Git copia todo lo que hay en la rama actual y lo pone en la que has creado. Se puede comprobar la rama en la que estás actualmente con un `git status`. El comado para crear una
rama nueva es `git branch <NombredelaBranch>`, y te pasas a esa rama con `git checkout <NombredelaBranch>`.

Cuando hayas hecho todos los cambios necesarios, habrá que guardar los cambios. Con `git status` para comprobar la rama y los cambios, un `git add <NombredelaCarpeta/NombredelArchivo>`
y un commit con `git commit -m "mensaje"`, y ya hacerle un push para subir los cambios `git push origin <NombredelaBranch>`

- Para renombrar una rama, se usa `git branch -m <NuevoNombredelaBranch>`
- Puedes crear y moverte a la rama a la vez usando `git checkout -b <NombredelaBranch`
- Puedes ver un listado de las ramas con `git branch`

Una de las cosas fundamentales de Github es trabajar con gente desde cualquier lugar, y para eso hay que añadir colaboradores/contribuyentes.
Para eso, en la página de Github del repositorio, entras a **settings**, y en los colaboradores puedes añadir a quien quieras.
