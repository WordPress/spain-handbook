# Guía de uso de Github para la colaboración en la Comunidad WordPress de España

## Pasos a seguir para colaborar en el manual a través de Github

### ¿En qué procesador de textos lo escribimos?
En realidad, vamos a usar un editor de texto plano con formato **Markdown**. Se trata de un formato de texto que podemos editar con cualquier editor de código como Visual Studio Code, Sublime Text o Atom o en la misma web de GitHub (recomendado), en el que el formato se introduce con una serie de comandos que veremos a continuación.

## Crear una cuenta en Github
Para crearte una cuenta en Github, debes ir a su página principal [github.com](https://github.com/) y crearte una cuenta.

Una vez que hemos creado nuestra cuenta, buscaremos el repositorio donde se encuentra el manual dentro de Github, que se encuentra en [WPGranada/HandBook](https://github.com/WPES/spain-handbook).

[Cómo colaborar en un proyecto en Github](https://gist.github.com/BCasal/026e4c7f5c71418485c1) **(esto queda provisional)**

## Hacer una copia del repositorio en nuestra cuenta de github (fork)


## Edición del archivo



## Pasos a seguir (esquema WCES)

**Como editor**:

Paso 1: Hacer Fork

Paso 2: 
- Hacer modificación (editar archivo)
- Comentar la modificación
- Enviar la propuesta de cambio

Paso 3: Pull request

Paso 4: Fetch Upstream

Una vez creado el *fork*, trabajamos paralelamente al archivo máster. Es decir, los cambios producidos en el archivo principal (máster) no se sincronizan automáticamente con nuestro *fork*.

GitHub nos lo indicará con la siguiente frase:
“This branch is 8 commits behind WPES:master.”
Significa que se han realizado 8 modificaciones desde que hicimos nuestra copia (*fork*).

A continuación un ejemplo del aviso:

![branch-outdated](https://github.com/AlexMusetti/spain-handbook/blob/master/manual-github/assets/branch-outdated.png)

Tenemos dos opciones: *Contribute* o *Fetch upstream*

Si decidimos editar en ese momento y pulsamos *Contribute*, nos aparece una pequeña ventana que indica que el archivo no está actualizado y nos invita a hacer un *Pull request* para fusionar nuestra edición con el archivo principal (máster).

![contribute](https://github.com/AlexMusetti/spain-handbook/blob/master/manual-github/assets/contribute.png)

Para volver a trabajar en la versión aceptada más actualizada del archivo principal (máster), podemos pulsar en *Fetch Upstream*, que nos dará a su vez dos opciones más: *Compare* o *Fetch and merge*

![fetch-upstream](https://github.com/AlexMusetti/spain-handbook/blob/master/manual-github/assets/fetch-upstream.png)

*Compare* nos permite comparar las distintas versiones que se han creado y *Fetch and merge* sincronizará nuestro *fork* con el archivo principal (máster). Si hubiera algún conflicto entre ambas versiones, el sistema nos avisará y nos invitará a hacer antes un *Pull request*.

A continuación una imagen de lo que nos mostraría la opción *compare*:

![Comparing-changes](https://github.com/AlexMusetti/spain-handbook/blob/master/manual-github/assets/Comparing-changes.png)

**Como moderador**:

Paso 1: Revisar los pull request

Paso 2: Aprobación o modificación de los pull request.


Como editor cuando volvemos a editar:
Paso 1: Hacer "Fetch upstream" y dar a "fetch and merge" si queremos unir o "compare" si no tenemos claro.

![Captura de los proyectos en Github](https://github.com/WPES/spain-handbook/blob/master/manual-github/assets/Pasted-image-20211125184751.png "pie de foto")






## Cómo funciona Markdown

Es muy fácil, consulta el siguiente manual y, en apenas 10 minutos lo tendrás listo.

[Manual de Markdown](https://commonmark.org/help/)

[Generador de tablas en Markdown](https://www.tablesgenerator.com/markdown_tables)

[Cómo colaborar en un proyecto en Github](https://gist.github.com/BCasal/026e4c7f5c71418485c1)

Es muy importante que, antes de hacer absolutamente nada, creemos una rama. La nombraremos con nuestro nombre de usuario en WordPress.org y un pequeño texto descriptivo. separado por guiones.

Una vez que terminemos de hacer los cambios, haremos un commit y posteriormente un pull request.

