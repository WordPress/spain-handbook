

## Trabajar con el núcleo de WordPress

### Introducción para trabajar con el núcleo de WordPress

Si completó el módulo Cómo funcionan las traducciones en este curso, ahora tiene una comprensión general de cómo el proyecto de WordPress maneja la traducción y la localización. Esto incluye cosas como qué proyectos se traducen, la prioridad de la traducción y cómo se estructuran los equipos de traducción.

En esta lección, exploraremos más sobre cómo utilizar las traducciones, los componentes técnicos de la traducción de WordPress y cómo se relacionan con sus responsabilidades como administrador local o editor de traducción.

### Internacionalización de WordPress

Los desarrolladores de WordPress optaron por utilizar el marco de localización Gettext de GNU para proporcionar infraestructura de localización a WordPress. Gettext en un marco maduro y ampliamente utilizado para la traducción modular de software y, es el estándar para la localización en el ámbito del código abierto/software libre.

Gettext utiliza la traducción a nivel de mensaje. Cada “mensaje” que se muestra a los usuarios se traduce individualmente, ya sea un párrafo o una sola palabra. En WordPress, dichos “mensajes” son generados, traducidos y utilizados por los archivos PHP de WordPress a través de dos funciones PHP.

1. `_()` se usa cuando el mensaje se pasa como argumento a otra función.
2. `_e()` se usa para escribir el mensaje directamente en la página.

#### _(‘mensaje’)

Busca en el módulo de localización la traducción de ‘mensaje’ y pasa la traducción a la declaración de retorno de PHP. Si no encuentra ninguna traducción para ‘mensaje’, simplemente devuelve ‘mensaje’.

#### -e(‘mensaje’)

Busca en el módulo de localización la traducción de ‘mensaje’ y pasa la traducción a la declaración de eco de PHP. Si no encuentra ninguna traducción para ‘mensaje’, simplemente se hace eco de ‘mensaje’.

··· IMAGEN ··· Un ejemplo de la página Configuración > General. _(‘Para más información:’) es una cadena disponible para traducir.

Hay tres tipos de archivos utilizados en el marco de traducción Gettext. Estos archivos son utilizados y/o generados por herramientas de traducción durante el proceso de traducción, de la siguiente manera:

##### Archivos POT (Portable Object Template)

El primer paso en el proceso de localización es que se utiliza un programa para buscar a través del código fuente de WordPress y seleccionar cada mensaje pasado a una función `_()` o `_e()`.

Esta lista de mensajes en inglés se coloca en un archivo de plantilla con formato especial POT para WordPress, por lo que debería de generar uno propio. También se pueden crear archivos POT separados para temas y complementos, si el desarrollador del tema/complemento ha encerrado todo el texto en las funciones `_()` o `_e()`.

##### Archivos PO (Portable Object)

El segundo paso en el proceso de localización es que el traductor traduce todos los mensajes del archivo POT al idioma de destino y guarda los mensajes en inglés y traducidos en un archivo PO.

##### Archivos MO (Machine Object)

El paso final en el proceso de localización es que el archivo PO se ejecute a través de un programa que lo convierte en un archivo binario legible para una maquina optimizado (Archivo MO).

La compilación de las traducciones de código de máquina hace que el programa localizado sea mucho más rápido para recuperar las traducciones mientras se está ejecutando.

##### Archivos JSON

A partir de WordPress 5.0, los componentes de JavaScript se traducen mediante archivos JSON. Dentro del código JavaScript existen funciones de traducción similares a las del código PHP.

Estas cadenas se extraen automáticamente y están disponibles para su traducción en el sitio web: translate.wordpress.org, cuando se crea un `paquete de idioma o un paquete de instalación localizado, las traducciones de las funciones de JavaScript se incluyen como archivos JSON.

### Casos especiales y otros proyectos

#### Traducción directa

Si bien Gettext de GNU funciona bien para la mayoría de los aspectos de WordPress, hay algunos componentes del software que no se prestan a la localización con Gettext o que no deben traducirse. Esos incluyen:

1. `readme.html`: este es un archivo HTML estático, no un archivo PHP y, como tal, no se puede ejecutar a través de Gettext.
2. `licencia.txt`: por razones legales, debe mantenerse en inglés. Sin embargo, puede agregar una versión traducida al archivo.
3. `wp-config-sample.php`

··· IMAGEN ··· Ejemplo de un archivo wp-config-sample.php traducido

#### Parámetros de localización

Los proyectos de traducción para cada lugar contienen algunos parámetros que nunca deben “traducirse”, sino ajustarse a las especificaciones del idioma de destino.

Los más importantes como “prioridad alta” y se encuentran en la traducción del núcleo principal y en la parte “administrativa” y se pueden encontrar ordenando las cadenas de traducción en orden de prioridad descendente.

Puede ver una lista completa de estos parámetros, así como también cómo localizarlos, en la página del manual de políglotas: 

[Localization parameters](https://make.wordpress.org/polyglots/handbook/for-editors/working-with-core/#localization-parameters)

#### Complementos, temas y otros proyectos

Como se mencionó en la lección “lo que traducimos” de este curso, muchas regiones contribuyen con traducciones más allá del software principal de WordPress. Para complementos, yemas y otros proyectos en translate.wordpress.org, los paquetes de idioma se publicarán automáticamente cuando el proyecto esté traducido al menos en un 90%.

··· IMAGEN ··· Ejemplo de un complemento que no ha alcanzado el umbral de lanzamiento.

Cuando se lanza una nueva versión del complemento/tema con cadenas añadidas o actualizadas, las traducciones recién aprobadas del proyecto siempre desencadenarán la creación de un nuevo paquete de idioma.

Las traducciones del archivo léame del complemento se actualizan cadena por cadena después de que se aprueben sin umbrales específicos. Las traducciones para los “meta proyectos” https://translate.wordpress.org/projects/meta/ se implementan en varios intervalos.

### Lanzamiento de paquetes de WordPress

Un paquete de lanzamiento es un archivo ZIP que consta de WordPress en su totalidad, junto con archivos de traducción para el núcleo, los temas predeterminados y akismet o cualquier cambio personalizado que pueda tener.

Una vez que se contempla la traducción de un software principal de WordPress, es hora de generar un paquete. La mayoría de las configuraciones regionales utilizan lanzamientos automáticos, lo que significa que el paquete se lanzará una vez que se alcance el umbral de traducción. Si bien no es el método recomendado, los administradores de la configuración regional pueden crear paquetes de lanzamiento manualmente, si su configuración regional no utiliza versiones automáticas.

#### Liberación automatizada

Se recomienda que las configuraciones regionales y los administradores de configuradores regionales se aseguren de que su configuración regional sea elegible para paquetes de lanzamiento automatizados. Esto se debe a que ya no se recomienda el proceso de liberación manual del paquete y está sujeto a eliminación.

Si nunca ha tenido cambios personalizados y i18n.svn.wordpress.org está completamente vacío para su configuración regional, no necesita hacer nada. Su paquete de lanzamiento se creará automáticamente para usted.

Si tiene cambios personalizados menores para la versión estable actual (como 5.8), que consisten, como máximo, en los siguientes archivos:
1. un archivo Léame traducido
2. archivo de licencia
3. wp-config-sample.php

Asegúrese de que estos archivos existan en un directorio Branch/5.8/dist en i18n.snv.wordpress.org. Si es así, su paquete de lanzamiento se creará automáticamente para usted.

##### ¿Cuándo se lanza un nuevo paquete?

Se creará una nueva compilación solo si se cambió una traducción después de la última compilación. Eso significa que rechazar y aprobar una traducción dentro del proyecto de WordPress en translate-wordpress.org activará una nueva compilación. Los paquetes de lanzamiento y los paquetes de idioma para versiones estables generalmente se crean cada hora en punto.

##### ¿Cuáles son los umbrales de traducción necesarios para un lanzamiento automatizado?

Los paquetes de lanzamiento y los paquetes de idioma para las versiones estables generalmente se crean cada hora después de que el subproyecto “desarrollo” tenga al menos el 90% y el subproyecto “administración” tenga al menos el 75%.

··· IMAGEN ···

#### Liberación manual

Tenga en cuenta: no se recomienda la publicación manual de paquetes y, se recomienda a los locales que se aseguren de que son elegibles para los lanzamientos automáticos, esto es lo que necesita saber.

Primero, debe obtener el número de revisión del paquete de WordPress correspondiente. Los lanzamientos están disponibles en la lista de etiquetas en core trac o en esta página en la sección “revisiones de lanzamiento”. Esta lista no incluye prelanzamientos, incluidas versiones beta y candidatos de lanzamiento. Para esos, deberá buscar una referencia a la versión. “bump” en el registro de revisión de build.trac.wordpress.org.

Una vez que tenga el número de revisión de la versión que empaquetará, es hora de crear el paquete real. Para ello, sigue estos pasos:

1. Inicie sesión como editor de traducción general en su sitio local de WordPress (locale.wordpress.org)
2. Vaya a Herramientas¬Paquetes de lanzamiento
3. Desplácese hacia abajo hasta la sección Crear nuevo paquete
4. En ¿de dónde deberíamos obtener sus traducciones?, seleccione translate.wordpress.org si desea utilizar esas traducciones actuales. Si ha registrado archivos de mensajes traducidos en snv, seleccione subversión.
5. Para la rama Locale para archivos dist, seleccione la ubicación de sus archivos traducidos en:  https://i18n.svn.wordpress.org/locale/
6. Para rama de WordPress, seleccione la rama original correspondiente.
7. Para la revisión de WordPress seleccione el número de revisión que encontró al principio.
8. La versión WordPress se utilizará como nombre del paquete (p. ej. 3.9-beta3, 3.9-RC1).
9. Haga clic en el botón crear paquete.

Antes de lanzar el paquete al público, descargue el archivo ZIP o tar.gz de los enlaces en la parte superior de la página y pruébelo.

Cuando esté listo para lanzar la versión final al público, haga clic en el enlace Lanzamiento de la versión debajo de la columna de acción. ¡Esto marca el lanzamiento oficial de la versión!

A los usuarios se les pedirá que actualicen su paquete de idioma en su tablero y se actualizará la información de descarga en su sitio local.
