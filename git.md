# Git: Una gran herramienta para el control de versiones

Git es un sistema de control de versiones distribuido de código abierto que se utiliza para rastrear cambios en archivos y colaborar en proyectos de software con un equipo de programadores. Fue desarrollado originalmente por Linus Torvalds en 2005 para gestionar el desarrollo del kernel de Linux, pero ahora es ampliamente utilizado en proyectos de todo tipo y tamaño.

## ¿Qué es un sistema de control de versiones?

Un sistema de control de versiones (VCS, por sus siglas en inglés) es una herramienta de software que permite a los desarrolladores rastrear y gestionar los cambios realizados en el código fuente y otros archivos de un proyecto de software.

Un VCS almacena todos los cambios realizados en el código y los archivos, lo que permite a los desarrolladores acceder a versiones anteriores de un archivo, comparar diferentes versiones, fusionar cambios de diferentes desarrolladores y ramas de trabajo, y revertir cambios no deseados.

Los sistemas de control de versiones son particularmente útiles en proyectos de software con varios desarrolladores que trabajan en diferentes partes del proyecto simultáneamente, ya que ayudan a evitar conflictos en el código y permiten una colaboración más eficiente y efectiva. También son útiles para proyectos de una sola persona, ya que genera un control más riguroso del historial y de los cambios realizados en el código fuente.

Hay diferentes tipos de sistemas de control de versiones, como sistemas centralizados (como SVN) y sistemas distribuidos (como Git), cada uno con sus propias ventajas y desventajas.

## ¿Qué hace Git?

Algunas de las funciones principales que ofrece Git son:

- Control de versiones: Permite tener un registro detallado de las modificaciones realizadas en un archivo a lo largo del tiempo, lo que facilita la colaboración y la corrección de errores.

- Gestión de ramas: Permite la creación de diferentes versiones de un mismo proyecto, conocidas como ramas, que se pueden desarrollar de forma independiente y fusionar después.

- Acceso concurrente: Permite que múltiples desarrolladores trabajen simultáneamente en diferentes secciones del mismo proyecto, evitando así conflictos y problemas de sincronización.

- Historial de cambios: Permite revisar los cambios realizados en un archivo a lo largo del tiempo, lo que facilita la identificación de errores y el seguimiento de la evolución del proyecto.

- Restauración de versiones anteriores: Permite recuperar versiones antiguas de un archivo, lo que es útil en caso de errores o fallos en el código.

## ¿Por qué usar Git?

Git es un sistema de control de versiones distribuido, lo que significa que cada desarrollador tiene una copia completa del historial de cambios de un proyecto, incluyendo todos los archivos y metadatos. Esto permite a los desarrolladores trabajar de forma independiente sin tener que conectarse a un servidor central, lo que facilita la colaboración y la gestión de proyectos de gran tamaño.

## Instalación de Git

Para instalar Git en Windows, macOS o Linux, puedes seguir las instrucciones de la [página oficial de Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

## Configuración de Git

Para configurar Git, debes establecer tu nombre de usuario y dirección de correo electrónico. Esto se hace con los siguientes comandos:

```bash
git config --global user.name "Gabriel Romero"
git config --global user.email "gabriel.romero@utec.edu.pe"
```

Utilice el mismo correo electrónico que usó para su cuenta de GitHub. Para verificar que la configuración se haya realizado correctamente, puede ejecutar el siguiente comando:

```bash
git config --list
```

## Creación de un repositorio

¿Qué es un repositorio? Un repositorio es un directorio que contiene todos los archivos de un proyecto, incluyendo el historial de cambios. Los repositorios de Git se almacenan en un directorio oculto llamado `.git`.

Para crear un repositorio, debes ejecutar el siguiente comando:

```bash
git init
```

Este comando crea un nuevo directorio oculto llamado `.git` en el directorio actual. Este directorio contiene todos los archivos necesarios para rastrear los cambios realizados en el proyecto.

Git tiene tres estados principales en los que se pueden encontrar tus archivos: confirmado (committed), modificado (modified), y preparado (staged). 

    - Confirmado: significa que los datos están almacenados de manera segura en tu base de datos local. 
    - Modificado: significa que has modificado el archivo pero todavía no lo has confirmado a tu base de datos. 
    - Preparado: significa que has marcado un archivo modificado en su versión actual para que vaya en tu próxima confirmación. 
    
    - Esto nos lleva a las tres secciones principales de un proyecto de Git: El directorio de Git (Git directory), el directorio de trabajo (working directory), y el área de preparación (staging area). El flujo de trabajo básico en Git es algo así:

    1. Modificas una serie de archivos en tu directorio de trabajo.
    2. Preparas los archivos, añadiéndolos a tu área de preparación.
    3. Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

![git phases Image](https://static.packt-cdn.com/products/9781782168454/graphics/8454OS_01_4.jpg)

## Comandos básicos de Git

### git status
git status es un comando que muestra el estado actual de un repositorio. Este comando es muy útil para verificar si hay archivos que no se han agregado al área de preparación o que no se han confirmado.

### git add
git add es un comando que agrega un archivo al área de preparación. Este comando es muy útil para preparar los archivos antes de confirmarlos.

### git commit
git commit es un comando que confirma los cambios realizados en un archivo y los almacena en el directorio de Git. Este comando es muy útil para confirmar los cambios realizados en un archivo.

Ejemplo:

```bash
$ git commit -m "Primera version del codigo"
[main (root-commit) 57e9b7f] Primera version del codigo
 1 file changed, 1 insertion(+)
 create mode 100644 index.html
```

Si es que no usa el parámetro -m, Git abrirá un editor de texto para que escriba el mensaje de confirmación. Para salir del editor de texto, presione la combinación de teclas Ctrl + X, luego presione la tecla Y y, finalmente, presione la tecla Enter. Otra forma de salir es esc + shift + zz.

### git log
git log es un comando que muestra el historial de confirmaciones de un repositorio. Este comando es muy útil para verificar el historial de confirmaciones de un repositorio.

Ejemplo:

```bash
$ git log
commit 57e9b7f8d7cb553ca46aeef926408e3dd5bbd493 (HEAD -> main)
Author: Gabriel Romero <gabriel.romero@utec.edu.pe>
Date:   Sun Mar 12 17:43:32 2023 -0500

    Correccion de errores en el codigo fuente

commit ac1f44923ad945d53fdb1541359d09e4bba78c5e
Author: Gabriel Romero <gabriel.romero@utec.edu.pe>
Date:   Sun Mar 12 17:42:10 2023 -0500

    Primera version del codigo
```

Si nos fijamos en el historial de confirmaciones, podemos ver que cada confirmación tiene un identificador único (commit hash), un autor, una fecha y una descripción. El identificador único de una confirmación se utiliza para identificar de forma única una confirmación en el historial de confirmaciones.

### git show
git show es un comando que muestra los cambios realizados en un archivo. Este comando es muy útil para verificar los cambios realizados en un archivo.

Ejemplo:

```bash
$ git show pruebas.txt
commit 57e9b7f8d7cb553ca46aeef926408e3dd5bbd493 (HEAD -> main)
Author: Gabriel Romero <gabriel.romero@utec.edu.pe>
Date:   Sun Mar 12 17:43:32 2023 -0500

    Correccion de errores en el codigo fuente

diff --git a/pruebas.txt b/pruebas.txt
index 8b0b5b8..b8b9b5b 100644
--- a/pruebas.txt
+++ b/pruebas.txt
@@ -1,3 +1,3 @@
-Prueba 1
-Prueba 2
-Prueba 3
+Prueba 1.1
+Prueba 2.1
```

En este ejemplo, podemos ver que el comando git show muestra los cambios realizados en el archivo pruebas.txt. En este caso, se eliminaron las líneas 1, 2 y 3 y se agregaron las líneas 1.1 y 2.1.

### git diff
git diff es un comando que muestra los cambios realizados en un archivo comparado con el último commit o el archivo que le indiquemos. Este comando es muy útil para verificar los cambios realizados en un archivo.

Ejemplo:

```bash
$ git diff 57e9b7f8d7cb553ca46aeef926408e3dd5bbd493 ac1f44923ad945d53fdb1541359d09e4bba78c5e
diff --git a/prueba.txt b/prueba.txt
index 5ddc3df..4cf6276 100644
--- a/prueba.txt
+++ b/prueba.txt
@@ -1,7 +1,6 @@
 Git es un sistema de control de versiones distribuido de código abierto diseñado para manejar todo, desde proyectos pequeños a muy grandes, con velocidad y eficiencia.

-Por Pepe Gomez
-Por Juan Perez
+Por Luis Perez

 Gracias por leer este articulo.
```

En este ejemplo, podemos ver que el comando git diff muestra los cambios realizados en el archivo prueba.txt entre las confirmaciones 57e9b7f8d7cb553ca46aeef926408e3dd5bbd493 y ac1f44923ad945d53fdb1541359d09e4bba78c5e. En este caso, se eliminaron las líneas 2 y 3 y se agregó la línea 2.1.

## Branches y Merges en Git

En Git, una rama (branch en inglés) es una línea de desarrollo independiente que permite a los usuarios trabajar en diferentes versiones de un proyecto de forma simultánea. Cada rama puede tener su propia versión del código fuente, y los cambios realizados en una rama no afectan a otras ramas a menos que se fusionen explícitamente.

La fusión (merge en inglés) es la acción de combinar los cambios de dos o más ramas en una sola rama. Cuando se fusionan dos ramas, Git intenta combinar los cambios realizados en cada una de las ramas y aplicarlos a la rama destino.

Un ejemplo de cómo se pueden usar las ramas y la fusión en Git es el siguiente:

Supongamos que estás trabajando en un proyecto en Git y tienes una rama principal (llamada "main") que representa la versión actual del proyecto. Quieres agregar una nueva funcionalidad al proyecto, pero no estás seguro de si funcionará correctamente. En lugar de hacer cambios directamente en la rama "main", puedes crear una nueva rama (llamada "nueva-funcionalidad") y realizar los cambios en esa rama.

```bash
$ git branch nueva-funcionalidad
$ git checkout nueva-funcionalidad
Switched to branch 'nueva-funcionalidad'
```

Ahora estás trabajando en la rama "nueva-funcionalidad", que es una copia exacta de la rama "main" en ese momento. Puedes realizar cambios en la rama "nueva-funcionalidad" sin afectar la rama "main". Cuando hayas terminado de implementar la nueva funcionalidad, puedes fusionar la rama "nueva-funcionalidad" con la rama "main" usando el comando git merge.

```bash
$ git checkout main
$ git merge nueva-funcionalidad
Updating 57e9b7f..ac1f449
Fast-forward
 prueba.txt | 1 +
 1 file changed, 1 insertion(+)
```

Si no hay conflictos entre los cambios realizados en ambas ramas, Git fusionará automáticamente los cambios de la rama "nueva-funcionalidad" con la rama "main". Si hay conflictos, Git te pedirá que los resuelvas manualmente antes de continuar con la fusión.

Este ejemplo ilustra cómo se pueden usar las ramas y la fusión en Git para desarrollar nuevas funcionalidades sin afectar la versión actual del proyecto y luego fusionar los cambios en la rama principal de forma segura y controlada.