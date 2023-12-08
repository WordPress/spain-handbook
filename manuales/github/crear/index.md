# Crear una cuenta en GitHub

## Registrarse en GitHub

Para crearte una cuenta en GitHub, debes ir a su página principal [github.com](https://github.com/) y crearte una cuenta.

Haz clic en el botón *"Sign up"*, que está rodeado con un círculo rojo en la siguiente imagen:

![Imagen de la pantalla de bienvenida de Github y resaltado del botón Sign Up](https://raw.githubusercontent.com/WPES/spain-handbook/master/assets/manuales-wordpress-crear-cuenta-github.png)

## Activar el 2FA

Una vez que te hayas registrado, lo primero que deberás hacer es activar el 2FA, es decir, la autentificación de doble factor. GitHub nos obliga a hacer esto por seguridad.

Para activar el 2FA, no tienes más que hacer clic en la foto de perfil arriba, en la esquina derecha.


![Hacer clic en el avatar del perfil en la esquina derecha](https://raw.githubusercontent.com/WPES/spain-handbook/master/assets/activar-2FA-2.jpg)

A continuación, haz clic en la opción **Settings**.

![Haz clic en Settings](https://raw.githubusercontent.com/WPES/spain-handbook/master/assets/activar-2FA-1.jpg)

Una vez que haz entrado en los ajustes de tu perfil, puedes aprovechar para personalizar tu cuenta de GitHub (nombre, etc.). Y, a continuación, haz clic en **Password and authentication**.

![Haz clic en Password and authentification](https://raw.githubusercontent.com/WPES/spain-handbook/master/assets/activar-2FA-2.jpg)

Si haces un poco de scroll hasta el final de la página, verás que hay un botón que invita a activar la autentificación de doble factor. Haz clic en ese botón.

![Haz scroll hasta el final de la página y haz clic en Enable two-factor authentication](https://raw.githubusercontent.com/WPES/spain-handbook/master/assets/activar-2FA-3.jpg)

La aplicación te ofrecerá un proceso de tres pasos, que deberás completar con la ayuda de una herramienta de autentificación o de gestión de contraseñas como 1Password, Authy, Microsoft Authenticator, Google Authenticator, etc.

Una vez que tengas esta herramienta, que normalmente se trata de una app que podrás instalar en tu móvil, lo único que tendrás es que crear una contraseña nueva dentro de dicha herramienta, y te ofrecerá escanear el código QR que GitHub te está ofreciendo en pantalla. 

Una vez que lo hayas hecho, te ofrecerá un número de seis cifras, el cual deberás introducir en el espacio que hay debajo del código QR en pantalla, donde dice "**Verify the code from the app**". 

Si lo prefieres, este proceso lo puedes hacer también mediante SMS, como puedes ver un poco más abajo.

![Escanea el QR con una app de autentificación e introduce el código que te ofrece en la casilla bajo el mismo QR](https://raw.githubusercontent.com/WPES/spain-handbook/master/assets/activar-2FA-4.jpg)

En cualquier caso, se trata de hacer la doble autentificación con tu dispositivo móvil.

Una vez que hagas esto, verás que te aparece una pantalla con un montón de números. Estos códigos, o el archivo que te puedes descargar, deberás guardarlos en un lugar seguro ya que, si algún día no funcionase correctamente la autentificación de doble factor, **éstos códigos son tu llave para poder entrar a GitHub y no perder para siempre tu cuenta**.

Finalmente, una vez que hayas completado todo el proceso, tienes varias opciones para configurar métodos adicionales de autentificación como Passkey, llaves de seguridad físicas o con GitHub Mobile, que es el que recomendamos por su comodidad.

![Una vez finalizado el proceso puedes activar métodos adicionales de autentificación](https://raw.githubusercontent.com/WPES/spain-handbook/master/assets/activar-2FA-5.jpg)

## Instalar la App del móvil

Es conveniente que instales la App de GitHub para el móvil, ya que es la que te va a permitir autentificarte en su web utilizando el 2FA. Además, podrás recibir, si quieres, las notificaciones de cambios que puedan afectarte.

Si dispones de un dispositivo Android, puedes descargar la [aplicación de GitHub en Google Play](https://play.google.com/store/apps/details?id=com.github.android&hl=es_ES).

Si dispones de un dispositivo Apple, puedes descargar la [aplicación de GitHub en la Apple Store](https://apps.apple.com/es/app/github/id1477376905).

Una vez descargada, solo tienes que identificarte en ella y tenerla a mano para cuando te identifiques en la web.

## Instalar la App de Escritorio

Si eres un usuario que no ha utilizado nunca GitHub o Git, es preferible que realices todas tus colaboraciones desde la propia web de GitHub. De hecho, en este manual encontrarás todas las explicaciones para este caso.

Pero, si te dedicas al desarrollo web o tienes experiencia utilizando Git o GitHub, puede que te sientas con más comodidad trabajando en Escritorio. En ese caso, puede interesarte descargarte las diferentes herramientas de escritorio en tu ordenador.

### Herramienta oficial de GitHub

Con la herramienta oficial de GitHub puedes sincronizar el repositorio de GitHub con tu carpeta local, crear los commits, y enviar los cambios fácilmente. Para ello, puedes [descargar GitHub Desktop de su web oficial](https://desktop.github.com/).

### Visual Studio Code

Visual Studio Code es un IDE de programación muy extendido, creado por Microsoft, a quien también pertenece GitHub. Por este motivo, el editor está muy integrado con GitHub y es fácil trabajar con repositorios alojados en esta plataforma desde el escritorio. 

Si tienes experiencia y prefieres trabajar con esta herramienta, puedes descargar [Visual Studio Code desde su web](https://code.visualstudio.com/download).

## Una vez que tengas una cuenta de GitHub

Una vez que has creado tu cuenta, ya puedes acceder el [repositorio de WordPress en español](https://github.com/WordPress/spain-handbook), donde encontrarás todas las carpetas de los equipos con los diferentes manuales. Ten en cuenta que, para trabajar en ellas, deberás crear una nueva tarea (Issue) para proponer cambios, o bien solicitar en una tarea existente para que te sea asignada.

Si no tienes todavía cuenta en WordPress.org, puedes hacerlo siguiendo el [manual para crear una cuenta de WordPress.org](https://es.wordpress.org/team/handbook/handbook/manuales/wordpress/crear/).

Y si ya tienes una cuenta de WordPress.org, es importante que la sincronices con GitHub, ya que se reflejarán en tu perfil todas las contribuciones que realices con GitHub tanto en España como en la comunidad Global. Para ello, sigue el [manual para sincronizar tu cuenta de WordPress.org con GitHub](https://es.wordpress.org/team/handbook/handbook/manuales/wordpress/github/).