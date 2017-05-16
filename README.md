# Taller de iniciacion al desarrollo frontend

## Instalación del editor de código
Para este taller vamos a necesitar un editor de código, para aquellos que nunca han usado un editor de código recomiendo usar [brackets](http://brackets.io/), pero también podéis probar otros editores de código como [Atom](https://atom.io/) o [Sublime Text](https://www.sublimetext.com/).

Id a [brackets.io](http://brackets.io/) y descargar la aplicación que está disponible tanto para Windows como OS X y Linux. El proceso de instalación dependerá de la plataforma.

## Html 

Lo primero que tenemos que saber es que **Html** **NO** es un lenguage de programación, si no que es un lenguage de marcas, esto quiere decir que simplemente es un lenguaje que usamos para añadir información adicional de presentación o estructura a un texto. Así, de esta forma, podremos hacer cosas tansimples como escribir `<b>Hola Mundo!</b>` para escribir `Hola Mundo!` en negrita. Pongamos unos ejemplos de código `Html`:

- `<b>Hola Mundo!</b>` :

<b>Hola Mundo!</b>

- `<i>El frontend mola!</i>` :

<i>El frontend mola!</i>

- `<h6>Meetup Day</h6>` :

<h6>Meetup Day</h6>

Podemos ver el listado de todas las etiquetas *html* que hay en [w3schools](https://www.w3schools.com/tags/), aunque parezca un listado enorme, no os debéis preocupar porque sólo se suelen utilizar un pequeño número de ellas.

### Etiquetas no semánticas
Hay ciertas etiquetas que no añaden información al contenido al que envuelven, éstas etiquetas son `<div></div>` y `<span></span>` que simplemente nos ayudan a estructurar el documento y luego más tarde podremos modificar como se muestra su contenido en pantalla mediante reglas de estilo *Cascade StyleSheets* (*CSS*). La diferencia entre `<div></div>` y `<span></span>` la veremos más adelante.

También hay otras etiquetas no semánticas como `<b></b>` y `<i></i>` que sirven para añadir información de presentación, en este caso la primera etiqueta pondría el contenido que envuelve en negrita, y la segunda etiqueta pondría el contenido en itálica. Ambas etiquetas pueden ser combinadas de forma que `<b><i>Texto en negrita y cursiva</i></b>` es un texto en negrita y cursiva. El orden de las etiquetas no es importante en este caso, en cambio si que es importante que estén cerradas en orden, es decir, `<b><i>Texto en negrita y cursiva</b></i>` no sería *Html* válido.

### Etiquetas semánticas
Son aquellas que envuelven un contenido dotándolo de cierta información adicional semántica como `<h1></h1>` que indica que el texto que contiene es un encabezado, o `<article></article>` que indica que lo que hay dentro de esa etiqueta es un artículo.

El siguiente listado es una muestra de algunas de las etiquetas semánticas que hay:

- `<article>` : Artículo
- `<aside>` : Contenido secundario
- `<footer>` : Pie de un contenido, puede ser bien un pie de página, o bien un pie de sección o artículo en combinación con otras etiquetas.
- `<header>` : Cabecera de página, sección o artículo, dependiendo de cómo se componga con otras etiquetas.
- `<nav>` : Menú de navegación.
- `<p>`: Párrafo.
- `<h1>`, `<h2>`, `<h3>` ... : Textos de encabezados.
- `<strong>` : Resalta un texto destacando su importancia.
- `<em>` : Emfatiza un texto.

`<strong>` y `<em>` son las versiones semánticas de `<b>` y `<i>` puesto que `<strong>` presenta el texto en negrita, pero además resalta su importancia, igualmente `<em>` presenta el texto en cursiva, pero semánticamente enfatiza el contenido.

Formar el documento correctamente de estructura y semántica ayudará a que los robots de los buscadores indexen bien nuestro contenido y nuestra página.

## CSS (Cascade StyleSheets)
Ahora que ya estamos familiarizados con *Html* vamos a ver cómo se muestran esas etiquetas en pantalla. En este proceso vamos hablar sobre lo que se conoce como *mode lo de cajas* y las propiedades *CSS* que permiten que nuestras etiquetas se representen en pantalla con estilos diferentes al estilo que el navegador aplica por defecto a las etiquetas.

### Etiquetas de bloque y en linea

### Modelo de cajas

Las etiquetas de nuestro documento se renderizan en el navegador como cajas. Estas cajas tienen tienen diferentes secciones. En la imagen de abajo se puede ver cómo se estructuran las seciones de una caja.

![modelo de cajas](.github/images/box-model.png)

El ancho de la caja viene definido por el **ancho del contenido** más el **padding izquierdo y derecho** y el **borde izquierdo y derecho**, por otro lado la altura viene definida por **la altura del contenido** más el **padding superior e inferior** y el  **borde superior e inferior**. 

### Posicionamiento

CSS nos permite modificar el comportamiento para que nuestras etiquetas puedan renderizarse en otro lugar diferente al que se renderizarían por defecto. Para ello, utilizaremos la propiedad *CSS* `position`. Esta propiedad puede tomar cuatro valores: `static`, `relative`, `fixed` y `absolute`.

- **static**: Es el posicionamiento por defecto. Las etiquetas se renderizarán de arriba a abajo y de izquierda a derecha cuando las etiquetas se muestre en linea (con `display: inline`).

- **relative**: Nos permite *empujar* la etiqueta respecto a la posición en la que sería renderizada por defecto. Se puede usar en combinación de las propiedades *CSS* `top`, `right`, `bottom` y `left` para desplazarlo un número de *píxeles* u otra medida desde arriba, la derecha etc.

- **fixed**: Nos permite fijar un elemento o etiqueta en una posicion determinada de la pantalla. El elemento siempre permanecerá en esa posición de la pantalla aunque hamos *scroll*. También podremos usarlo en combinación con `top`, `right`, `bottom` y `left`, donde `top` será la parte superior de la pantalla, `right` será la parte derecha de la pantalla y así...

- **absolute**: Nos permite posicionar un elemento tomando como referencia el ancestro posicionado de manera diferente a `static`, de esta forma `top`, `right`, `bottom` y `left` harán referencia a ese elemento.

### Otras propiedades CSS

- `color` : color de la fuente
- `background-color`: color de fondo
- `background-image`: imagen de fondo
- `font-family`: tipo de fuente
- `font-size`: tamaño de la fuente
- `width`: ancho
- `height`: alto

[referencia de todas las propiedades *CSS*](https://www.w3schools.com/cssref/)

# Recursos

- [Learn to Code HTML & CSS from @shayhowe](http://learn.shayhowe.com/html-css/)
- [Tachyons](http://tachyons.io/)
- [Bootstrap](http://getbootstrap.com/)
