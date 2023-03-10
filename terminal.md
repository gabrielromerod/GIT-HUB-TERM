# La Terminal

En esta sección aprenderemos la historia de la terminal, y cómo usarla para ejecutar comandos escenciales con el objetivo de poder usar Git y GitHub.

## Introducción a la terminal - La historia de la computación
Antes de empezar a trabajar con Git, es necesario conocer lo que es la terminal. Para comenzar este viaje, es necesario dar un recorrido por la historia de la computación.

Corrian los años 80 con la aparición de MS-DOS, un sistema operativo que permitía a los usuarios interactuar con la computadora a través de comandos.

Estos comandos eran escritos en una ventana de texto, la cual se llamaba terminal. Cosas sencillas que hacemos en nuestro día a día con la computadora, como abrir un archivo, copiarlo, moverlo, etc., se hacían a través de comandos. Es decir, los clicks que hacemos con nuestro mouse, se hacían con comandos en la terminal.

![MS-DOS](https://media.wired.com/photos/5932672e5c4fbd732b552457/master/w_2560%2Cc_limit/MSDOS.jpg)

El uso de comandos generó una barrera de entrada para muchas personas, por lo que se empezó a desarrollar una interfaz gráfica para que las personas pudieran interactuar con la computadora de una manera más sencilla tal como lo hacemos hoy en día.

Para ello una empresa llamada Microsoft, desarrolló una interfaz gráfica para el sistema operativo MS-DOS, la cual se llamó Windows. Windows fue un éxito, y que años después se convirtió en el sistema operativo más usado en la historia de la computación.

![Windows 1985](https://upload.wikimedia.org/wikipedia/en/4/4e/Windows1.0.png)

La salida de Windows, hizo que muchas personas dejaran de usar la terminal, y se centraran en la interfaz gráfica. Sin embargo, la terminal no desapareció, y sigue siendo usada principalmente por desarrolladores.

Entre sus principales ventajas, se encuentra la velocidad con la que se pueden ejecutar comandos, y la capacidad de automatizar tareas. 

Por ejemplo, si queremos copiar un archivo de un directorio a otro, podemos hacerlo con un solo comando, en lugar de hacerlo con el mouse. Una tarea que puede parecer sencilla, puede ser tediosa si se tiene que hacer muchas veces, y es ahí donde la terminal se vuelve muy útil. Así mismo conectarse a un servidor remoto, o ejecutar un script, se vuelve mucho más sencillo con la terminal.

##  Introducción a la terminal - Tipos de terminales

Cada sistema operativo tiene su propia terminal, y cada una de ellas tiene sus propias características. En esta sección aprenderemos sobre la terminal de Windows, Linux y Mac.

### Terminales de Windows

En Windows, la terminal principal se llama **PowerShell**. Esta terminal es una alternativa a la terminal de comandos de Windows, la cual se llama **CMD**.

La terminal de comandos de Windows **CMD** fue la primera terminal que se usó en Windows, y es la que se usaba en la mayoría de las computadoras antes de la aparición de Windows 10. Sin embargo, la terminal de comandos de Windows tiene algunas limitaciones, por lo que Microsoft creó PowerShell, la cual es una terminal más poderosa y de sintaxis similar a la de Linux.

 1. Windows Command Prompt (CMD): El símbolo del sistema (en inglés, 'Command Prompt', también conocido como cmd.exe o simplemente cmd) es el intérprete de comandos.

    ![Command Prompt Image](https://upload.wikimedia.org/wikipedia/commons/b/b3/Command_Prompt_on_Windows_10_RTM.png)
    
    2. Windows Power Shell: Se considera la evolución del CMD, aumenta la cantidad de funciones y optimiza los procesos previos.

    ![Power Shell Image](https://www.muycomputerpro.com/wp-content/uploads/2019/04/PowerShell7.jpg)


### Terminales de Linux y Mac

- MAC y Linux cuentan con famoso un shell llamado Unix, dicho shell es más conocido como bash. Dentro de sus principales caracteristicas permite la integracion de herramientas para desarrolladores con facilidad.

    - Ubuntu Terminal:
    
    ![Ubuntu Terminal Image](https://www.ionos.es/digitalguide/fileadmin/DigitalGuide/Screenshots/ubuntu-bash.png)

    - Mac OS Terminal:

    ![Mac OS Terminal Image](https://tecno-adictos.com/wp-content/uploads/2021/06/Como-usar-la-terminal-macOS-una-guia-para-principiantes.png)

Nota: Una shell es un programa que permite a los usuarios interactuar con el sistema operativo. En otras palabras, es un intérprete de comandos. La shell más popular es Bash, la cual es la shell por defecto en la mayoría de las distribuciones de Linux.

## Introducción a la terminal - Comandos básicos

### ¿Cómo abrir la terminal?

La terminal esta disponible en todos los sistemas operativos, y se puede abrir de diferentes maneras. 

- Windows:

En Windows, la terminal se puede abrir de muchas maneras, pero la más sencilla es a través de la barra de búsqueda:

1. Abrimos la barra de búsqueda y escribimos **PowerShell**:

![PowerShell](https://i.imgur.com/vgAqKO0.png)

2. Le damos click al PowerShell que aparece en la barra de búsqueda y se abre la terminal:

![PowerShell](https://i.imgur.com/K6jOFPu.png)

- Linux y Mac:

Para abrir la terminal en Linux o Mac, podemos usar la combinación de teclas **Ctrl + Alt + T**.

Terminal en Linux:

![Linux Terminal](https://ubuntucommunity.s3.dualstack.us-east-2.amazonaws.com/original/2X/b/ba76cbf3dc8dc2cc94d26dd61c7aad3cedcd5102.png)

Terminal en Mac:

![Mac Terminal](https://media.idownloadblog.com/wp-content/uploads/2021/12/Terminal-Command-Window-Mac.png)

### Comandos básicos

Ahora que ya sabemos cómo abrir la terminal, es hora de aprender los comandos básicos que se usan en la terminal.

A diario nosotros nos movemos por la computadora usando el mouse, pero en la terminal se usan comandos para moverse por la computadora. Estos comandos se llaman **comandos de navegación**.

El explorador de archivos de Windows se llama **Explorador de archivos**, y en la terminal se llama **Directorio**. En la terminal, el directorio actual se llama **Directorio de trabajo**.

Explorador de archivos en Windows:

![Windows Explorer](https://www.adslzone.net/app/uploads-adslzone.net/2020/10/panel-acceso-rapido-655x500.jpg)

Explorador de archivos en Linux:

![Linux Directory](https://ubunlog.com/wp-content/uploads/2018/02/Nautilus.jpg)

Explorador de archivos en Mac: Más conocido como Finder en Mac, es el explorador de archivos por defecto en Mac.

![Mac Finder](https://i.blogs.es/81404d/es1/1366_2000.jpg)

Es importante tener en cuenta el explorador de archivos que se usa en cada sistema operativo, ya que en la terminal nos movemos por los directorios, y no por los exploradores de archivos.

Los directorios se organizan en una estructura de árbol, y el directorio raíz es el directorio más alto de la estructura. En Windows, el directorio raíz se llama **C:\**, y en Linux y Mac se llama **/**.

> C:\ es el directorio raíz en Windows

> / es el directorio raíz en Linux y Mac

En la terminal, el directorio raíz se llama **Directorio raíz**.

Si quiere saber más sobre la estructura de directorios, puede leer el artículo [¿Qué es un directorio en informática ](https://www.hostgator.mx/blog/que-es-un-directorio/).

Ahora que ya sabemos cómo se organizan los directorios, es hora de aprender los comandos de navegación.

#### Comandos de navegación

Los comandos de navegación se usan para moverse por los directorios. Estos comandos son:

  * **pwd**: Muestra el directorio de trabajo actual.
  * **cd**: Cambia el directorio de trabajo actual.
    * **cd ..**: Cambia al directorio padre del directorio de trabajo actual.
  * **ls**: Muestra los archivos y directorios del directorio de trabajo actual.
  * **mkdir**: Crea un directorio.
  * **touch**: Crea un archivo.
  * **rm**: Elimina un archivo.
  * **rm -r**: Elimina un directorio.
  * **mv**: Mueve un archivo o directorio.
  * **cp**: Copia un archivo o directorio.
  * **cat**: Muestra el contenido de un archivo.
  * **clear**: Limpia la pantalla de la terminal.

1. cd - Change Directory permite moverse entre directorios una actividad que hacemos a diario en el explorador de archivos:
![Change Directory Image](https://generalassembly.github.io/prework/cl/Graphics/terminal_cd.gif)

2. ls - List Files permite ver las carpetas y archivos:
![List Files Image](https://www.solvetic.com/uploads/monthly_03_2017/tutorials-7463-0-36962500-1489423518.jpg)

3. dir - List Files permite ver las carpetas y archivos en Windows:
![List Files Image](https://www.solvetic.com/uploads/monthly_03_2017/tutorials-7463-0-36962500-1489423518.jpg)

4. pwd - Print Working Directory muestra el directorio actual, para windows cd solo te muestra la ubicación:
![PWD Image](https://generalassembly.github.io/prework/cl/Graphics/terminal_ls.gif)

5. mkdir - Create a Folder crea una carpeta el directorio actual:
![mkdir Image](https://generalassembly.github.io/prework/cl/Graphics/terminal_rm_r.gif)