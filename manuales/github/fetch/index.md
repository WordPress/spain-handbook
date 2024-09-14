# Sincronizar tu fork desde el repositorio personal (fetch)

Antes de empezar a trabajar en cualquier fork, es necesario sincronizarlo (actualizarlo) con el repositorio principal. Esto te asegurará que estás trabajando sobre la última versión del mismo.

Esto es porque, cuando se trabaja en una copia o _fork_, lo haces de forma paralela al repositorio principal (**wordpress/spain-handbook**) en tu cuenta de github (**micuenta/spain-handbook**).

Ya sabes, recuerda que para saber que estás en tu copia, verás la frase `forked from WordPress/spain-handbook` bajo el nombre del mismo.

![Indicación de que estamos en nuestro fork](/assets/fork-estamos-en-fork.webp)

En el caso de que acabes de crear el fork, y esté todo actualizado, verás un mensaje como éste:

`This branch is up to date with WordPress/spain-handbook:main`

Este mensaje indica que todo está actualizado y que no hay que sincronizar nada. De hecho, si intentas hacerlo, en el botón **Sync Fork**, verás que no aparece botón ninguno para poder sincronizar.

![Sync Fork cuando el repositorio está actualizado](/assets/fetch-si-todo-esta-sincronizado.webp)

Pero es posible que, mientras estés trabajando, otros contribuidores estén haciendo lo mismo en sus respectivos _forks_ y que hayan mandado sus cambios al repositorio principal. Esos cambios no se aplicarán en tu _fork_ hasta que no sincronices tu copia con el repositorio principal.

En ese caso, puede que te encuentres un mensaje como el siguiente, siempre en tu _fork_:

![Aviso de que hay cambios en el repositorio original](/assets/fetch-aviso-modificaciones-fork.webp)

Significaría que se han realizado 2 modificaciones en el repositorio original desde que hicimos nuestro _fork_.

En este caso, si el archivo principal se ha adelantado a nuestra versión, tenemos dos opciones: Contribute o Update branch.

Si **no hemos realizado aun cambios** en nuestro fork, para trabajar en la versión aceptada más actualizada del archivo principal (main), podemos pulsar en **Sync fork**, que nos dará a su vez la opción: _Update branch_.

![Actualizamos Rama](/assets/Fork-actualizar-rama.jpg)

Si **ya hemos editado nuestro archivo**, pulsaremos **Contribute**, aparecerá una pequeña ventana que indica que el archivo no está actualizado y nos invita a hacer un Pull request para solicitar que un moderador revise los cambios.

![Solicitamos Pull Request](/assets/Fork-contribute-send-PR.jpg)

**Compare** nos permite comparar las distintas versiones que se han creado.
En cualquier caso, si hubiera algún conflicto entre ambas versiones, el sistema nos avisará y nos invitará a hacer antes un _Pull request_.

Pero eso será más adelante, puesto que estamos en el supuesto de que estamos empezando a contribuir y todavía no hemos hecho ninguna edición.

El siguiente paso que debemos llevar a cabo es [crear una rama en nuestro fork](https://es.wordpress.org/team/handbook/manuales/github/rama/) para editar en ella sin peligro de modificar nada en la rama principal.