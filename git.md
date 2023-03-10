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