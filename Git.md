# Gestión de la Configuración en GitHub
La gestión de la configuración en GitHub se refiere a la capacidad de controlar y mantener diferentes versiones de un proyecto o aplicación en un repositorio de GitHub.

GitHub es una plataforma muy popular para la gestión del control de versiones y permite a los desarrolladores colaborar en un mismo proyecto y mantener un historial de cambios en el código.

## A Que es?
GitHub es una plataforma de alojamiento de código fuente y gestión de proyectos que utiliza la gestión de la configuración para controlar y rastrear los cambios en el código y otros elementos del proyecto. Al alojar el código en un repositorio, GitHub permite a los desarrolladores trabajar en el código de forma colaborativa, y ofrece herramientas para gestionar y controlar las diferentes versiones del código.

Con GitHub, los desarrolladores pueden crear ramas o "branches" del código para trabajar en nuevas funcionalidades o arreglar errores sin afectar al código base. Una vez que las nuevas funcionalidades o correcciones se han completado, se puede integrar o "merge" el código de vuelta al código base.

Además, GitHub también ofrece herramientas para la gestión de problemas, seguimiento de errores y solicitudes de pull requests, lo que permite a los desarrolladores colaborar y trabajar juntos de manera más eficiente en proyectos de software. En resumen, GitHub utiliza la gestión de la configuración para facilitar el trabajo colaborativo en proyectos de software, permitiendo a los desarrolladores trabajar de manera más eficiente y reduciendo la posibilidad de conflictos en el código.

## B ¿Por qué necesitamos la administración de la configuración del software? 
La gestión de la configuración del software es importante por varias razones:

Control de versiones: La gestión de la configuración permite a los desarrolladores controlar y rastrear los cambios realizados en el código fuente y otros elementos del proyecto a lo largo del tiempo. Esto les permite volver a versiones anteriores si algo sale mal o si necesitan volver a una versión anterior de un proyecto.

Trabajo colaborativo: La gestión de la configuración permite que varios desarrolladores trabajen juntos en un mismo proyecto, al mismo tiempo. Los cambios realizados por cada desarrollador pueden ser integrados fácilmente y controlados para evitar conflictos en el código.

Seguimiento de problemas: La gestión de la configuración también permite que los desarrolladores realicen un seguimiento de los problemas o errores del software y realicen cambios específicos para corregirlos.

Automatización de procesos: La gestión de la configuración permite la automatización de muchos procesos de software, lo que ahorra tiempo y reduce errores. Por ejemplo, los procesos de compilación, pruebas y distribución de software pueden ser automatizados a través de herramientas de gestión de la configuración.

## C Tareas en el proceso de gestión de la configuración
En GitHub, algunas de las tareas que se realizan en el proceso de gestión de la configuración del software son:

Crear un repositorio: El primer paso es crear un repositorio donde se almacenará el código fuente y otros elementos del proyecto.

Control de versiones: Los cambios en el código fuente y otros elementos del proyecto se realizan en diferentes ramas (branches) y se integran de vuelta al repositorio principal cuando están listos.

Trabajo colaborativo: Los desarrolladores trabajan en diferentes ramas del proyecto y pueden colaborar en un mismo archivo, realizando cambios y comentarios que son revisados y aprobados antes de ser integrados al repositorio principal.

Seguimiento de problemas: Los problemas y errores se registran en la plataforma, se asignan a un desarrollador y se realiza un seguimiento hasta que se resuelve.

Automatización de procesos: Se pueden utilizar herramientas de integración continua (CI) para automatizar procesos como la compilación, pruebas y distribución de software.

Comentarios y revisiones: Los desarrolladores pueden revisar los cambios realizados por otros, comentar y sugerir mejoras antes de ser integrados al repositorio principal.

Control de acceso: Se puede limitar el acceso al repositorio a los desarrolladores y colaboradores que necesiten trabajar en el proyecto.

## D Identificación de la configuración
La identificación de la configuración en GitHub es un proceso que consiste en identificar y controlar los elementos del proyecto que serán gestionados en el repositorio de GitHub. Algunos de los elementos que se pueden incluir en la identificación de la configuración son:

Código fuente: El código fuente es uno de los principales elementos que se identifican en la configuración de un proyecto en GitHub. El código se puede dividir en diferentes archivos y carpetas, y se puede controlar su versión a través de ramas (branches) y etiquetas (tags).

Dependencias: Las dependencias del proyecto, como librerías externas, módulos y paquetes, también deben ser identificadas y controladas en el repositorio de GitHub.

Documentación: La documentación del proyecto, como los archivos README, las guías de usuario, los manuales técnicos, entre otros, también se deben identificar y controlar en el repositorio.

## E Participantes del proceso 
En GitHub, los participantes en el proceso de gestión de la configuración pueden variar dependiendo del proyecto y la organización, pero algunos de los roles más comunes son:

Propietario del repositorio: El propietario del repositorio es la persona o equipo que es responsable del proyecto y tiene control completo sobre el repositorio de GitHub.

Desarrolladores: Los desarrolladores son las personas encargadas de escribir el código y contribuir al proyecto. Pueden hacer cambios en el repositorio y proponer solicitudes de extracción (pull requests) para que sus cambios sean revisados y aprobados antes de ser integrados al repositorio principal.



# ¿Qué es GIT?

Es un sistema de control de versiones de software distribuido de código abierto, diseñado para manejar distintos tipos de proyectos de manera eficiente y confiable. Fue desarrollado originalmente por Linus Torvalds en 2005 para el desarrollo del kernel de Linux, pero hoy en día se utiliza ampliamente en todo tipo de proyectos de software.

Permite a los desarrolladores trabajar en equipo en el mismo proyecto de manera concurrente, manteniendo un historial completo y detallado de todos los cambios realizados en el código fuente. Esto permite a los desarrolladores revertir a versiones anteriores del proyecto si algo sale mal, rastrear bugs y colaborar en la mejora del software de manera eficiente.

Funciona mediante la creación de repositorios, que son lugares donde se almacena el código fuente del proyecto y se lleva un registro de los cambios realizados. Los desarrolladores pueden clonar un repositorio para trabajar en su propia copia del proyecto, realizar cambios y luego enviar sus cambios de regreso al repositorio principal a través de un proceso conocido como **pushing** y **pulling** de los cambios realizados por otros colaboradores.

## Diferencias entre Git y otros sistemas de control de versiones

Mientras que la mayoría de los otros sistemas almacenan información como una lista de cambios basados ​​en archivos, Git piensa en sus datos más como una serie de instantáneas de un sistema de archivos en miniatura. Con Git, cada vez que se realiza un **commit** o se guarda el estado del proyecto, Git básicamente toma una imagen de cómo se ven todos sus archivos en ese momento y almacena una referencia a esa instantánea. Para ser eficiente, si los archivos no han cambiado, Git no vuelve a almacenar el archivo, solo un enlace al archivo idéntico anterior que ya ha almacenado. En resumen, la diferencia sería en que Git piensa en sus datos más como un flujo de instantáneas.

## Estados y secciones

Hay tres estados en los que pueden estar los archivos en Git

- `modified`: indica que se ha cambiado el archivo, pero esté no ha sido ingresado a la base de datos todavía 
- `staged`: indica que se ha marcado un archivo modificado en su versión actual para pasar a su próxima instantánea de confirmación.
- `committed`: indica que los datos se almacenaron de forma segura en la base de datos local

Con base a los estados anteriores se puede definir tres secciones principales de un proyecto Git:

-   `working tree`: es una comprobación única de una versión del proyecto. Acá los archivos se extraen de la base de datos comprimida en el directorio Git y se colocan en el disco para su uso.
-   `staging area`: esta área es un archivo, generalmente contenido en su directorio Git, que almacena información sobre que se incluirá en el próximo commit.
-   `.git directory (repository)`: es donde Git almacena los metadatos y la base de datos de objetos para su proyecto. Esta es la parte más importante de Git y es lo que se copia cuando clonas un repositorio desde otra computadora.

El flujo de trabajo básico de Git sería:

-   Se modifican archivos en el working tree.
-   Se organiza selectivamente solo aquellos cambios que se desean sean parte del próximo commit, que agrega solo esos cambios al staging area.
-   Se realiza un commit, que toma los archivos tal como están en el staging area y almacena esa instantánea de forma permanente en el directorio de Git.

# Comandos Básicos y Avanzados

Estos son todos los comandos de **Git** disponibles en la versión más reciente. No hay más comandos que puedan ser usados en **Git** que no se encuentren en esta lista. Algunos comandos pueden tener opciones y argumentos adicionales, pero todos los comandos fundamentales están incluidos en la lista.

## Configuración

-   `git config`: Lee o establece opciones de configuración para Git.
	```
	git config --global user.name "Tu nombre" 
	git config --global user.email "tu@email.com"
	```
-   `git help`: Muestra información de ayuda sobre un comando específico.
	```
	git help <comando>
	```

## Comandos de inicio

-   `git init`: Crea un nuevo repositorio de Git vacío en la carpeta actual.
	 ```
	git init
	```
-   `git clone`: Clona un repositorio existente en una nueva carpeta.
	 ```
	git clone <url_del_repositorio>
	```

## Comandos básicos

-   `git add`: Agrega un archivo a la zona de preparación para que se incluya en el próximo commit.
	 ```
	git add <nombre_del_archivo>
	```
-   `git status`: Muestra el estado actual del repositorio, incluyendo los archivos que han sido modificados, añadidos o eliminados.
	 ```
	git status
	```
-   `git commit`: Crea un nuevo commit con los cambios en la zona de preparación y un mensaje descriptivo.
	 ```
	git commit  -m "mensaje descriptivo"
	```
-   `git rm`: Elimina un archivo del índice y del árbol de trabajo.
	 ```
	git rm <nombre_del_archivo>
	```
-   `git mv`: Cambia el nombre de un archivo y lo prepara para el commit.
	 ```
	git mv <nombre_antiguo>  <nombre_nuevo>
	```
-   `git restore`: Descarta los cambios realizados en el árbol de trabajo.
	 ```
	git restore <nombre_del_archivo>
	```

## Comandos de historial

-   `git log`: Muestra un historial de todos los commits realizados en el repositorio.
	 ```
	git log
	```
-   `git diff`: Muestra las diferencias entre dos commits o entre el commit y el árbol de trabajo.
	 ```
	git diff <commit1>  <commit2>
	```
-   `git show`: Muestra la información detallada de un commit específico.
	 ```
	git show <identificador_del_commit>
	```
-   `git blame`: Muestra quién ha modificado cada línea de un archivo específico.
	 ```
	git blame <nombre_del_archivo>
	```
-   `git grep`: Busca una cadena de texto en todos los archivos del repositorio.
	 ```
	git grep <cadena_de_texto>
	```
-   `git bisect`: Encuentra el primer commit que introdujo un error en el repositorio.
	 ```
	git bisect start 
	git bisect good <commit_bueno> 
	git bisect bad <commit_malo> 
	git bisect run <comando_para_verificar_el_estado>
	```

## Comandos de ramas y etiquetas

-   `git branch`: Muestra una lista de todas las ramas disponibles en el repositorio.
	``` 
	git branch 
	```
-   `git checkout`: Cambia a la rama o commit especificado.
	``` 
	git checkout nombre_de_la_rama
	```
-   `git merge`: Combina la rama especificada con la rama actual.
	``` 
	git merge nombre_de_la_rama
	```
-   `git tag`: Crea, lista o borra una etiqueta.
	``` 
	git tag nombre_de_la_etiqueta
	```
-   `git branch -d`: Elimina una rama que ha sido completamente fusionada en el repositorio.
	``` 
	git branch -d nombre_de_la_rama 
	```
-   `git branch -D`: Fuerza la eliminación de una rama, incluso si no ha sido completamente fusionada.
	``` 
	git branch -D nombre_de_la_rama
	```
-   `git branch -m`: Cambia el nombre de una rama.
	``` 
	git branch -m nuevo_nombre_de_la_rama 
	```
-   `git tag -a`: Crea una etiqueta anotada con un mensaje detallado.
	``` 
	git tag -a nombre_de_la_etiqueta -m "Mensaje detallado de la etiqueta"
	```
-   `git tag -d`: Elimina una etiqueta existente.
	``` 
	git tag -d nombre_de_la_etiqueta
	```

## Comandos remotos

-   `git remote`: Muestra una lista de todos los repositorios remotos disponibles.
	``` 
	git remote
	```
-   `git fetch`: Descarga los cambios del repositorio remoto sin fusionarlos con el repositorio local.
	``` 
	git fetch nombre_del_repositorio_remoto
	```
-   `git pull`: Descarga los cambios del repositorio remoto al repositorio local y fusiona los cambios.
	``` 
	git pull nombre_del_repositorio_remoto nombre_de_la_rama
	```
-   `git push`: Sube los cambios locales al repositorio remoto.
	``` 
	git push nombre_del_repositorio_remoto nombre_de_la_rama
	```
-   `git remote add`: Agrega un nuevo repositorio remoto al repositorio local.
	``` 
	git remote add nombre_del_repositorio_remoto URL_del_repositorio_remoto
	```
-   `git remote rm`: Elimina un repositorio remoto del repositorio local.
	``` 
	git remote rm nombre_del_repositorio_remoto
	```
-   `git remote set-url`: Cambia la URL del repositorio remoto existente.
	``` 
	git remote set-url nombre_del_repositorio_remoto URL_nueva_del_repositorio_remoto
	```
-   `git remote show`: Muestra información detallada sobre un repositorio remoto específico.
	``` 
	git remote show nombre_del_repositorio_remoto
	```

## Comandos de anotación y corrección de errores

-   `git commit --amend`: Añade los cambios actuales al último commit.
	``` 
	git commit --amend
	```
-   `git reset`: Deshace los cambios realizados en el último commit.
	``` 
	git reset HEAD~1
	```
-   `git revert`: Crea un nuevo commit que deshace los cambios realizados en un commit específico.
	``` 
	git revert <tu commit>
	```
-   `git cherry-pick`: Aplica los cambios de un commit específico en la rama actual.
	``` 
	git cherry-pick <tu commit>
	```

## Comandos avanzados

-   `git rebase`: Cambia la base de la rama actual a la rama especificada.
	``` 
	git rebase <tu rama>
	```
-   `git reflog`: Muestra un registro de todas las referencias del repositorio.
	``` 
	git reflog
	```
-   `git submodule`: Muestra una lista de submódulos en el repositorio.
	``` 
	git submodule
	```
-   `git worktree`: Crea y administra árboles de trabajo adicionales
	``` 
	git worktree add ../my-feature-branch
	```

## Comandos de colaboración

-   `git clone --bare`: Crea un clon sin árbol de trabajo de un repositorio existente.
	``` 
	git clone --bare https://github.com/user/repo.git
	```
-   `git pull --rebase`: Descarga los cambios del repositorio remoto y aplica los cambios locales por encima de los cambios remotos.
	``` 
	git pull --rebase origin main
	```
-   `git push --force`: Fuerza la actualización del repositorio remoto con los cambios locales.
	``` 
	git push --force origin feature-branch
	```

## Comandos de depuración y optimización

-   `git fsck`: Muestra una lista de objetos corruptos en el repositorio.
	``` 
	git fsck
	```
-   `git gc`: Optimiza y limpia el repositorio, eliminando los objetos no utilizados.
	``` 
	git gc
	```
-   `git stash`: Guarda temporalmente los cambios no commitados en una pila de cambios y los restaura más tarde.
	``` 
	git stash save "mensaje del stash"
	```
-   `git clean`: Elimina los archivos no rastreados del árbol de trabajo.
	``` 
	git clean -f
	```

## Comandos de flujo de trabajo

-   `git cherry`: Muestra los commits que no se han fusionado en una rama específica.
	``` 
	git cherry <branch-a> <branch-b>
	```
-   `git format-patch`: Crea parches de correo electrónico de los cambios realizados en un rango de commits.
	``` 
	git format-patch <desde>..<hasta>
	```
-   `git merge-base`: Encuentra el commit base común entre dos ramas.
	``` 
	git merge-base <branch-a> <branch-b>
	```
-   `git rebase --interactive`: Permite la edición interactiva de los commits durante un rebase.
	``` 
	git rebase -i <commit>
	```
-   `git worktree add`: Crea un nuevo árbol de trabajo y lo asocia con una rama específica.
	``` 
	git worktree add <ruta>  <branch>
	```
