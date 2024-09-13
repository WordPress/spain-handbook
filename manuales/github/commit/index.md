# Crear una instantánea de los cambios realizados en un documento

Al terminar la edición, para guardar los cambios, debemos hacer clic en el botón **Commit changes...**, que se encuentra sobre la ventana de edición.

![Hacer un commit para guardar los cambios](https://raw.githubusercontent.com/WordPress/spain-handbook/master/assets/commit-hacer-un-commit.webp)

A continuación aparecerá una ventana emergente que nos pedirá una pequeña descripción sobre lo que hemos hecho y, a continuación, una descripción más detallada donde podemos explicar a los moderadores el cambio que hemos realizado y por qué lo hemos hecho, o bien podemos comentar el nuevo texto que hemos añadido al documento y justificar por qué.

Si, además, estamos posicionados en la rama correcta, verás que estará marcada la opción `Commit directly to the nombre-de-la-rama`. Esto es importante, si no, nos da la oportunidad de crear la rama. 

Lo que no podemos hacer bajo ningún concepto es guardar los cambios en la rama `main`.

![Campos a rellenar antes de hacer el commit](https://raw.githubusercontent.com/WordPress/spain-handbook/master/assets/commit-campos-commit.webp)

Una vez realizado el _commit_, arriba saldrá un mensaje con nuestra descripción del commit y algunos datos más, y con el botón _History_ podremos consultar el historial de ediciones de ese archivo.

![Aviso de que hemos hecho el commit correctamente](https://raw.githubusercontent.com/WordPress/spain-handbook/master/assets/commit-aviso-commit-realizado.webp)

Pero aquí no ha terminado todo, ya que los cambios están en nuestro _Fork_, y debemos avisar al mundo de que hemos realizado estos cambios. Para ello, deberemos [solicitar revisión de los cambios](https://es.wordpress.org/team/handbook/manuales/github/pullrequest/) o como se llama en GitHub, haremos un _Pull request_.