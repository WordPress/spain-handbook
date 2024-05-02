# Entorno del servidor

Aunque WordPress puede funcionar en casi cualquier entorno, incluso en los más mínimos, hay que reconocer que no funciona completamente bien en estos. Por eso, aquí vamos a hacer algunas recomendaciones mínimas sobre el entorno en el que funcionaría más eficazmente, teniendo en cuenta que la mayoría de los sitios web de WordPress utilizan plugins y temas de terceros que comúnmente introducen requisitos adicionales a nivel de servidor.

## Servidor Web

El servidor web es un software que acepta solicitudes web de los usuarios y les proporciona el resultado adecuado. Hay muchos servidores web diferentes que funcionan en diferentes sistemas operativos. Generalmente, si tu servidor web admite y ejecuta archivos PHP, debería ser capaz de trabajar con WordPress.

Los dos más populares que se recomiendan son:

- [Apache HTTPD](https://httpd.apache.org/) 2.4
- [nginx](https://nginx.org/) 1.24

Otros son utilizados por empresas de alojamiento y desarrolladores y también son conocidos por funcionar bien:

- [Angie](https://angie.software/en/) 1.5
- [LiteSpeed Web Server](https://www.litespeedtech.com/products/litespeed-web-server) 6.2 / 6.1 / 6.0 / 5.4
- [OpenLiteSpeed](https://openlitespeed.org/) 1.8 / 1.7

_Esas son las versiones más recientes en el momento de escribir este documento. ¡Mantén siempre tu servidor web actualizado para asegurar el mejor rendimiento!_

## PHP

PHP es un lenguaje de programación en el que se basa el código de WordPress. Este lenguaje se ejecuta en el servidor y es importante mantenerlo actualizado, tanto por seguridad como por funcionalidad.

WordPress es compatible con muchas versiones de PHP, algunas incluso obsoletas ([Compatibilidad de PHP y versiones de WordPress](https://make.wordpress.org/core/handbook/references/php-compatibility-and-wordpress-versions/)). Para las empresas de alojamiento, recomendamos:

**WordPress 6.5**

- [PHP 8.1](https://www.php.net/ChangeLog-8.php#PHP_8_1)
- [PHP 8.2](https://www.php.net/ChangeLog-8.php#PHP_8_2)
- [PHP 8.3](https://www.php.net/ChangeLog-8.php#PHP_8_3)

_IMPORTANTE: WordPress 6.4 es **compatible con excepciones** con PHP 8.0, PHP 8.1 y PHP 8.2, y **compatible en beta** con PHP 8.3._

_¿Qué significa "compatible con excepciones"?_

- PHP 8.0
	- [Parámetros nombrados](https://core.trac.wordpress.org/ticket/59649). WordPress no admite parámetros nombrados.
	- [Sistema de archivos WP_Filesystem_FTPext y WP_Filesystem_SSH2 cuando la conexión falla](https://core.trac.wordpress.org/ticket/48689).

- PHP 8.1
	- No se han encontrado todos los problemas de "pasar null a parámetros no nulos".
	- [htmlentities() y funciones relacionadas necesitan que se establezca explícitamente el valor predeterminado del parámetro de flags](https://core.trac.wordpress.org/ticket/53465).
	- [Reemplazar la mayoría de los strip_tags() por wp_strip_tags()](https://core.trac.wordpress.org/ticket/57579).

- PHP 8.2
	- [Depreciación de utf8_{encode|decode}](https://core.trac.wordpress.org/ticket/55603) con una decisión pendiente sobre la necesidad de una extensión de PHP.
	- [Propiedades dinámicas desconocidas](https://core.trac.wordpress.org/ticket/56034) en desuso.

_¿Qué significa "beta"?_

- PHP 8.3
	- Notificaciones de depreciación: Una notificación de depreciación no es un error, sino más bien un indicador de dónde se necesita trabajo adicional para la compatibilidad antes de PHP 9.0. Con una notificación de depreciación, el código PHP seguirá funcionando y nada está roto.

**WordPress 6.4**

- [PHP 8.1](https://www.php.net/ChangeLog-8.php#PHP_8_1)
- [PHP 8.2](https://www.php.net/ChangeLog-8.php#PHP_8_2)

_IMPORTANTE: WordPress 6.4 es **compatible con excepciones** con PHP 8.0, PHP 8.1 y PHP 8.2, y **compatible en beta** con PHP 8.3._

_¿Qué significa "compatible con excepciones"?_

- PHP 8.0
	- [Parámetros nombrados](https://core.trac.wordpress.org/ticket/59649). WordPress no admite parámetros nombrados.
	- [Sistema de archivos WP_Filesystem_FTPext y WP_Filesystem_SSH2 cuando falla la conexión](https://core.trac.wordpress.org/ticket/48689).

- PHP 8.1
	- No se han encontrado todas las incidencias de "pasar null a parámetros no nulos".
	- [htmlentities() y funciones relacionadas necesitan que el valor predeterminado del parámetro de flags se establezca explícitamente](https://core.trac.wordpress.org/ticket/53465).
	- [Reemplazar la mayoría de strip_tags() por wp_strip_tags()](https://core.trac.wordpress.org/ticket/57579).

- PHP 8.2
	- [Depreciación de utf8_{encode|decode}](https://core.trac.wordpress.org/ticket/55603) con una decisión pendiente sobre la necesidad de una extensión de PHP.
	- [Propiedades dinámicas desconocidas](https://core.trac.wordpress.org/ticket/56034) en desuso.

_¿Qué significa "beta"?_

- PHP 8.3
	- Avisos de depreciación: Un aviso de depreciación no es un error, sino un indicador de dónde se necesita trabajo adicional para la compatibilidad antes de PHP 9.0. Con un aviso de depreciación, el código PHP seguirá funcionando y nada está roto.

**WordPress 6.3**

- [PHP 8.1](https://www.php.net/ChangeLog-8.php#PHP_8_1)
- [PHP 8.2](https://www.php.net/ChangeLog-8.php#PHP_8_2)

_IMPORTANTE: WordPress 6.3 es **compatible con excepciones** con PHP 8.0 y PHP 8.1, y **compatible en beta** con PHP 8.2._

_¿Qué significa "compatible con excepciones"?_

- PHP 8.0
	- Parámetros nombrados. WordPress no admite parámetros nombrados.
	- [Sistema de archivos WP_Filesystem_FTPext y WP_Filesystem_SSH2 cuando falla la conexión](https://core.trac.wordpress.org/ticket/48689).

- PHP 8.1
	- [htmlentities() y funciones relacionadas necesitan que el valor predeterminado del parámetro de flags se establezca explícitamente](https://core.trac.wordpress.org/ticket/53465).
	- [Reemplazar la mayoría de strip_tags() por wp_strip_tags()](https://core.trac.wordpress.org/ticket/57579).
	- [unregister_setting() para una configuración desconocida](https://core.trac.wordpress.org/ticket/57674).

_¿Qué significa "beta"?_

- PHP 8.2
	- Avisos de depreciación: Un aviso de depreciación no es un error, sino un indicador de dónde se necesita trabajo adicional para la compatibilidad antes de PHP 9.0. Con un aviso de depreciación, el código PHP seguirá funcionando y nada está roto.

**WordPress 6.2**

- [PHP 7.4](https://www.php.net/ChangeLog-7.php#PHP_7_4)
- [PHP 8.0](https://www.php.net/ChangeLog-8.php#PHP_8_0)
- [PHP 8.1](https://www.php.net/ChangeLog-8.php#PHP_8_1)
- [PHP 8.2](https://www.php.net/ChangeLog-8.php#PHP_8_2)

_IMPORTANTE: WordPress 6.2 es **compatible en beta** con [PHP 8.0](https://make.wordpress.org/core/2020/11/23/wordpress-and-php-8-0/), [PHP 8.1](https://make.wordpress.org/core/2022/01/10/wordpress-5-9-and-php-8-0-8-1/) y PHP 8.2. El uso de algunas de estas versiones puede generar advertencias._

**WordPress 6.1**

- [PHP 7.4](https://www.php.net/ChangeLog-7.php#PHP_7_4)
- [PHP 8.0](https://www.php.net/ChangeLog-8.php#PHP_8_0)*
- [PHP 8.1](https://www.php.net/ChangeLog-8.php#PHP_8_1)*
- [PHP 8.2](https://www.php.net/ChangeLog-8.php#PHP_8_2)*

_IMPORTANTE: WordPress 6.1 es **compatible en beta** con [PHP 8.0](https://make.wordpress.org/core/2020/11/23/wordpress-and-php-8-0/), [PHP 8.1](https://make.wordpress.org/core/2022/01/10/wordpress-5-9-and-php-8-0-8-1/) y PHP 8.2. El uso de algunas de estas versiones puede generar advertencias._

### Acerca de PHP

PHP 8.1 solo recibe mantenimiento por parte de la Comunidad de PHP en forma de _correcciones de seguridad_ desde el 26-11-2022. Mantener tu versión de PHP actualizada a la última versión estable es importante para la velocidad y la seguridad de WordPress.

Las versiones anteriores a PHP 8.1 no son mantenidas por la Comunidad de PHP, aunque podrían recibir actualizaciones de seguridad por parte de las distribuciones de sistemas operativos.

Versiones de PHP al final de su vida útil:

- PHP 8.3: 23-11-2026
- PHP 8.2: 08-10-2025
- PHP 8.1: 25-11-2024
- PHP 8.0: 26-11-2023 _última versión: 8.0.30_
- PHP 7.4: 28-11-2022 _última versión: 7.4.33_
- PHP 7.3: 06-12-2021 _última versión: 7.3.33_
- PHP 7.2: 30-11-2020 _última versión: 7.2.34_
- PHP 7.1: 01-12-2019 _última versión: 7.1.33_
- PHP 7.0: 10-01-2019 _última versión: 7.0.33_
- PHP 5.6: 31-12-2018 _última versión: 5.6.40_
- PHP 5.5: 21-07-2016 _última versión: 5.5.38_
- PHP 5.4: 03-09-2015 _última versión: 5.4.45_
- PHP 5.3: 14-08-2014 _última versión: 5.3.29_
- PHP 5.2: 06-01-2011 _última versión: 5.2.17_
- PHP 5.1: 24-08-2006 _última versión: 5.1.6_
- PHP 5.0: 05-09-2005 _última versión: 5.0.5_
- PHP 4.4: 07-08-2008 _última versión: 4.4.9_
- PHP 4.3: 31-03-2005 _última versión: 4.3.11_
- PHP 4.2: 06-09-2002 _última versión: 4.2.3_
- PHP 4.1: 12-03-2002 _última versión: 4.1.2_
- PHP 4.0: 23-06-2001 _última versión: 4.0.6_

### Extensiones de PHP

El núcleo de WordPress hace uso de varias extensiones de PHP cuando están disponibles. Si falta la extensión preferida, WordPress tendrá que trabajar más para realizar la tarea que el módulo ayuda a realizar o, en el peor de los casos, eliminará la funcionalidad. Todas las extensiones son para instalaciones con PHP >= 7.4.

Las siguientes extensiones de PHP son _necesarias_ para que un sitio de WordPress funcione:

- [json](https://www.php.net/manual/es/book.json.php) (incluido en >=8.0.0) - Se utiliza para comunicaciones con otros servidores y procesamiento de datos en formato JSON.
- Una de las siguientes: [mysqli](https://www.php.net/manual/es/book.mysqli.php) (incluido en >=5.0.0), o [mysqlnd](https://www.php.net/manual/es/book.mysqlnd.php) - Conecta a MySQL para interacciones con la base de datos.

Las siguientes extensiones de PHP son _altamente recomendadas_ para permitir que WordPress opere de manera óptima y para maximizar la compatibilidad con muchos plugins y temas populares:

- [curl](https://www.php.net/manual/es/book.curl.php) (PHP >= 7.3 requiere libcurl >= 7.15.5; PHP >= 8.0 requiere libcurl >= 7.29.0) - Realiza operaciones de solicitud remota.
- [dom](https://www.php.net/manual/es/book.dom.php) (requiere libxml) - Se usa para validar el contenido del Widget de Texto y para configurar automáticamente IIS7+.
- [exif](https://www.php.net/manual/es/book.exif.php) (requiere php-mbstring) - Trabaja con metadatos almacenados en imágenes.
- [fileinfo](https://www.php.net/manual/es/book.fileinfo.php) (incluido en PHP) - Se utiliza para detectar el mimetype de las subidas de archivos.
- [hash](https://www.php.net/manual/es/book.hash.php) (incluido en PHP >=5.1.2) - Se utiliza para hashing, incluyendo contraseñas y paquetes de actualización.
- [igbinary](https://www.php.net/manual/es/book.igbinary.php) - Aumenta el rendimiento como un reemplazo del serializador estándar de PHP.
- [imagick](https://www.php.net/manual/es/book.imagick.php) (requiere ImageMagick >= 6.2.4) - Proporciona mejor calidad de imagen para las subidas de medios. Véase [WP\_Image\_Editor](https://developer.wordpress.org/reference/classes/wp_image_editor/) para más detalles. Redimensionamiento inteligente de imágenes (para imágenes más pequeñas) y soporte de miniaturas de PDF, cuando también está disponible Ghost Script.
- [intl](https://www.php.net/manual/es/book.intl.php) (PHP >= 7.4.0 requiere ICU >= 50.1) - Habilita para realizar operaciones conscientes de la localización incluyendo, pero no limitado a, formateo, transliteración, conversión de codificación, operaciones de calendario, colación conforme, localización de límites de texto y trabajo con identificadores de localización, zonas horarias y grafemas.
- [mbstring](https://www.php.net/manual/es/book.mbstring.php) - Se utiliza para manejar correctamente el texto en UTF8.
- [openssl](https://www.php.net/manual/es/book.openssl.php) (PHP 7.1-8.0 requiere OpenSSL >= 1.0.1 / < 3.0; PHP >= 8.1 requiere OpenSSL >= 1.0.2 / < 4.0) - Conexiones basadas en SSL con otros hosts.
- [pcre](https://www.php.net/manual/es/book.pcre.php) (incluido en PHP >= 7.0 recomendado PCRE 8.10) - Aumenta el rendimiento de las coincidencias de patrones en las búsquedas de código.
- [xml](https://www.php.net/manual/es/book.xml.php) (requiere libxml) - Se utiliza para el análisis de XML, como el de un sitio de terceros.
- [zip](https://www.php.net/manual/es/book.zip.php) (requiere libzip >= 0.11; recomendado libzip >= 1.6) - Se utiliza para descomprimir plugins, temas y paquetes de actualización de WordPress.

Las siguientes extensiones de PHP son _recomendadas_ para permitir algún tipo de caché en WordPress (si es necesario). APCu, Memcached y Redis son alternativas de las cuales solo se necesita usar una.

- [apcu](https://www.php.net/manual/es/book.apcu.php) – Almacén de clave-valor en memoria para PHP (APC sin caché de opcode).
- [memcached](https://www.php.net/manual/es/book.memcached.php) (requiere libmemcached >= 1.0.0) - memcached es un sistema de caché de objetos en memoria distribuido de alto rendimiento, de naturaleza genérica, pero diseñado para acelerar aplicaciones web dinámicas al aliviar la carga de la base de datos.
- [opcache](https://www.php.net/manual/es/book.opcache.php) - PHP puede configurarse para precargar scripts en el opcache cuando el motor arranca.
- [redis](https://pecl.php.net/package/redis) - Extensión de PHP para la interfaz con Redis.

Para completar, a continuación se lista el resto de los módulos de PHP que WordPress _puede_ utilizar en ciertas situaciones o si otros módulos no están disponibles. Estos son alternativas o opcionales y no necesariamente necesarios en un entorno óptimo, pero instalarlos no perjudicará.

- [bc](https://www.php.net/manual/es/book.bc.php) - Para matemáticas de precisión arbitraria, que soporta números de cualquier tamaño y precisión hasta 2147483647 dígitos decimales.
- [filter](https://www.php.net/manual/es/book.filter.php) - Se utiliza para filtrar de manera segura la entrada del usuario.
- [image](https://www.php.net/manual/es/book.image.php) (requiere libgd >= 2.1.0; requiere zlib >= 1.2.0.4; opcional freetype2) - Si Imagick no está instalado, la Biblioteca Gráfica GD se utiliza como una alternativa funcionalmente limitada para la manipulación de imágenes.
- [iconv](https://www.php.net/manual/es/book.iconv.php) (requiere libiconv/POSIX) - Se utiliza para convertir entre conjuntos de caracteres.
- [shmop](https://www.php.net/manual/es/book.shmop.php) - Shmop es un conjunto fácil de usar de funciones que permite a PHP leer, escribir, crear y eliminar segmentos de memoria compartida de Unix.
- [simplexml](https://www.php.net/manual/es/book.simplexml.php) (requiere libxml) - Se utiliza para el análisis de XML.
- [sodium](https://www.php.net/manual/es/book.sodium.php) - (incluido en PHP >=7.2.0; requiere libsodium >= 1.0.8) - Valida firmas y proporciona bytes aleatorios de manera segura.
- [xmlreader](https://www.php.net/manual/es/book.xmlreader.php) (requiere libxml) - Se utiliza para el análisis de XML.
- [zlib](https://www.php.net/manual/es/book.zlib.php) (requiere zlib >= 1.2.0.4) - Compresión y descompresión Gzip.

Estas extensiones se utilizan para cambios de archivos, como actualizaciones e instalación de plugins/temas, cuando los archivos no son escribibles en el servidor.

- [ssh2](https://www.php.net/manual/es/book.ssh2.php) (requiere OpenSSL y libssh >= 1.2; recomendado libssh >= 1.2.9) - Proporciona acceso a recursos (shell, ejecución remota, túneles, transferencia de archivos) en una máquina remota utilizando un transporte criptográfico seguro.
- [ftp](https://www.php.net/manual/es/book.ftp.php) - Implementa acceso de cliente a servidores de archivos que hablan el Protocolo de Transferencia de Archivos (FTP).
- [sockets](https://www.php.net/manual/es/book.sockets.php) - Implementa una interfaz de bajo nivel a las funciones de comunicación de sockets basadas en los populares sockets BSD.

La prioridad de los transportes son IO de archivos directo, SSH2, Extensión FTP de PHP, FTP implementado con Sockets y FTP implementado mediante PHP solo.

### Paquetes del Sistema

- [curl](https://curl.se/) (recomendado >= 8.4)
- [Ghost Script](https://www.ghostscript.com/) (recomendado Ghost Script >= 10.0) - Permite que Imagick/ImageMagick genere miniaturas de PDF para la biblioteca de medios. Vea [Soporte mejorado de PDF en WordPress 4.7](https://make.wordpress.org/core/2016/11/15/enhanced-pdf-support-4-7/) para más detalles.
- [ImageMagick](https://imagemagick.org/) (recomendado ImageMagick >= 7.1) - Necesario para la extensión Imagick.
- [OpenSSL](https://www.openssl.org/) (recomendado >= 3.0)

## Base de Datos

Para el almacenamiento de datos, WordPress utiliza sistemas compatibles con MySQL.

Oficialmente recomendados por WordPress son:

- [MySQL](https://dev.mysql.com/downloads/mysql/) 8.0 LTS
- [MariaDB](https://mariadb.org/) 10.11 LTS

Versiones de MySQL al final de su vida útil:

- MySQL 8.3: n/d
- MySQL 8.2: n/d
- MySQL 8.1: 25-10-2023
- MySQL 8.0: 30-04-2026
- MySQL 5.7: 31-10-2023
- MySQL 5.6: 28-02-2021
- MySQL 5.5: 31-12-2018

Versiones de MariaDB al final de su vida útil:

- MariaDB 11.3: 16-02-2025
- MariaDB 11.2: 21-11-2024
- MariaDB 11.1: 21-08-2024
- MariaDB 11.0: 07-06-2024
- MariaDB 10.11: 16-02-2028
- MariaDB 10.10: 17-11-2023
- MariaDB 10.9: 22-08-2023
- MariaDB 10.8: 20-05-2023
- MariaDB 10.7: 09-02-2023
- MariaDB 10.6: 06-07-2026
- MariaDB 10.5: 24-06-2025
- MariaDB 10.4: 18-06-2024
- MariaDB 10.3: 25-05-2023
- MariaDB 10.2: 22-05-2022
- MariaDB 10.1: 17-10-2020
- MariaDB 10.0: 31-03-2019
- MariaDB 5.5: 11-04-2020

Otros servidores MySQL conocidos por su buen rendimiento son:

- [Percona MySQL Server](https://www.percona.com/software/mysql-database) 8.0
- [Amazon Aurora](https://aws.amazon.com/rds/aurora/)
- [Amazon RDS para MariaDB](https://aws.amazon.com/rds/mariadb/) 10.11
- [Amazon RDS para MySQL](https://aws.amazon.com/rds/mysql/) 8.0
- [Azure Database para MySQL](https://azure.microsoft.com/products/mysql/)
- [Google Cloud MySQL](https://cloud.google.com/sql/mysql) 8.0
- [MySQL de DigitalOcean](https://www.digitalocean.com/products/managed-databases-mysql)
- [IBM Cloud Databases para MySQL](https://www.ibm.com/cloud/databases-for-mysql)
- [MySQL HeatWave](https://www.oracle.com/mysql/)

Aunque WordPress puede funcionar en versiones anteriores, se recomienda utilizar estas o versiones más recientes por razones de seguridad y rendimiento.

## ¿Cómo sé qué versión tengo?

Si tienes WordPress 5.2 o superior, el administrador de WordPress ya incluye herramientas que muestran esa información en la sección `Salud del sitio` (en el menú `Herramientas`).

Si tienes una versión más antigua, puedes activar la sección `Salud del sitio` instalando el plugin de la comunidad de WordPress llamado [Health Check & Troubleshooting](https://wordpress.org/plugins/health-check/) (más [ayuda para este plugin](https://make.wordpress.org/support/handbook/appendix/troubleshooting-using-the-health-check/)).

## Registro de cambios

- 2024-05-02: Actualizado de la versión principal en inglés.
