$ aptitude install git

$ git config --global user.name "Argenis Osorio" // Asignamos el nombre de usuario que será la firma del usuario en cada commit

$ git config --global user.email aosorio@example.com // igualmente el correo que siempre acompañara al autor de cada commit

$ git init // Inicializar un repositorio

$ git status // Muestra el estado actual de la rama, como los cambios que hay sin commitear.

$ git add * // Agregar todos los archivos al seguimiento de Git.

ó

$ git add . // Agregar todos los archivos al seguimiento de Git.

$ git add fichero1.xxx fichero2.xxx fichero3.xxx // Agregando ficheros específicos al seguimiento de git.

$ git commit -m "Primer commit del proyecto" //Hacer un commit al proyecto, se activara la rama master por defecto.

$ git log // Podemos ver todos los commits que se han hecho a un proyecto, fecha, autor, etc...

$ git branch // Lista todas las ramas locales.

$ git commit --amend -m "comentario commit corregido" // Corregir algun error en el texto del último commit

$ git commit --amend // Corregir un error en el commit, abrira un editor de texto

$ git reset --hard HEAD~1 // Borrar el ultimo commit hecho.

$ git branch Nombre_Rama // Crear una rama.

$ git checkout -b Nombre_Rama // Crear una rama y cambiarse a ella.

$ git branch -d Nombre_Rama // Borrar una rama, se debe estar en otra rama para borrarla

$ git branch -D Nombre_Branch // Forzar el borrado de una rama, a veces no se dejan borrar si hay cambios sin guardar.

$ git push origin :the_remote_branch // Borrar una rama del repositorio remoto
<h1>guia rapida de github<h1>

$ git checkout Nombre_Rama // Cambiarse de rama

$ git push -f origin master // git push -f <remote> <branch> forzar el push para sobreescribir los ficheros en el repositorio remoto.
