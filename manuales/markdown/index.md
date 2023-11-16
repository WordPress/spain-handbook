# Manual de Markdown

## Introducción a Markdown

### ¿Qué es Markdown?

Markdown es un lenguaje de marcado ligero creado por John Gruber en colaboración con Aaron Swartz. Fue diseñado para ser convertido fácilmente a HTML y muchos otros formatos. Es una herramienta escrita en texto plano, pero que permite incluir elementos de formato con una sintaxis sencilla y fácil de leer. Markdown se ha convertido en un estándar de facto para la creación de archivos README, así como para la documentación de proyectos de software, debido a su simplicidad y eficacia.

La sintaxis de Markdown incluye marcadores para títulos, listas, énfasis (negritas y cursivas), y más, utilizando caracteres no alfabéticos como `#`, `*`, y `-`. Por ejemplo, para crear un encabezado, simplemente se coloca un signo de número `#` antes del texto del encabezado. Para enfatizar una palabra o frase, se rodea con asteriscos o guiones bajos. Esto hace que sea muy intuitivo para los que están familiarizados con la edición de texto en estilo plano.

### ¿Por qué es importante para los usuarios de GitHub?

Para los usuarios de GitHub, Markdown es una herramienta esencial por varias razones:

1. **Documentación del proyecto**: Markdown se utiliza para crear archivos README eficientes y otros documentos de proyecto que son fundamentales para explicar y demostrar el uso y contribución a un proyecto.

2. **Colaboración**: Markdown permite a los usuarios de GitHub comunicar ideas e información de forma clara y estructurada. Esto es vital para la colaboración en proyectos, ya que facilita la comprensión del propósito y el funcionamiento del código.

3. **Integración con GitHub**: GitHub proporciona un soporte excelente para Markdown, permitiendo que los documentos formateados se visualicen directamente en la interfaz web de GitHub. Esto significa que la documentación es accesible y fácil de leer sin requerir herramientas adicionales.

4. **Universalidad**: Markdown es ampliamente utilizado y reconocido en la comunidad de desarrollo de software. Aprender Markdown puede ser beneficioso no solo para el trabajo en GitHub, sino también en muchos otros contextos de desarrollo y documentación.

5. **Flexibilidad**: Los archivos de Markdown pueden convertirse fácilmente en otros formatos como HTML, PDF, o incluso Word, lo que los hace versátiles para la distribución y publicación en diferentes plataformas y formatos.

En resumen, Markdown es una habilidad fundamental para los usuarios de GitHub, facilitando la creación de documentación efectiva y la comunicación entre colaboradores. Su simplicidad y versatilidad hacen que sea una elección óptima para la documentación de proyectos en GitHub.

## Elementos Básicos de Markdown

### Encabezados

Los encabezados en Markdown se crean utilizando el símbolo `#`. La cantidad de símbolos `#` antes del texto determinará el nivel del encabezado, con `#` siendo el más grande (equivalente a `<h1>` en HTML) y `######` el más pequeño (equivalente a `<h6>`). Aquí tienes un ejemplo de cómo se utilizan:

```markdown
# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6
```

Esto producirá una jerarquía de encabezados, que no solo agrega estructura visual al documento sino que también es importante para la accesibilidad y la navegación del contenido.

### Párrafos y saltos de línea

En Markdown, los párrafos se crean simplemente escribiendo texto en líneas separadas. No es necesario usar etiquetas adicionales; un cambio de línea en el código fuente marca el inicio de un nuevo párrafo. Para forzar un salto de línea sin comenzar un nuevo párrafo, puedes usar dos espacios en blanco al final de la línea antes de presionar Enter, así:

```markdown
Este es el primer párrafo.  
Y esta línea está separada del párrafo anterior por un salto de línea sin comenzar uno nuevo.
```

### Énfasis: negrita e itálica

Para enfatizar texto, puedes hacer palabras o frases en itálica o negrita. Para itálica, rodea el texto con un asterisco `*` o un guión bajo `_`. Para negrita, utiliza dos asteriscos `**` o dos guiones bajos `__`. También puedes combinar ambos para negrita e itálica.

```markdown
*texto en itálica*
_texto en itálica también_

**texto en negrita**
__texto en negrita también__

**_texto en negrita y itálica_**
```

Al aplicar estos elementos básicos, tu documento Markdown tendrá una estructura clara y será visualmente atractivo, facilitando a los lectores la comprensión de la jerarquía y la importancia de las secciones de tu contenido.

# Listas y Viñetas

Las listas son un componente fundamental en la escritura de Markdown y proporcionan una manera sencilla de presentar información en puntos o pasos secuenciales.

### Listas ordenadas

Para crear listas ordenadas, las cuales muestran una secuencia o jerarquía, se utilizan números seguidos de un punto. Markdown automáticamente ordenará los elementos de la lista incluso si los números no están en secuencia en el texto plano. Aquí hay un ejemplo:

```markdown
1. Primer ítem
2. Segundo ítem
3. Tercer ítem
```

Esto se mostrará en la documentación como una lista numerada, uno después del otro.

### Listas desordenadas

Las listas desordenadas usan asteriscos `*`, signos más `+`, o guiones `-` como marcadores de viñetas. Estos elementos son intercambiables y se eligen por preferencia. Por ejemplo:

```markdown
- Ítem uno
- Ítem dos
- Ítem tres
```

O alternativamente:

```markdown
* Ítem uno
* Ítem dos
* Ítem tres
```

Esto creará una lista con viñetas, donde el orden de los elementos no implica jerarquía o secuencia.

### Listas anidadas

Para crear listas anidadas, se añaden espacios o tabulaciones antes del marcador de viñeta o número. Puedes anidar listas ordenadas dentro de desordenadas y viceversa. He aquí un ejemplo:

```markdown
1. Primer ítem de la lista ordenada
   - Subítem desordenado
   - Otro subítem desordenado
2. Segundo ítem de la lista ordenada
   1. Subítem ordenado
   2. Otro subítem ordenado
```

Esto creará una lista con diferentes niveles de ítems, lo que es útil para mostrar relaciones jerárquicas entre ellos.

Usar listas correctamente en Markdown te permite organizar la información de una manera clara y coherente, facilitando la lectura y comprensión de tus documentos en GitHub.


## Enlaces e Imágenes

En Markdown, agregar enlaces e imágenes es una forma efectiva de enriquecer tus documentos, proporcionando referencias contextuales y visuales.

### Insertar enlaces

Para insertar un enlace, se utiliza la siguiente sintaxis:

```markdown
[Texto del enlace](URL "Título opcional")
```

- `Texto del enlace` es el texto que será clickeable.
- `URL` es la dirección web a la que el enlace apunta.
- `"Título opcional"` es un atributo de título que aparecerá como un tooltip en algunos navegadores cuando pasas el cursor sobre el enlace; es opcional.

Por ejemplo:

```markdown
[GitHub](https://github.com "Visita GitHub")
```

Esto creará un enlace a GitHub con el texto "GitHub" que se puede clickear.

### Insertar imágenes

La sintaxis para insertar imágenes es muy similar a la de los enlaces, pero se añade un signo de exclamación `!` al principio:

```markdown
![Texto alternativo](URL de la imagen "Título opcional")
```

- `Texto alternativo` es la descripción de la imagen que se muestra si la imagen no se puede cargar; también es utilizado por lectores de pantalla para accesibilidad.
- `URL de la imagen` es la dirección web donde se aloja la imagen.
- `"Título opcional"` funciona igual que en los enlaces.

Ejemplo:

```markdown
![Logo de GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png "Logo de GitHub")
```

Esto mostrará el logo de GitHub en tu documento Markdown.

### Enlaces para navegar entre documentos de Markdown en GitHub

Puedes crear enlaces entre documentos de Markdown en un repositorio de GitHub usando rutas relativas. Esto es útil para estructurar la documentación de tu proyecto en múltiples archivos. Por ejemplo:

```markdown
[Guía de Contribución](CONTRIBUTING.md)
```

Este enlace llevará al usuario al archivo `CONTRIBUTING.md` en el mismo directorio que el documento que contiene el enlace. Para referenciar un archivo en un directorio superior, puedes usar `..`:

```markdown
[Volver al README](../README.md)
```

Este enlace devolverá al usuario al archivo `README.md` ubicado un directorio por encima del actual.

Con estos elementos, puedes construir documentos ricos y conectados que faciliten a los usuarios navegar por tu proyecto y acceder a recursos visuales directamente desde GitHub.

## Código y Sintaxis

Markdown provee herramientas para incorporar código en tus documentos, lo cual es especialmente útil para la documentación técnica en GitHub.

### Código en línea

Para incluir código en línea dentro de un párrafo, lo envuelves con comillas invertidas (backticks), así:

```markdown
Para instalar las dependencias, ejecuta `npm install` en tu terminal.
```

El texto entre las comillas invertidas aparecerá como código dentro de la línea de texto.

### Bloques de código

Si necesitas incluir múltiples líneas de código, puedes usar tres comillas invertidas (```) o tres tildes (~~~) para crear un bloque de código. También puedes indentar cada línea con cuatro espacios o un tabulador, aunque la primera opción es más clara y permite el resaltado de sintaxis. Así es como se ve un bloque de código:

~~~markdown
 ```
function test() {
  console.log("notice the blank line before this function?");
}
 ```
~~~

## Resaltado de sintaxis específica de lenguaje

Markdown en GitHub soporta el resaltado de sintaxis para muchos lenguajes de programación. Para activar esta característica, especifica el lenguaje inmediatamente después de las comillas invertidas que abren el bloque de código:

~~~markdown
 ```javascript
function test() {
  console.log("¡HOLA!");
}
 ```
~~~

Reemplaza "javascript" con el lenguaje correspondiente al código que estás incluyendo. Esto ayudará a GitHub a colorear y formatear adecuadamente el código, haciéndolo más legible.

Utilizando estos métodos para incluir código, los documentos de Markdown se vuelven más interactivos y útiles para los usuarios que buscan implementar los ejemplos o entender mejor las funcionalidades de un proyecto en GitHub.

## Tablas

Las tablas son una manera efectiva de organizar y presentar datos de forma clara y estructurada en Markdown. Aquí te explicamos cómo crearlas, alinear texto en ellas y aplicar formato.

### Crear tablas

Puedes crear tablas usando barras verticales `|` y guiones `-` para separar columnas y filas. La primera fila de la tabla es generalmente el encabezado, seguido por una fila de guiones que define las columnas, y luego las filas de datos. Aquí tienes un ejemplo básico de una tabla en Markdown:

```markdown
| Encabezado 1 | Encabezado 2 | Encabezado 3 |
| ------------ | ------------ | ------------ |
| Dato 1       | Dato 2       | Dato 3       |
| Dato 4       | Dato 5       | Dato 6       |
```

Esto generará una tabla con dos filas de datos y tres columnas.

### Alineación de texto en tablas

Para alinear el texto en las columnas de las tablas, se utilizan dos puntos `:` junto con los guiones en la fila de definición de columnas. La alineación puede ser a la izquierda, a la derecha o centrada. A continuación se muestra cómo se aplica cada tipo de alineación:

```markdown
| Alineado a la izquierda | Centrado | Alineado a la derecha |
| :---------------------- | :------: | -------------------: |
| Texto                   | Texto    | Texto                |
| Más texto               | Más texto| Más texto            |
```

En este ejemplo, la primera columna está alineada a la izquierda, la segunda al centro y la tercera a la derecha.

### Formato de tablas

Markdown te permite añadir un formato básico dentro de las tablas, como poner texto en **negrita** o en _itálica_. También puedes incluir enlaces o imágenes en las celdas de la tabla. Sin embargo, el formato debe ser simple ya que no todas las funcionalidades de HTML están soportadas en las tablas de Markdown. Aquí hay un ejemplo de una tabla con formato:

```markdown
| **Negrita**           | _Itálica_             | `Código`                |
| :-------------------: | :-------------------: | :---------------------: |
| **Texto en negrita**  | _Texto en itálica_    | `Código fuente`         |
| [Enlace](#)           | ![Imagen](url)        | **_Combinado_**         |
```

El formato aplicado aparecerá en las celdas correspondientes, mejorando la presentación de la información en tus documentos de GitHub.

## Citas y Bloques de Cita

Las citas en Markdown son una forma de destacar texto, como citas textuales o para dar énfasis a comentarios o notas.

### Uso de citas

Para crear una cita en Markdown, utilizas el signo mayor que `>` seguido de un espacio y luego el texto de la cita. Esto se alineará el texto a la izquierda y lo distinguirá visualmente del resto del párrafo. Aquí tienes un ejemplo simple:

```markdown
> Esta es una cita en Markdown.
```

El resultado será un texto indentado con un estilo que indica que es una cita.

### Bloques de cita anidados

También puedes anidar bloques de citas dentro de otros bloques de citas agregando múltiples signos mayores que `>>`. Esto es útil para representar conversaciones o para responder a múltiples niveles de comentarios. Aquí te muestro cómo hacerlo:

```markdown
> Esta es la primera nivel de la cita.
>> Esta es una cita anidada dentro de la primera cita.
>>> Esta es una cita más profundamente anidada.
```

Cada nivel adicional de anidamiento aumentará la indentación del texto, permitiendo que los lectores sigan fácilmente la estructura de la conversación o los niveles de comentario.

Los bloques de cita pueden incluir otros elementos de Markdown, como encabezados, listas y código, lo que los hace muy versátiles para la creación de contenido enriquecido y bien estructurado en la documentación de GitHub.

## Elementos Adicionales

Más allá de los elementos de formato básico, Markdown también incluye la capacidad de agregar otros componentes útiles que pueden mejorar la interactividad y el atractivo visual de tus documentos.

### Líneas horizontales

Las líneas horizontales se utilizan para separar secciones de texto y se pueden crear usando tres o más asteriscos `***`, guiones `---`, o guiones bajos `___` en una línea por sí mismos. Aquí tienes un ejemplo:

```markdown
Esto es un texto que precede a una línea horizontal.

---

Y este es un texto que sigue a una línea horizontal.
```

Esto insertará una línea divisoria en tu documento que puede ayudar a organizar visualmente las secciones de contenido.

### Tareas pendientes (checkboxes)

Los checkboxes son una manera interactiva de listar tareas o ítems de acción y se crean utilizando corchetes. Para una casilla sin marcar, utiliza `[ ]`, y para una casilla marcada, `[x]`. Por ejemplo:

```markdown
- [ ] Tarea pendiente 1
- [ ] Tarea pendiente 2
- [x] Tarea completada
```

En GitHub, estas casillas son interactivas y pueden marcarse o desmarcarse directamente en la vista previa del archivo Markdown.

### Emojis

Puedes animar tus documentos de Markdown con emojis. Aunque no es parte de la especificación original de Markdown, GitHub tiene soporte para emojis utilizando `:nombre_del_emoji:`. Por ejemplo:

```markdown
:smile: Este es un emoji sonriente.
:thumbsup: Este es un pulgar hacia arriba.
```

GitHub convertirá estos códigos en los emojis gráficos correspondientes, permitiendo una comunicación más expresiva y amigable en tus documentos.

Estos elementos adicionales brindan maneras simples pero poderosas para añadir claridad, interactividad y un poco de diversión a tus archivos Markdown en GitHub, ayudando a captar la atención del lector y a organizar mejor tu contenido.

## GitHub Flavored Markdown (GFM)

GitHub Flavored Markdown (GFM) es la variante de Markdown que utiliza GitHub, incorporando características adicionales que están especialmente diseñadas para interactuar con la plataforma.

### Diferencias con Markdown estándar

Mientras que el Markdown estándar proporciona la base para la creación de documentos y comentarios en GitHub, GFM añade una serie de mejoras y extensiones para una integración más estrecha con la plataforma. Estas incluyen:

- **Tablas**: A diferencia del Markdown estándar, GFM permite la creación de tablas utilizando barras verticales y guiones.
- **Tachado**: GFM añade la posibilidad de tachar texto, lo cual no está disponible en el Markdown tradicional.
- **Autoenlace para URLs**: Las URLs se convierten automáticamente en enlaces clicables.
- **Listas de Tareas**: GFM introduce listas de tareas con casillas de verificación interactivas.

### Extensiones específicas de GitHub

GFM está diseñado para facilitar la colaboración entre usuarios en GitHub. Para ello, añade funcionalidades específicas que permiten la referencia y la interacción entre diferentes partes de la plataforma:

- **Menciones de Usuario**: Al igual que en las redes sociales, puedes mencionar a otros usuarios utilizando `@` seguido de su nombre de usuario. Esto les notificará sobre la mención.
  
- **Referencias a Issues y Pull Requests**: Puedes referenciar issues y pull requests utilizando el signo `#` seguido del número del issue o pull request. Esto crea un enlace directo al item correspondiente y ayuda a mantener una conversación organizada y rastreable.

- **Emojis**: GFM soporta una amplia gama de emojis que puedes incluir en tus documentos y comentarios.

- **Resaltado de Síntaxis**: GFM mejora el resaltado de sintaxis para soportar muchos lenguajes de programación y marcado, permitiendo que los fragmentos de código se muestren de manera más legible.

Estas extensiones de GFM están diseñadas para mejorar la experiencia de los usuarios en GitHub, permitiendo una documentación más dinámica y una comunicación más efectiva dentro de la plataforma.

## Consejos para Documentar Proyectos en GitHub

La documentación es esencial para cualquier proyecto en GitHub. Ayuda a los usuarios y colaboradores a entender qué hace tu proyecto, cómo pueden usarlo, y cómo pueden contribuir. Aquí hay algunos consejos para las partes más importantes de la documentación en GitHub.

### READMEs

El archivo `README.md` es a menudo el primer punto de contacto para quienes encuentran tu repositorio. Aquí hay algunas prácticas recomendadas:

- **Comienza con una introducción clara**: Explica el propósito de tu proyecto y para quién está diseñado.
- **Proporciona instrucciones de instalación**: Describe cómo los usuarios pueden instalar y configurar tu proyecto.
- **Incluye ejemplos de uso**: Ofrece ejemplos claros de cómo usar tu proyecto.
- **Detalla cómo contribuir**: Anima a otros a contribuir y explica el proceso para hacerlo.
- **Lista las dependencias**: Si tu proyecto depende de otros proyectos, asegúrate de listarlos.

### Guías de contribución

Un archivo `CONTRIBUTING.md` informa a los colaboradores potenciales cómo pueden participar en tu proyecto. Deberías:

- **Explicar el proceso de contribución**: Describe los pasos que los usuarios deben seguir para contribuir al proyecto.
- **Establecer las expectativas**: Ofrece una idea de qué tipo de contribuciones necesitas.
- **Definir estándares de codificación**: Mantén tu código organizado estableciendo y describiendo estándares de codificación y estilo.
- **Incluir información sobre pruebas**: Detalla cómo los colaboradores pueden probar sus cambios.

### Licencias

Incluir un archivo de licencia, como `LICENSE.md`, es crucial para informar a los usuarios sobre lo que pueden y no pueden hacer con tu código. Algunos puntos a considerar:

- **Elige la licencia adecuada**: Dependiendo de cómo deseas que otros usen y modifiquen tu proyecto, elige una licencia que refleje eso.
- **Sé claro y directo**: Utiliza una licencia estándar para evitar confusiones. Plataformas como [choosealicense.com](https://choosealicense.com/) pueden ayudarte a seleccionar una.
- **Coloca la licencia en un lugar visible**: Generalmente, esto significa tener un archivo `LICENSE` en la raíz de tu repositorio.

Documentar tu proyecto de manera efectiva en GitHub no solo facilita a los usuarios entender y usar tu proyecto, sino que también anima a una comunidad más amplia a contribuir y colaborar en tu trabajo.

## Integración de Markdown con el Editor de GitHub

GitHub proporciona un editor integrado para archivos Markdown que facilita la creación y edición de documentos con una vista previa en tiempo real. A continuación, te ofrezco algunos consejos para sacarle el máximo provecho.

### Editar y previsualizar documentos

- **Editor en línea**: Puedes editar archivos Markdown directamente en tu navegador utilizando el editor de GitHub.
- **Vista previa en vivo**: Mientras editas, GitHub te permite alternar entre la vista de edición y la de vista previa para ver cómo quedará tu documento una vez publicado.
- **Arrastrar y soltar**: GitHub te permite arrastrar y soltar imágenes en el editor, las cuales se cargarán y se enlazarán automáticamente en el documento.

### Uso de plantillas

- **Plantillas de issues y pull requests**: GitHub permite crear plantillas personalizadas para issues y pull requests utilizando Markdown, lo que ayuda a estandarizar la información que se solicita a los colaboradores.
- **Plantillas de repositorio**: También puedes definir plantillas para tus archivos README, CONTRIBUTING, y LICENSE para que cada nuevo repositorio comience con la documentación esencial.

### Atajos de teclado y trucos

- **Atajos de teclado**: GitHub soporta varios atajos de teclado para acelerar el proceso de edición. Por ejemplo, puedes presionar `Ctrl + B` para poner texto en negrita o `Ctrl + I` para cursiva.
- **Guardado automático de borradores**: Mientras editas, GitHub guarda automáticamente un borrador de tu trabajo, así que no perderás tus cambios si se cierra el navegador.
- **Sugerencias de autocompletado**: Al escribir un issue o pull request, puedes utilizar el símbolo `#` o `@` para obtener sugerencias de autocompletado para referenciar otros issues, pull requests o colaboradores.

Utilizando estas características de integración, los usuarios de GitHub pueden trabajar de manera más eficiente con documentos Markdown, desde la creación de contenido hasta la colaboración en el desarrollo del software.