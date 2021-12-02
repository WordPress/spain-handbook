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

**Para editar:**

Una vez creado nuestro *fork* podemos proceder a editar el archivo, para ello pulsaremos el icono en forma de lápiz.

![editar-archivo](https://github.com/AlexMusetti/spain-handbook/blob/c932e5905c888d32679236e58023be6e68fb04ff/manual-github/assets/editar-archivo.png)

**Para validar los cambios de edición:**

Al terminar la edición, para guardar los cambios, debemos ir al final de la página, rellenar los campos correspondientes a *commit changes* y pulsar *Commit changes*.
Si queremos añadir los cambios en nuestro *fork*, dejaremos seleccionada la opción "*Commit directly to the master branch.*". De lo contrario estaríamos creando una nueva rama a partir de nuestro *fork*.

![commit-changes](https://github.com/AlexMusetti/spain-handbook/blob/32d9431ffc9bcc68a89f6a2fd8e999fbf944b702/manual-github/assets/commit-changes.png)

**Si nuestro *fork* deja de estar actualizado:**

Cuando se trabaja en un *fork*, se trabaja paralelamente al archivo máster. Es decir, los cambios producidos en el archivo principal (máster) no se sincronizan automáticamente con nuestro *fork*.

GitHub nos lo indicará con la siguiente frase:
“This branch is 8 commits behind WPES:master.”
Significa que se han realizado 8 modificaciones desde que hicimos nuestra copia (*fork*).

A continuación un ejemplo del aviso:

![branch-outdated](https://github.com/AlexMusetti/spain-handbook/blob/afa1336b95b12fab6848cedb8d76146e2de423a9/manual-github/assets/branch-outdated.png)

En este caso, si el archivo principal se ha adelantado a nuestra versión, tenemos dos opciones: *Contribute* o *Fetch upstream*

Si ya hemos editado nuestro archivo, pulsaremos *Contribute*, aparecerá una pequeña ventana que indica que el archivo no está actualizado y nos invita a hacer un *Pull request* para fusionar nuestra edición con el archivo principal (máster).

![contribute](https://github.com/AlexMusetti/spain-handbook/blob/afa1336b95b12fab6848cedb8d76146e2de423a9/manual-github/assets/contribute.png)

Si no hemos realizado aun cambios en nuestro fork, para trabajar en la versión aceptada más actualizada del archivo principal (máster), podemos pulsar en *Fetch Upstream*, que nos dará a su vez dos opciones más: *Compare* o *Fetch and merge*

![fetch-upstream](https://github.com/AlexMusetti/spain-handbook/blob/afa1336b95b12fab6848cedb8d76146e2de423a9/manual-github/assets/fetch-upstream.png)

*Compare* nos permite comparar las distintas versiones que se han creado y *Fetch and merge* sincronizará nuestro *fork* con el archivo principal (máster). 

En cualquier caso, si hubiera algún conflicto entre ambas versiones, el sistema nos avisará y nos invitará a hacer antes un *Pull request*.

A continuación una imagen de lo que nos mostraría la opción *compare*:

![Comparing-changes](https://github.com/AlexMusetti/spain-handbook/blob/afa1336b95b12fab6848cedb8d76146e2de423a9/manual-github/assets/Comparing-changes.png)

**Pull request:**

Cuando terminamos de editar nuestro archivo podemos proceder a realizar un *pull request*, nuestro archivo se enviará al administrador para su revisión y, una vez realizadas las comprobaciones pertinentes, nuestro *fork* se fusionará con el archivo principal.

Para hacer *pull request* a partir de nuestro *fork*:

1. Ir al repositorio principal y una vez allí, pulsar en *Pull requests*
![pull-request-1](https://github.com/AlexMusetti/spain-handbook/blob/679a74e857e45abac3de1855ef13291e299c1cbc/manual-github/assets/pull-request-1.png)
2. En pantalla aparecerá un listado con los *pull requests* existentes en ese momento (si los hay), para crear el nuestro pulsaremos en *New pull request*
![pull-request-2](https://github.com/AlexMusetti/spain-handbook/blob/679a74e857e45abac3de1855ef13291e299c1cbc/manual-github/assets/pull-request-2.png)
3. En este paso tenemos la oportunidad de comparar el archivo principal con nuestra propuesta, como en nuestro caso lo estamos haciendo desde un fork, pulsaremos *compare accross forks*, puesto que necesitamos indicar qué dos archivos vamos a comparar.
![pull-request-3](https://github.com/AlexMusetti/spain-handbook/blob/679a74e857e45abac3de1855ef13291e299c1cbc/manual-github/assets/pull-request-3.png)
4. Nos aparecerá un nuevo encabezado en el que podremos seleccionar nuestro fork pulsando en el desplegable *head repository*
![pull-request-4](https://github.com/AlexMusetti/spain-handbook/blob/679a74e857e45abac3de1855ef13291e299c1cbc/manual-github/assets/pull-request-4.png)
5. Si no hay ningún conflicto entre ambas versiones, el sistema nos indicará *Able to merge*, lo que significa que ya podemos pulsar la opción *Create pull request*
![pull-request-5](https://github.com/AlexMusetti/spain-handbook/blob/679a74e857e45abac3de1855ef13291e299c1cbc/manual-github/assets/pull-request-5.png).
6. En la siguiente pantalla aparecerá una ventana con los campos *Title* para poner un título a nuestra propuesta y *Write* para añadir los comentarios necesarios. Es imprescindible rellenar el campo *Title* para que se habilite la opción *Create pull request*, de lo contrario, la selección permanecerá deshabilitada.
![pull-request-6](https://github.com/AlexMusetti/spain-handbook/blob/2198d3ee5d93c4bd7a77ffea5ac04f506afb738a/manual-github/assets/pull-request-6.png)
7. Cuando terminamos de rellenar los campos, pulsamos sobre *create pull request* y se abre un desplegable con dos opciones como vemos en la siguiente imagen. Dejaremos seleccionada la primera opción si nuestro archivo ya está listo para revisión.
![pull-request-7](https://github.com/AlexMusetti/spain-handbook/blob/15876801347ec678982a08cf3d4fbb93500156ea/manual-github/assets/pull-request-7.png)


## Pasos a seguir (esquema WCES)

Como editor:

Paso 1: Hacer Fork

Paso 2: 
- Hacer modificación (editar archivo)
- Comentar la modificación
- Enviar la propuesta de cambio

Paso 3: Pull request


Como moderador:

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

