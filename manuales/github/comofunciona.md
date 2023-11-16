# Cómo funciona GitHub

GitHub puede parecer, a priori, un poco intimidante, pero nada más lejos si se se siguen unos pasos concretos.

Lo más importante es que te hayas creado una cuenta en GitHub. Si todavía no lo has hecho, puedes [ir al apartado del manual en el que se explica cómo crear una cuenta en GitHub](https://es.wordpress.org/team/handbook/manuales/github/crear/).

Si ya tienes una cuenta, puedes continuar en este camino.

## Qué es un repositorio

Llamamos repositorio a un lugar, que se podría comparar con una unidad de disco duro o una carpeta principal de un servidor, en definitiva, un lugar de almacenamiento de archivos.

En este repositorio se pueden almacenar todo tipo de archivos, desde carpetas y ficheros sin un orden concreto, un programa completo o un manual como el que estás leyendo ahora mismo, que fue escrito en GitHub antes de ser publicado en la web.

## Acceder al repositorio de WordPress España

Para acceder al repositorio de WordPress, no tienes más que acceder a través de la siguiente dirección:

[https://github.com/WPES/spain-handbook/](https://github.com/WPES/spain-handbook)

En este repositorio están alojados todos los archivos que conforman todo el manual de WordPress en español.

Aquí es donde vas a hacer todos los cambios que, una vez aceptados, se reflejarán en la esta web que estás leyendo.

Una vez registrados podemos acceder a la página principal de [GitHub](https://github.com/) y en la barra lateral aparecerá el listado de repositorios a los que tenemos acceso.

Pinchamos en [WPES/spain-handbook](https://github.com/WPES/spain-handbook) para acceder al repositorio de manuales de WordPress España. En la parte superior izquierda podremos ver en todo momento en qué repositorio estamos.

Con el fin de evitar posibles errores o conflictos **es importante no trabajar nunca directamente en este repositorio principal**. Para poder editar con seguridad, crearemos una copia del repositorio principal (*fork*) que será donde trabajaremos.

## Crear un fork

Crearemos el *fork* pinchando en el último botón que aparece en la parte superior derecha, está rodeado en azul para que puedas localizarlo más fácilmente.

![Realización Fork](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/ForkCuentaPrincipal.png)

Después de realizarlo, la ventana cambiará y si nos fijamos en la ruta que se muestra en la parte de arriba a la izquierda ya aparecerá nuestro nombre de usuario, desde este momento cualquier cambio que hagamos en este repositorio, no afectará al repositorio original hasta que no hagamos un *Pull request* y éste no sea verificado y aprobado.

![Fork realizado](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/ForkRealizado.PNG)

## Seleccionar un Issue

## Crear una rama

## Editar un contenido

## Enviar un contenido

## Crear un Pull Request

Cuando terminamos de editar nuestro archivo podemos proceder a realizar un *pull request*, nuestro archivo se enviará al administrador para su revisión y, una vez realizadas las comprobaciones pertinentes, nuestro *fork* se fusionará con el archivo principal.

Para hacer *pull request* a partir de nuestro *fork*:

1. Ir al repositorio principal y una vez allí, pulsar en *Pull requests*.

![pull-request-1](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/pull-request-1.png)

2. En pantalla aparecerá un listado con los *pull requests* existentes en ese momento (si los hay), para crear el nuestro pulsaremos en *New pull request*.

![pull-request-2](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/pull-request-2.png)

3. En este paso tenemos la oportunidad de comparar el archivo principal con nuestra propuesta, como en nuestro caso lo estamos haciendo desde un *fork*, pulsaremos *compare accross forks*, puesto que necesitamos indicar qué dos archivos vamos a comparar.

![pull-request-3](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/pull-request-3.png)

4. Nos aparecerá un nuevo encabezado en el que podremos seleccionar nuestro *fork* pulsando en el desplegable *head repository*.

![pull-request-4](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/pull-request-4.png)

5. Si no hay ningún conflicto entre ambas versiones, el sistema nos indicará *Able to merge*, lo que significa que ya podemos pulsar la opción *Create pull request*.

![pull-request-5](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/pull-request-5.png)

6. En la siguiente pantalla aparecerá una ventana con los campos *Title* para poner un título a nuestra propuesta y *Write* para añadir los comentarios necesarios.

Es imprescindible rellenar el campo *Title* para que se habilite la opción *Create pull request*, de lo contrario, la selección permanecerá deshabilitada.

![pull-request-6](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/pull-request-6.png)

7. Cuando terminamos de rellenar los campos, pulsamos sobre *create pull request* y se abre un desplegable con dos opciones como vemos en la siguiente imagen.

Dejaremos seleccionada la primera opción si nuestro archivo ya está listo para revisión.

![pull-request-7](https://raw.githubusercontent.com/WPES/spain-handbook/master/manuales/github/assets/pull-request-7.png)

