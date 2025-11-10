# __Manual-Git__  
Manual de comandos básicos de Git.

## `git init`  
Inicializa un repositorio local en la carpeta actual. Este comando crea la carpeta oculta `.git`, donde se guarda toda la información del historial, las ramas y la configuración del proyecto. Se utiliza al comenzar un proyecto desde cero para ponerlo bajo control de versiones.

## `git clone`  
Clona un repositorio remoto en tu máquina, copiando todos los archivos, el historial y las ramas. Es la forma de obtener una copia exacta de un proyecto existente para empezar a trabajar en él.

## `git add`  
Añade archivos al área de preparación (*staging area*), indicando qué cambios se incluirán en el próximo commit. Puede usarse con archivos específicos (`git add archivo.txt`) o con todos los cambios (`git add .`).

## `git commit`  
Guarda los cambios preparados en el historial del repositorio, creando un punto de control con un mensaje descriptivo. Es recomendable que el mensaje explique claramente qué se ha cambiado y por qué.

## `git log`  
Muestra el historial de commits realizados, incluyendo autor, fecha y mensaje. Con opciones como `--oneline` o `--graph` se puede ver un historial más compacto y visual, lo que facilita seguir la evolución del proyecto.

## `git checkout`  
Permite cambiar entre ramas o restaurar archivos a un estado anterior. Por ejemplo, `git checkout nombre-rama` te mueve a otra rama. También puede usarse para volver un archivo a la versión guardada en el último commit.

## `git branch`  
Crea nuevas ramas o lista las existentes en el repositorio. Por ejemplo, `git branch nueva-rama` crea una rama llamada *nueva-rama*. Trabajar con ramas permite desarrollar nuevas funcionalidades sin afectar la rama principal.

## `git push`  
Envía los commits locales al repositorio remoto, actualizando la rama correspondiente. Por ejemplo, `git push origin main` sube los cambios a la rama *main* en GitHub. Si la rama remota no existe, se puede usar `git push -u origin nombre-rama` para crearla y vincularla.

## `git pull`  
Descarga y fusiona los cambios del repositorio remoto en tu rama local. Es equivalente a hacer `git fetch` seguido de `git merge`. Se utiliza para mantener tu copia local sincronizada con el repositorio remoto.

## `git merge`  
Fusiona el contenido de una rama en la rama actual, integrando sus commits. Por ejemplo, `git merge feature-x` combina la rama *feature-x* con la rama en la que estás trabajando. Si hay conflictos, deben resolverse manualmente antes de completar la fusión.
