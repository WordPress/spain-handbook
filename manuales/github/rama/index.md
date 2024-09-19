# Crear una rama en tu fork

Una vez que hayas elegido el _issue_ que creas conveniente, debes crear una **rama** en la que trabajar. Esto es importante para que no haya colisiones cuando quieras enviar tu trabajo para fusionar con el del resto del equipo, puesto que no se puede trabajar en la rama principal (main), que es la que está publicada.

Antes de continuar, y para que lo veas de una forma gráfica, cuando se trabaja en GitHub, se parte de una rama principal (en azul), que es la que está publicada. Cada modificación que se haga en el texto, se aplicará sobre una rama que sale de la rama principal (las lineas de colores) y que, cuando ha sido finalizada y los cambios han sido aceptados, vuelve a fusionarse con la rama principal.

![Representación gráfica de las ramas](https://raw.githubusercontent.com/WordPress/spain-handbook/main/assets/rama-grafica-ramas.webp)

 Si te fijas en la siguiente imagen, volviendo a GitHub, en la columna de la derecha, donde se encuentran los ficheros, verás un desplegable en el que está seleccionado **main**. Eso quiere decir que estás trabajando sobre la rama **main** o principal de tu copia del repositorio (asegúrate arriba de que estás en _tu-usuario/spain-handbook/_).

 Por otro lado, en el centro de la página, te está indicando que esa rama se va a actualizar con los cambios que vengan del repositorio principal, de su rama **main** (_WordPress/spain-handbook:main_).

![Imagen en la que se comprueba en qué rama se está trabajando](https://raw.githubusercontent.com/WordPress/spain-handbook/main/assets/rama-crear-rama-1.webp)

Como queremos evitar colisiones, debemos trabajar en una rama nuestra, propia. Para ello, ve al desplegable mencionado antes, y despliégalo. Ahí debes escribir el nombre de la nueva rama.

Para que sea inteligible por parte de los moderadores, este nombre debe tener un formato que será:

**nombre_usuario_wordpress**-_nombre_asociado_al_issue_

Por ejemplo, imagina que has escogido un issue en el que la tarea es corregir el documento "Crear la estructura de archivos del manual de GitHub". Además, imagina que tu usario de tu perfil en WordPress es _uncontributorrandom_. El nombre de tu rama sería:

`uncontributorrandom-crear-rama`

![Imagen de cómo crear una nueva rama](https://raw.githubusercontent.com/WordPress/spain-handbook/main/assets/rama-crear-rama-2.webp)

Una vez que hayas escrito el nombre (en el ejemplo puedes ver que se llama _uncontributorrandom-crear-rama_), haz clic en **Create branch...** y ya tendrás creada la rama.

Asegúrate en el desplegable que estás editando en esa rama todo el tiempo.

![Imagen de cómo se verá que estás trabajando en una rama](https://raw.githubusercontent.com/WordPress/spain-handbook/main/assets/rama-crear-rama-3.webp)

Si vas a trabajar en otro issue, siénte libre de crear una rama nueva para trabajar en ese issue. **Pero te aconsejamos que no estés saltando de una rama a otra**, es preferible que vayas cerrando ramas e issues (tareas), para que así no haya confusiones.

Ahora estamos preparados para [editar el documento](https://es.wordpress.org/team/handbook/manuales/github/editardocumento/) en el que hemos elegido colaborar.