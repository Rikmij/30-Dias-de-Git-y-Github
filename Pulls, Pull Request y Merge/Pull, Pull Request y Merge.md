Para tener al día los repositorios con todos los cambios (especialmente si estás trabajando con alguien), hay que tirar **(pull)** de los cambios que se han añadido al repositorio.
- Para hacer el pull, se usa el comando `git pull <NombredelRepoRemoto> <NombredelaBranchRemota>`
- Para ver los cambios `git fetch --dry-run`

Cuando se trabaja en un proyecto (en tu proyecto fork), van cambiando cosas, añadiendo y mejorándolo, y querrás enviar esos cambios al repositorio original. Eso es hacer una _pull request_
(pedirles que tiren de esos cambios al repo original).
Muchas veces, Github detecta automáticamente si has empujado (push) una branch a un fork y te mostrará un aviso. Puedes hacer la PR (pull request) desde ahí, si no, en el botón de "New Pull Request",
y eliges la rama que tiene los cambios.
A continuación verás una página con los commits y cambios, y enlazará el repositorio con (si la tuviera) documentación de contribución (documentación en que los propietarios describen
cómo contribuir al proyecto). Si todo está correcto, sólo falta esperar que te acepten la PR.

Cuando aceptan la PR, la rama se fusiona en el repositorio de Github, pero también se puede fusionar en el local. Para eso, hay que ir a la rama a la cual quieres fusionar y poner
el comando `git checkout gh-pages`, para decirle desde la rama que quieres traer los cambios (con `git merge <NombredelaBranch>`).
Ya está todo añadido, puedes borrar la/s rama/s innecesarias con `git branch -d <NombredelaBranch>, y eliminarla de Github con `git push <NombredelRemoto> --delete <NombredelaBranch>`.

Por último, el repositorio original ha cambiado, y si tiras desde upstream (el original) tendrás la última versión.
Para tirar de ella habría que usar `git pull upstream gh-pages`
