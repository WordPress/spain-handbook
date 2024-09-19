# Editar un documento/archivo

Una vez creado nuestro *fork* y creada la rama sobre la que vamos a trabajar, seleccionaremos el archivo que vamos a editar y, a continuación seleccionaremos el lápiz que hay sobre el marco del contenido.

![editar archivo](https://raw.githubusercontent.com/WordPress/spain-handbook/main/assets/editardocumento-abrir-sesion-edicion.webp)

De esta forma abriremos la sesión de edición y podremos escribir.

En GitHub se escribe en formato **Markdown**. Se trata de un lenguaje de marcado de texto plano muy sencillo que puedes aplicar en cualquier aplicación de mensajería como Telegram o Whatsapp, y que te permite aplicar formato a un texto.

Para que no tengas problema ninguno, hemos creado este [manual de Markdown](https://es.wordpress.org/team/handbook/manuales/markdown/) con absolutamente todo lo que necesitas para colaborar en el manual de WordPress en Español.

## Aspectos a tener en cuenta a la hora de editar el manual de WordPress en Español

Hay algunas cosas que debes tener en cuenta cuando estás editando en el manual de WordPress en Español, para facilitar el trabajo de moderación del equipo de documentación.

### Encabezados

La jerarquía de encabezados es como la de cualquier página web, solamente puede haber un H1, que corresponde con el título de la página, y que introducirás con (#).

A partir de ahí, todos los encabezados que se añadan a continuación serán de jerarquías inferiores (H2, H3, etc), intentando no dar más de dos niveles de profundidad al texto.

### Imágenes

Cuando insertamos las imágenes en nuestro _fork_, las alojaremos en la carpeta **assets**.

Deberemos intentar que las imágenes estén en formato WebP, y el nombre no contendrá espacios ni símbolos extraños, tan solo caracteres alfanuméricos (letras y números, sin tildes) y guiones medios (-) para separar palabras.

La ruta de la imagen que insertemos puede que lleve la ruta de nuestro repositorio, pero debemos sustituirla por la ruta del repositorio principal del manual, que es la siguiente:

`https://raw.githubusercontent.com/WordPress/spain-handbook/master/assets/`

De este modo, el nombre de una imagen llamada `captura-de-ventana-de-login.webp` quedaría así, incluyendo el texto alternativo para la accesibilidad:

`![Vista de la ventana de login](https://raw.githubusercontent.com/WordPress/spain-handbook/master/assets/captura-de-ventana-de-login.webp)`

Estas imágenes conviene que las redimensiones y optimices para que no sean enormes y ralenticen la carga de la web. Para ello, tienes sobre [cómo editar las imágenes](https://es.wordpress.org/team/handbook/manuales/github/editarimagen/) de una forma muy sencilla.

## Una vez que he terminado de editar

Una vez que hayas terminado de editar, como en cualquier otro programa de edición, deberás guardar los cambios. Esto en GitHub es [**hacer un _commit_**](https://es.wordpress.org/team/handbook/manuales/github/commit/), que es lo siguiente que vamos a ver.