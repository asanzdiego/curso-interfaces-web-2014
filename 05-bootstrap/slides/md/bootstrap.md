% Bootstrap, un framework CSS
% Adolfo Sanz De Diego
% Septiembre 2014



# El autor



## Adolfo Sanz De Diego

- **Antiguo programador web JEE (6 años)**

- Hoy en día:

    - **Profesor de FP (6 años)**:
        - Hardware, Sistemas Operativos
        - Redes, Programación

    - **Formador Freelance (3 años)**:
        - Java, Android
        - JavaScript, jQuery
        - JSF, Spring, Hibernate
        - Groovy & Grails

## Algunos proyectos

- Fundador y/o creador:

    - **Hackathon Lovers**: <http://hackathonlovers.com>
    - **Tweets Sentiment**: <http://tweetssentiment.com>
    - **MarkdownSlides**: <https://github.com/asanzdiego/markdownslides>

- Co-fundador y/o co-creador:

    - **PeliTweets**: <http://pelitweets.com>
    - **Password Manager Generator**: <http://pasmangen.github.io>

## ¿Donde encontrarme?

- Mi nick: **asanzdiego**

    - AboutMe:  <http://about.me/asanzdiego>
    - GitHub:   <http://github.com/asanzdiego>
    - Twitter:  <http://twitter.com/asanzdiego>
    - Blog:     <http://asanzdiego.blogspot.com.es>
    - LinkedIn: <http://www.linkedin.com/in/asanzdiego>
    - Google+:  <http://plus.google.com/+AdolfoSanzDeDiego>



# Introducción

## ¿Qué es?

- Boostrap es un **framework CSS, liberado por Twitter** y muy popular hoy en día.

- Está pensado para hacer un desarrollo **Mobile First**

## Ventajas (I)

- Utiliza componentes y servicios creados por la **comunidad web**.

- Utiliza un conjunto de **buenas prácticas** que perdurarán en el tiempo.

- Utiliza **HTML5 y CSS3**

## Ventajas (II)

- Implementa un **sistema de rejillas**, que por defecto incluye 12 columnas.

- Utiliza **LESS**, un preprocesador CSS. (Ahora también soporta Saas).

- Es **OOCSS**, osea CSS Orientado a Objetos: organizado por módulos independientes y reutilizables.

## Ventajas (III)

- Hay una enorme **comunidad detrás**.

- Herramienta **sencilla y ágil** para construir sitios web e interfaces.

- Tiene un **theme** por defecto bastante optimizado y que puedes modificar fácilmente.

## Desventajas (I)

- Es necesario **adaptarse a su forma de trabajo**, si bien su curva de aprendizaje es liviana, deberás comprender y familiarizarte con su estructura y nomenclatura.

- Debes adaptar tu diseño a un grid de **12 columnas**.

- Trae **anchos y márgenes por defecto**, que a veces son un poco tediosos de cambiar.

## Desventajas (II)

- Es complicado **cambiar de versión** si has realizado modificaciones profundas sobre el core.

- Si necesitas **añadir componentes que no existen**, debes hacerlos tú mismo en CSS y cuidar de que mantenga coherencia con tu diseño y cuidando el responsive.

- A veces hacer **implementar un diseño impuesto**, puede llegar a resultar bastante difícil, al menos si eres un perfeccionista.

## Descarga

- Si sólo quieres **lo fundamental**:

    - <https://github.com/twbs/bootstrap/releases/download/v3.2.0/bootstrap-3.2.0-dist.zip>

~~~
bootstrap/
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.min.css
│   ├── bootstrap-theme.css
│   └── bootstrap-theme.min.css
├── js/
│   ├── bootstrap.js
│   └── bootstrap.min.js
└── fonts/
~~~


## Plantilla básica

~~~
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta name="viewport"...>
    <title>Template</title>
    <link href="bootstrap.min.css"...>
  </head>
  <body>
    <h1>Hello, world!</h1>
    <script src=".../jquery.min.js">
    </script>
    <script src="bootstrap.min.js">
    </script>
  </body>
</html>
~~~



# Resumen CSS



## HTML5 doctype

- Bootstrap necesita un **doctype de HTML5**:

~~~
<!DOCTYPE html>
<html lang="en">
  ...
</html>
~~~

## Mobile first

- Desde la versión 3, Boostrap es **Mobile first**.

- Para garantizar un buen renderizado y un buen funcionamiento del zoom:

~~~
<meta name="viewport"
   content="width=device-width,
            initial-scale=1">
~~~

## Desactivar zoom (I)

- Se puede desactivar el zoom con **user-scalable=no**

~~~
<meta name="viewport"
   content="width=device-width,
            initial-scale=1,
            maximum-scale=1,
            user-scalable=no">
~~~

## Desactivar zoom (II)

- Hace que el sitio se parezca más una aplicación nativa, pero también lo hace **menos accesible**. En general, no se recomienda.

## Normalize.css

- Para un **mejor renderizado** en varios navegadores, Boostrap usa Normalize.css, un proyecto desarrollado por Nicolas Gallagher y Jonathan Neal:

    - <http://necolas.github.io/normalize.css/>



# Grid system



## Introducción

- Bootstrap incluye un **sistema de rejilla responsive y mobile first de 12 columnas**.

## Funcionamiento

- El sistema de rejilla de Bootstrap **funciona así**:

    - Se deben colocar .row dentro de un **.container** (ancho fijo) o **.container-fluid** (ancho completo).
    - Utilice **.row** para crear grupos horizontales.
    - El contenido se debe colocar entre .row y deben de ser **hijos inmediatos**.
    - Si hay más de 12 columnas en una .row, esta son desplazadas abajo.

## 1 columna (I)

- Ejemplo de 1 columna de un tamaño de 12

![1 columna](../img/1-columna.png)

## 1 columna (II)

- Ejemplo de 1 columna de un tamaño de 12

~~~
<div class="row">
  <div class="col-xs-12">1</div>
  <div class="col-xs-12">2</div>
  <div class="col-xs-12">3</div>
  <div class="col-xs-12">4</div>
</div>
~~~

## 2 columnas (I)

- Ejemplo de 2 columnas de un tamaño de 6

![2 columnas](../img/2-columnas.png)

## 2 columnas (II)

- Ejemplo de 2 columnas de un tamaño de 6

~~~
<div class="row">
  <div class="col-xs-6">1</div>
  <div class="col-xs-6">2</div>
  <div class="col-xs-6">3</div>
  <div class="col-xs-6">4</div>
</div>
~~~

## 3 columnas (I)

- Ejemplo de 3 columnas de un tamaño de 4

![3 columnas](../img/3-columnas.png)


## 3 columnas (II)

- Ejemplo de 3 columnas de un tamaño de 4

~~~
<div class="row">
  <div class="col-xs-4">1</div>
  <div class="col-xs-4">2</div>
  <div class="col-xs-4">3</div>
  <div class="col-xs-4">4</div>
</div>
~~~

## 4 columnas (I)

- Ejemplo de 4 columnas de un tamaño de 3

![4 columnas](../img/4-columnas.png)


## 4 columnas (II)

- Ejemplo de 4 columnas de un tamaño de 3

~~~
<div class="row">
  <div class="col-xs-3">1</div>
  <div class="col-xs-3">2</div>
  <div class="col-xs-3">3</div>
  <div class="col-xs-3">4</div>
</div>
~~~

## Multidispositivo

- 1 columna para xs (\<768px)
- 2 columnas para sm (≥768px)
- 3 columnas para md (≥992px)
- 4 columnas para lg (≥1200px)

## Normal

~~~
<div class="row">
  <div class="col-xs-12 col-sm-6
    col-md-4 col-lg-3">1</div>
  <div class="col-xs-12 col-sm-6
    col-md-4 col-lg-3">2</div>
  <div class="col-xs-12 col-sm-6
    col-md-4 col-lg-3">3</div>
  <div class="col-xs-12 col-sm-6
    col-md-4 col-lg-3">4</didv>
</div>
~~~

## clearfix (I)

- Problema cuando una capa tiene un alto mayor que la de los demás:

![Problema clearfix](../img/clearfix.png)

## clearfix (II)

~~~
<div class="row">
  <div class="...">1
    Resize your viewport</div>
  <div class="...">2</div>
  <div class="clearfix
    visible-sm-block"></div>
  <div class="...">3</div>
  <div class="clearfix
    visible-md-block"></div>
  <div class="...">4</didv>
</div>
~~~

## Huecos con offset (I)

![Huecos con offset](../img/offset.png)

## Huecos con offset (II)

~~~
<div class="row">
  <div class="col-md-4">
    .col-md-4</div>
  <div class="col-md-4
    col-md-offset-4">
    .col-md-4 .col-md-offset-4</div>
</div>
~~~

## Huecos con offset (III)

~~~
<div class="row">
  <div class="col-md-3
    col-md-offset-3">.col-md-3
      .col-md-offset-3</div>
  <div class="col-md-3
    col-md-offset-3">.col-md-3
      .col-md-offset-3</div>
</div>
~~~

## Huecos con offset (IV)

~~~
<div class="row">
  <div class="col-md-6
    col-md-offset-3">.col-md-6
      .col-md-offset-3</div>
</div>
~~~

## push & pull (I)

![push & pull](../img/push-and-pull.png)

## push & pull (II)

~~~
<div class="row">
  <div class="col-md-9
    col-md-push-3">
    .col-md-9 .col-md-push-3</div>
  <div class="col-md-3
    col-md-pull-9">
    .col-md-3 .col-md-pull-9</div>
</div>
~~~

## Media Queries (I)

- Estas son las Media Queries que se usan:

~~~
/* Extra small devices
   (phones, less than 768px) */
/* default in Bootstrap */

/* Small devices
   (tablets, 768px and up) */
@media (min-width: @screen-sm-min) {}

/* Medium devices
   (desktops, 992px and up) */
@media (min-width: @screen-md-min) {}

/* Large devices
   (large desktops, 1200px and up) */
@media (min-width: @screen-lg-min) {}
~~~

## Media Queries (II)

- A veces también usan max-witdh para limitar ciertas reglas.

~~~
@media (max-width: @screen-xs-max) {}

@media (min-width: @screen-sm-min)
    and (max-width: @screen-sm-max) {}

@media (min-width: @screen-md-min)
    and (max-width: @screen-md-max) {}

@media (min-width: @screen-lg-min) {}
~~~



# Tipografía



## Cabeceras (I)

![Cabeceras](../img/cabeceras.png)

## Cabeceras (II)

~~~
<h1>h1.Cabeceras con Bootstrap
  <small>Texto secundario</small></h1>

<h2>h2.Cabeceras con Bootstrap
  <small>Texto secundario</small></h2>
~~~

## Párrafos (I)

![Párrafos](../img/parrafos.png)

## Párrafos (II)

~~~
<p class="lead">
  Párrafo con class="lead"</p>

<p>Párrafo normal</p>

<p class="small">
  Párrafo con class="small"</p>
~~~

## Textos en línea

![Textos en línea](../img/textos-en-linea.png)

## strong

- mucho émfasis

~~~
<p>Puedes usar el tag strong para darle <strong>mucho émfasis</strong> a un texto</p>
~~~

## em

- émfasis

~~~
<p>Puedes usar el tag em para darle <em>émfasis</em> a un texto</p>
~~~

## mark

- marcar

~~~
<p>Puedes usar el tag mark para <mark>marcar</mark> un texto</p>
~~~

## ins

- insertar un texto (mejor que subrallar)

~~~
<p>Puedes usar el tag ins para <ins>insertar</ins> un texto</p>
~~~

## del

- borrar un texto (mejor que tachar)

~~~
<p>Puedes usar el tag del para <del>borrar</del> un texto</p>
~~~

## Alineación

![Alineación](../img/alineacion.png)

## Izquierda

- Texto alineado a la izquierda.

~~~
<p class="text-left">Texto alineado a la izquierda.</p>
~~~

## Centrado

- Texto centrado.

~~~
<p class="text-center">Texto centrado.</p>
~~~

## Derecha

- Texto alineado a la derecha.

~~~
<p class="text-right">Texto alineado a la derecha.</p>
~~~

## Justificado

- Texto justificado.

~~~
<p class="text-justify">Texto justificado.</p>
~~~

## Sin ajuste

- Texto sin ajuste.

~~~
<p class="text-nowrap">Texto sin ajuste.</p>
~~~

## Capitalización

![Capitalización](../img/capitalizacion.png)

## Minúsculas

- Minúsculas

~~~
<p class="text-lowercase">Lowercased text.</p>
~~~

## Mayúsculas

- Mayúsculas

~~~
<p class="text-uppercase">Uppercased text.</p>
~~~

## Tipo Título

- Tipo Título

~~~
<p class="text-capitalize">Capitalized text.</p>
~~~

## Abreviaturas (I)

![Abreviaturas](../img/abreviaturas.png)

## Abreviaturas (II)

~~~
<abbr title="HyperText Markup Language">HTML</abbr> es una abreviatura. Pasa el ratón por encima para averiguar de que se trata.
~~~

## Direcciones (I)

![Direcciones](../img/direcciones.png)

## Direcciones (II)

~~~
<address>
  <strong>Twitter, Inc.</strong><br>
  795 Folsom Ave, Suite 600<br>
  San Francisco, CA 94107<br>
  <abbr title="Phone">P:</abbr>
  (123) 456-7890
</address>

<address>
  <strong>Full Name</strong><br>
  <a href="mailto:#">info@name.com</a>
</address>
~~~

## Citas (I)

![Citas](../img/citas.png)

## Citas (II)

~~~
<blockquote class="blockquote">

  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>

  <footer>Someone famous in <cite title="Source Title">Source Title</cite></footer>

</blockquote>
~~~

## Listas (I)

![Listas](../img/listas.png)

## Listas (II)

~~~
<ul class="list-inline">
  <li>Peras</li>
  <li>Manzanas</li>
  <li>Naranjas</li>
  <li>Platanos</li>
</ul>
~~~

## Descripciones (I)

![Descripciones](../img/descripciones.png)

## Descripciones (II)

~~~
<dl class="dl-horizontal">
  <dt>Descripción</dt>
  <dd>Perfecta para definir.</dd>
  <dt>Euismod</dt>
  <dd>Vestibulum id ligula...</dd>
  <dt>Felis euismod semper eget</dt>
  <dd>Fusce dapibus, tellus ...</dd>
</dl>
~~~


# Tablas



## Clases

- **table**: para darle el formato
- **table-striped**: para darle formato a las pares y a las impares
- **table-bordered**: para ponerle bordes a la tabla
- **table-hover**: para oscurecer la fila en donde está el ratón
- **table-condensed**: para que ocupe menos espacio

## Responsive

- Poniendo la tabla dentro de una **capa con class=table-responsive** aparecerá un scroll horizontal en la tabla en dispositivos pequeños.

## Ejemplo (I)

![Tabla](../img/tabla.png)

## Ejemplo (II)

~~~
<div class="table-responsive">
  <table class="table table-striped  table-bordered table-hover table-condensed">
    <thead>
      <tr>
        <th>...
    </thead>
    <tbody>
      <tr>
        <td>...
    </tbody>
  </table>
</div>
~~~



# Formularios

## Lo básico (I)

- Agrupar label + control con **class=form-group**

- Input, textarea y select con **class=form-control**

## Lo básico (II)

- Layouts: **normal, form-inline y form-horizontal**

- Para distribuir el contenido, se puede **usar .col- pero no hace falta usar .row**

## Normal

![Formulario normal](../img/formulario-normal.png)

## Inline

![Formulario inline](../img/formulario-inline.png)

## Horizontal

![Formulario horizontal](../img/formulario-horizontal.png)

## Ejemplo

~~~
<form class="form" role="form">
  <div class="form-group">
    <label for="inputEmail3"
      class="col-sm-2 control-label">
      Email</label>
    <div class="col-sm-10">
      <input class="form-control"
       id="inputEmail3"
       placeholder="Enter Email"
       type="email">
    </div>
  </div>
  <div class="form-group">
    <div class="col-sm-offset-2
      col-sm-10">
      <button type="submit"
        class="btn btn-default">
        Sign in</button>
    </div>
  </div>
</form>
~~~

## Inputs

- Los de **HTML5**: text, password, datetime, datetime-local, date, month, time, week, number, email, url, search, tel, and color.

## Checkboxes and radios

- Se puede usar **class=checkbox-inline** o **class=radio-inline**

~~~
<div class="radio">
  <label>
    <input type="radio"
      name="optionsRadios"
      id="optionsRadios1"
      value="option1" checked>
      checked</label>
</div>
<div class="radio disabled">
  <label>
    <input type="radio"
      name="optionsRadios"
      id="optionsRadios3"
      value="option3" disabled>
      disabled</label>
</div>
~~~

## Validaciones (I)

![Formulario Validaciones](../img/formulario-validaciones.png)

## Validaciones (II)

- Usar los helpers **has-success, has-warning y has-error**

~~~
<div class="form-group
  has-success
  has-feedback">

  <label class="control-label"
    for="inputSuccess2">
    Input with success</label>
  <input type="text"
    class="form-control"
    id="inputSuccess2">
  <span class="glyphicon
    glyphicon-ok
    form-control-feedback"></span>
</div>
~~~

## Tamaños (I)

![Tamaños](../img/formulario-tamanios.png)

## Tamaños (II)

- Usar los helpers **form-group-lg o form-group-sm** o bien, en caso de inputs aislados que no estén dentro de un form-group, usar **input-lg o input-sm**

~~~
<form class="form-horizontal"
  role="form">
  <div class="form-group
    form-group-lg">
    <label class="col-sm-2
      control-label"
      for="formGroupInputLarge">
      Large label</label>
    <div class="col-sm-10">
      <input class="form-control"
        type="text"
        id="formGroupInputLarge"
        placeholder="Large input">
    </div>
  </div>
</form>
~~~

## Tamaños (III)

- Usar los helpers **form-group-lg o form-group-sm** o bien, en caso de inputs aislados que no estén dentro de un form-group, usar **input-lg o input-sm**

~~~
<form class="form-horizontal" role="form">
  <div class="form-group
    form-group-sm">
    <label class="col-sm-2
      control-label"
      for="formGroupInputSmall">
      Small label</label>
    <div class="col-sm-10">
      <input class="form-control"
        type="text"
        id="formGroupInputSmall"
        placeholder="Small input">
    </div>
  </div>
</form>
~~~


# Botones

## Ejemplos

![Ejemplos de botones](../img/botones-ejemplos.png)

## Tipos (I)

![Tipos de botones](../img/botones-tipos.png)

## Tipos (II)

~~~
<button type="button"
  class="btn">
  Button</button>

<button type="button"
  class="btn btn-default">
  Default</button>

<button type="button"
  class="btn btn-primary">
  Primary</button>

...
~~~

## Activados (I)

![Botones activados](../img/botones-activados.png)

## Activados (II)

~~~
<button type="button"
  class="btn active">
  Button</button>

<button type="button"
  class="btn active btn-default">
  Default</button>

<button type="button"
  class="btn active btn-primary">
  Primary</button>

...
~~~

## Desactivados (I)

![Botones activados](../img/botones-desactivados.png)

## Desactivados (II)

~~~
<button type="button"
  disabled="disabled"
  class="btn active">
  Button</button>

<button type="button"
  disabled="disabled"
  class="btn active btn-default">
  Default</button>

<button type="button"
  disabled="disabled"
  class="btn active btn-primary">
  Primary</button>

...
~~~


## Enlaces (I)

![Tamaños de los botones](../img/botones-enlaces.png)

## Enlaces (II)

~~~
<a href="#"
  class="btn btn-primary"
  role="button">
  Primary link</a>

<a href="#"
  class="btn btn-primary active"
  role="button">
  Primary link Active</a>

<a href="#"
  class="btn btn-primary disabled"
  role="button">
  Primary link Disabled</a>
~~~

## Tamaños (I)

![Tamaños de los botones](../img/botones-tamanios.png)

## Tamaños (II)

~~~
<button type="button"
  class="btn btn-primary btn-lg">
  Large button</button>

<button type="button"
  class="btn btn-primary">
  Default button</button>

<button type="button"
  class="btn btn-primary btn-sm">
  Small button</button>

<button type="button"
  class="btn btn-primary btn-xs">
  Extra small button</button>
~~~

## Expandir (I)

![Expandir los botones](../img/botones-expandir.png)

## Expandir (II)

~~~
<button type="button"
  class="btn btn-primary btn-lg
  btn-block">Large button</button>

<button type="button"
  class="btn btn-primary
  btn-block">Default button</button>

<button type="button"
  class="btn btn-primary btn-sm
  btn-block">Small button</button>

<button type="button"
  class="btn btn-primary btn-xs
  btn-block">Extra small</button>
~~~



# Imágenes



## Responsive

- Añadir **class=img-responsive** pondrá max-size=100% y height=auto.

## Efectos (I)

![Efectos de imágenes](../img/imagenes.png)

## Efectos (II)

- Se pueden añadir efectos:
    - **class=img-rounded**: redondea los bordes de la foto.
    - **class=img-circle**: convierte la foto en circular.
    - **class=img-thumbnail**: deja un pequeño recuadro a la foto.


# Helpers


## Textos coloreados (I)

![Textos coloreados](../img/textos-coloreados.png)

## Textos coloreados (II)

~~~
<p class="text-muted">
  text-muted</p>

<p class="text-primary">
  text-primary</p>

<p class="text-success">
  text-success</p>

<p class="text-info">
  text-info</p>

<p class="text-warning">
  text-warning</p>

<p class="text-danger">
  text-dangerx</p>
~~~

## Colores de fondo (I)

![Colores de fondo](../img/colores-de-fondo.png)

## Colores de fondo (II)

~~~
<p class="bg-primary">
  bg-primary</p>

<p class="bg-success">
  bg-success</p>

<p class="bg-info">
  bg-info</p>

<p class="bg-warning">
  bg-warning</p>

<p class="bg-danger">
  bg-danger</p>
~~~


## float y clearfix

~~~
<div class="pull-left">
  pull-left</div>

<div class="pull-right">
  pull-right</div>

<p>antes del clearfix</p>

<div class="clearfix"></div>

<p>después del clearfix</p>
~~~

## Mostrar y ocultar

~~~
<p>class=show > display: block</p>
<div class="show">show</div>

<p>class=hidden > display: none</p>
<div class="hidden">hidden</div>

<p>class=invisible > visibility: hidden (no desaparece del dom) </p>
<div class="invisible">invisible</div>

<p>class=text-hide</p> útil cuando quieres una imagen de fondo
<div class="text-hide">text-hide</div>
~~~

## Accesibilidad

~~~
<p>class=sr-only > solo aparece en los lectores de pantalla</p>

<p>class=sr-only-focusable > aparece cuando se hace foco sobre él</p>

<a class="sr-only sr-only-focusable" href="#content">Skip to main content</a>
~~~



# Responsive



## Esconder según dispositivo

~~~
<p class="hidden-xs
  bg-primary">hidden-xs</p>

<p class="hidden-sm
  bg-primary">hidden-sm</p>

<p class="hidden-md
  bg-primary">hidden-md</p>

<p class="hidden-lg
  bg-primary">hidden-lg</p>
~~~

## Mostrar como block según dispositivo

~~~
<p class="visible-xs-block
  bg-primary">visible-block-xs</p>

<p class="visible-sm-block
  bg-primary">visible-block-sm</p>

<p class="visible-md-block
  bg-primary">visible-block-md</p>

<p class="visible-lg-block
  bg-primary">visible-block-lg</p>
~~~

## Mostrar como inline según dispositivo

~~~
<p class="visible-xs-inline
  bg-primary">visible-xs-inline</p>

<p class="visible-sm-inline
  bg-primary">visible-sm-inline</p>

<p class="visible-md-inline
  bg-primary">visible-md-inline</p>

<p class="visible-lg-inline
  bg-primary">visible-lg-inline</p>
~~~

## Mostrar u ocultar para imprimir

~~~
<p class="hidden-print
  bg-primary">hidden-print</p>

<p class="visible-print-block
  bg-primary">visible-print-block</p>

<p class="visible-print-inline
  bg-primary">visible-print-inline</p>
~~~



# Componentes



## Iconos (I)

- Utiliza una versión reducida de **glyphicons**:
    - <http://glyphicons.com>

- Alternativa **Font-Awesome**:
    - <http://fortawesome.github.io/Font-Awesome>


## Iconos (II)

![Ejemplo de iconos](../img/iconos.png)

## Iconos (III)

~~~
<button type="button"
  class="btn btn-default">
  <span class="glyphicon
    glyphicon-star"></span> Star
</button>
~~~

## Dropdown (I)

![Dropdown](../img/dropdown.png)

## Dropdown (II)

~~~
<div class="dropdown">
  <button ... data-toggle="dropdown">
    Dropdown</button>
  <ul ... class="dropdown-menu"
    role="menu">
    <li role="presentation"
      class="dropdown-header">
      Header</li>
    <li role="presentation"
      class="divider"></li>
    <li role="presentation">
      <a role="menuitem"... href="#">
      Action</a></li>
  </ul>
</div>
~~~

## Button groups (I)

![Button groups](../img/button-groups.png)

## Button groups (II)

~~~
<div class="btn-group">
  <button type="button"
    class="btn
      btn-default">Left</button>

  <button type="button"
    class="btn
      btn-default">Middle</button>

  <button type="button"
    class="btn
      btn-default">Right</button>
</div>
~~~

## Input groups (I)

![Input groups](../img/inputs-groups.png)

## Input groups (II)

~~~
<div class="input-group">
  <span
   class="input-group-addon">
   @</span>
  <input type="text"
    class="form-control"
    placeholder="Username">
</div>
~~~

## Varios

![Tabs, pills, navbars, breadcrumbs](../img/varios.png)

## Tabs

~~~
<ul class="nav nav-tabs"
  role="tablist">
  <li class="active">
    <a href="#">Home</a></li>
  <li><a href="#">Help</a></li>
  ...
</ul>
~~~

## Pills

~~~
<ul class="nav nav-pills">
  <li class="active">
    <a href="#">Home</a></li>
  <li><a href="#">Help</a></li>
  ...
</ul>
~~~

## Navbars

~~~
<nav ...>
  <div class="container-fluid">
    <div class="navbar-header">
      <button ... id="collapse-1">
        <span class="sr-only">
        Toggle navigation</span>
        ...
      </button>
      <a class="navbar-brand"
        href="#">Brand</a></div>
    <div ... id="collapse-1">
      <ul class="nav navbar-nav
        navbar-right">
        <li><a href="#">Link</a></li>
        ...
      </ul></div>
  </div>
</nav>
~~~

## Breadcrumbs

~~~
<ol class="breadcrumb">
  <li><a href="#">Home</a></li>
  <li><a href="#">Library</a></li>
  <li class="active">Data</li>
</ol>
~~~

## Pagination (I)

![Pagination](../img/pagination.png)

## Pagination (II)

~~~
<ul class="pagination">
  <li class="disabled">
    <span>&laquo;</span></li>
  <li class="active">
    <span>1 
      <span class="sr-only">
      (current)</span>
      </span></li>
  <li><a href="#">2</a></li>
  <li><a href="#">3</a></li>
  <li><a href="#">4</a></li>
  <li><a href="#">5</a></li>
  <li><a href="#">&raquo;</a></li>
</ul> 
~~~

## Pager (I)

![Pager](../img/pager.png)

## Pager (II)

~~~
<ul class="pager">
  <li class="previous disabled">
    <a href="#">&larr; Older</a></li>
  <li class="next">
    <a href="#">Newer &rarr;</a></li>
</ul>
~~~

## Labels (I)

![Labels](../img/labels.png)

## Labels (II)

~~~
<span class="label
  label-default">Default</span>
<span class="label
  label-primary">Primary</span>
<span class="label
  label-success">Success</span>
<span class="label
  label-info">Info</span>
<span class="label
  label-warning">Warning</span>
<span class="label
  label-danger">Danger</span>
~~~

## Badges (I)

![Badges](../img/badges.png)

## Badges (II)

~~~
<ul class="nav nav-pills">
  <li class="active">
    <a href="#">Home
      <span class="badge">
        42</span></a></li>
  <li><a href="#">Profile</a></li>
  <li><a href="#">Messages
    <span class="badge">
      3</span></a></li>
</ul>
~~~

## Badges (III)

~~~
<button class="btn btn-default"
  type="button">Messages
  <span class="badge">4</span>
</button>
~~~

## Jumbotron (I)

![Jumbotron](../img/jumbotron.png)

## Jumbotron (II)

~~~
<div class="jumbotron">
  <h1>Hello, world!</h1>
  <p>...</p>
  <p><a 
    class="btn btn-primary btn-lg"
    role="button">
    Learn more</a></p>
</div>
~~~

## Thumbnails (I)

![Thumbnails](../img/thumbnails.png)

## Thumbnails (II)

~~~
<div class="row">
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="img.jpg"...>
      <div class="caption">
        <h3>Thumbnail label</h3>
        <p>...</p>
      </div>
    </div>
  </div>
</div>
~~~

## Alerts (I)

![Alerts](../img/alerts.png)

## Alerts (II)

~~~
<div class="alert alert-success"
  role="alert">
  <strong>Well done!</strong></div>
<div class="alert alert-info"
  role="alert">
  <strong>Heads up!</strong></div>
<div class="alert alert-warning"
  role="alert">
  <strong>Warning!</strong></div>
<div class="alert alert-danger"
  role="alert">
  <strong>Oh snap!</strong></div>
~~~

## Progress Bar (I)

![Progress Bar](../img/progressbar.png)

## Progress Bar (II)

~~~
<div class="progress">
  <div class="progress-bar"
    role="progressbar"
    aria-valuenow="0"
    aria-valuemin="0"
    aria-valuemax="100">
    0%</div></div>
<div class="progress">
  <div class="progress-bar"
    role="progressbar"
    aria-valuenow="2"
    aria-valuemin="0"
    aria-valuemax="100"
    style="width: 2%;">
    2%</div></div>
~~~

## Progress Bar (III)

~~~
<div class="progress">
  <div class="progress-bar
    progress-bar-success"
    ... style="width: 40%">
    <span class="sr-only">
      40% Complete (success)...
<div class="progress">
  <div class="progress-bar
    progress-bar-info
    progress-bar-striped"
    ... style="width: 20%">
    <span class="sr-only">
      20% Complete...
<div class="progress">
  <div class="progress-bar
    progress-bar-warning
    progress-bar-striped active"
    ... style="width: 60%">
    <span class="sr-only">
    60% Complete (warning)...
~~~

## Progress Bar (IV)

~~~
<div class="progress">
  <div class="progress-bar"
    style="width: 35%">
    <span class="sr-only">
    35% Complete (success)</span></div>
  <div class="progress-bar
    progress-bar-warning
    progress-bar-striped"
    style="width: 20%">
    <span class="sr-only">
    20% Complete (warning)</span></div>
  <div class="progress-bar
    progress-bar-danger
    progress-bar-striped active"
    style="width: 10%">
    <span class="sr-only">
    10% Complete (danger)</span>
  </div>
</div>
~~~

## Media (I)

![Media](../img/media.png)

## Media (II)

~~~
<ul class="media-list">
  <li class="media">
    <a class="pull-left" href="#">
      <img src="img.png">
    </a>
    <div class="media-body">
      <h4 class="media-heading">
        Media heading</h4>
      <p>...</p>
    </div>
  </li>
</ul>
~~~

## List group (I)

![List group](../img/listgroup.png)

## List group (II)

~~~
<div class="list-group">
  <a href="#"
    class="list-group-item active">
    Cras justo odio
  </a>
  <a href="#"
    class="list-group-item">
    Dapibus ac facilisis in</a>
    ...
</div>
~~~

## Panel group (I)

![Panel group](../img/panelgroup.png)

## Panel group (II)

~~~
<div class="panel panel-primary">
  <div class="panel-heading">
    <h3 class="panel-title">
    Panel title</h3></div>
  <div class="panel-body">
    Panel content</div>
  <div class="panel-footer">
    Panel footer</div>
</div>
~~~

## Responsive embed

~~~
<div class="embed-responsive
  embed-responsive-16by9">
  <iframe
    class="embed-responsive-item"
    src="//www.youtube.com/..."
    allowfullscreen=""></iframe>
</div>
~~~



# JavaScript



## Modal (I)

![Dialogos modales](../img/modal.png)

## Modal (II)

~~~
<button
  class="btn btn-primary btn-lg"
  data-toggle="modal"
  data-target="#myModal">
  Launch demo modal
</button>
~~~

## Modal (III)

~~~
<div class="modal fade" id="myModal"
  tabindex="-1" role="dialog"
  aria-labelledby="myModalLabel"
  aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        ...</div>
      <div class="modal-body">
        ...</div>
      <div class="modal-footer">
        ...</div>
    </div>
  </div>
</div>
~~~

## Tabs (I)

![Tabs](../img/tabs.png)

## Tabs (II)

~~~
<ul id="myTab" class="nav nav-tabs"
  role="tablist">
  <li class="">
    <a href="#home" role="tab"
      data-toggle="tab">
      Home</a></li>
  <li class="active">
    <a href="#profile" role="tab"
      data-toggle="tab">
      Profile</a></li>
  ...
</ul>
~~~

## Tabs (III)

~~~
<div id="myTabContent"
  class="tab-content">
  <div class="tab-pane fade"
    id="home">
    <p>...</p>
  </div>
  <div class="tab-pane fade
    active in" id="profile">
    <p>...</p>
  </div>
  ...
</div>
~~~

## Tooltips (I)

![Tooltips](../img/tooltips.png)

## Tooltips (II)

~~~
<script>
  $( document ).ready( function() {
    $('[data-toggle="tooltip"]')
      .tooltip();
  });
</script>
~~~

## Tooltips (III)

~~~
<p class="muted">
  Farm-to-table seitan, mcsweeney's
  fixie sustainable quinoa 8-bit
  american apparel
  <a href="#"
    data-toggle="tooltip"
    title="Another tooltip">
    have a</a>
  terry richardson vinyl chambray.</p>
~~~

## Tooltips (IV)

~~~
<button type="button"
  class="btn btn-default"
  data-toggle="tooltip"
  data-placement="right"
  title="Tooltip on right">
    Tooltip on right</button>
~~~

## Popover (I)

![Popover](../img/popover.png)

## Popover (II)

~~~
<script>
  $( document ).ready( function() {
    $('[data-toggle="popover"]')
      .popover();
  });
</script>
~~~

## Popover (III)

~~~
<button type="button"
  class="btn btn-default"
  title="Popover title"
  data-container="body"
  data-toggle="popover"
  data-placement="right"
  data-content="Vivamus
    sagittis lacus vel
    augue laoreet
    rutrum faucibus.">
      Popover on right
</button>
~~~

## Accordion (I)

![Accordion](../img/accordion.png)

## Accordion (II)

~~~
<div class="panel-group"
  id="accordion">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title">
        <a data-toggle="collapse"
          data-parent="#accordion"
          href="#collapseOne">
            Group Item #1</a>
      </h4></div>
    <div id="collapseOne"
      class="panel-collapse
        collapse in">
      <div class="panel-body">
        ...</div></div>
  </div>
  ...
</div>
~~~

## Carousel (I)

![Carousel](../img/carousel.png)

## Carousel (II)

~~~
<div class="container"
  style="max-width: 900px">
  <div id="carousel-example-generic"
    class="carousel slide"
    data-ride="carousel">
    <ol class="carousel-indicators">
      ...</ol>
    <div class="carousel-inner">
      ...</div>
    <a class="left carousel-control"
      ...</a>
    <a class="right carousel-control"
      ...</a>
  </div>
</div>
~~~

## Carousel (III)

~~~
<ol class="carousel-indicators">
  <li data-target="
    #carousel-example-generic"
    data-slide-to="0" class=""></li>
  <li data-target="
    #carousel-example-generic"
    data-slide-to="1"
    class="active"></li>
  <li data-target="
    #carousel-example-generic"
    data-slide-to="2" class=""></li>
</ol>
~~~

## Carousel (IV)

~~~
<div class="carousel-inner">
  <div class="item active left">
    <img src="img1.png"
      data-src="..."
      alt="First slide">
  </div>
  <div class="item next left">
    <img src="img2.png"
      data-src="..."
      alt="Second slide">
  </div>
  <div class="item">
    <img src="img2.png"
      data-src="..."
      alt="Third slide">
  </div>
</div>
~~~

## Carousel (V)

~~~
<a class="left carousel-control"
  href="#carousel-example-generic"
  role="button"
  data-slide="prev">
  <span class="glyphicon
    glyphicon-chevron-left"></span>
</a>
<a class="right carousel-control"
  href="#carousel-example-generic"
  role="button"
  data-slide="next">
  <span class="glyphicon
    glyphicon-chevron-right"></span>
</a>
~~~




# Ejemplos



## Índice

- Using the framework
- Navbars in action
- Custom components
- Experiments



### Using the framework

- Starter template
- Bootstrap theme
- Grids
- Jumbotron
- Narrow jumbotron

#### Starter template

- <http://getbootstrap.com/examples/starter-template>
![Source: getbootstrap.com](../img/screenshots/starter-template.jpg)

#### Bootstrap theme

- <http://getbootstrap.com/examples/theme>
![Source: getbootstrap.com](../img/screenshots/theme.jpg)

#### Grids

- <http://getbootstrap.com/examples/grid>
![Source: getbootstrap.com](../img/screenshots/grid.jpg)

#### Jumbotron

- <http://getbootstrap.com/examples/jumbotron>
![Source: getbootstrap.com](../img/screenshots/jumbotron.jpg)

#### Narrow jumbotron

- <http://getbootstrap.com/examples/jumbotron-narrow>
![Source: getbootstrap.com](../img/screenshots/jumbotron-narrow.jpg)



### Navbars in action

- Navbar
- Static top navbar
- Fixed navbar

#### Navbar

- <http://getbootstrap.com/examples/navbar>
![Source: getbootstrap.com](../img/screenshots/navbar.jpg)

#### Static top navbar

- <http://getbootstrap.com/examples/navbar-static-top>
![Source: getbootstrap.com](../img/screenshots/navbar-static.jpg)

#### Fixed navbar

- <http://getbootstrap.com/examples/navbar-fixed-top>
![Source: getbootstrap.com](../img/screenshots/navbar-fixed.jpg)



### Custom components

- Cover
- Carousel
- Blog
- Dashboard
- Sign-in page
- Justified nav
- Sticky footer
- Sticky footer with navbar

#### Cover

- <http://getbootstrap.com/examples/cover>
![Source: getbootstrap.com](../img/screenshots/cover.jpg)

#### Carousel

- <http://getbootstrap.com/examples/carousel>
![Source: getbootstrap.com](../img/screenshots/carousel.jpg)

#### Blog

- <http://getbootstrap.com/examples/blog>
![Source: getbootstrap.com](../img/screenshots/blog.jpg)

#### Dashboard

- <http://getbootstrap.com/examples/dashboard>
![Source: getbootstrap.com](../img/screenshots/dashboard.jpg)

#### Sign-in page

- <http://getbootstrap.com/examples/signin>
![Source: getbootstrap.com](../img/screenshots/sign-in.jpg)

#### Justified nav

- <http://getbootstrap.com/examples/justified-nav>
![Source: getbootstrap.com](../img/screenshots/justified-nav.jpg)

#### Sticky footer

- <http://getbootstrap.com/examples/sticky-footer>
![Source: getbootstrap.com](../img/screenshots/sticky-footer.jpg)

#### Sticky footer with navbar

- <http://getbootstrap.com/examples/sticky-footer-navbar>
![Source: getbootstrap.com](../img/screenshots/sticky-footer-navbar.jpg)



### Experiments

- Non-responsive Bootstrap
- Offcanvas

#### Non-responsive Bootstrap

- <http://getbootstrap.com/examples/non-responsive>
![Source: getbootstrap.com](../img/screenshots/non-responsive.jpg)

#### Offcanvas

- <http://getbootstrap.com/examples/offcanvas>
![Source: getbootstrap.com](../img/screenshots/offcanvas.jpg)



# Personalización



## Tu propio CSS

- Una forma de personalizar tu página web hecha con bootstrap, es **añadiendo un fichero CSS, después de las llamadas a los CSS de bootstrap** (para que sobrescriba los valores)

- Esta es una **forma muy manual y muy poco productiva**.

## Página Customize

- Desde la página web de bootstrap <http://getbootstrap.com/customize> se pueden **personalizar un montón de variables, y descargar una versión personaliada** de bootstrap.

![Personalizar desde la página web de bootstrap](../img/customize.png)

- Esta forma es más productiva, pero **sigue siendo bastante manual**, y además no puedes tener un control de cambios eficiente.

## Compilar Less

- La forma **más productiva y eficiente** de personalizar bootstrap es **compilando los ficheros Less del core a CSS**.



# Compilar Less



## Descarga

- Para ver **las tripas, y modificarlas (LESS)**, hay que descargar la versión completa:

    - <https://github.com/twbs/bootstrap/archive/v3.2.0.zip>

~~~
bootstrap/
├── less/
├── js/
├── fonts/
├── dist/
│   ├── css/
│   ├── js/
│   └── fonts/
└── docs/
    └── examples/
~~~

## Entorno

- Si queremos modificar el core (LESS), necesitamos:
    - intalar **NodeJS**,
    - luego **Grunt**
    - y para terminar instalar las **dependencias**.


## NodeJS

- NodeJS nos permite ejecutar **JavaScript del lado del servidor**.

- Para **instalar NodeJS**, hay que seguir las instrucciones de instalación de la página oficial para cada sistema operativo:
    - <http://nodejs.org>

## Grunt

- Grunt es un **automatizador de tareas** que se ejecuta sobre NodeJS.

- Una vez instalado NodeJS, **hay que instalar Grunt desde el gestor de paquetes de node (npm)** ejecutando  en un terminal, como administrador, el siguiente comando:

~~~
$ npm install -g grunt-cli
~~~

## Dependencias

- Una vez instalado NodeJS y Grunt, hay que **instalar las dependencias de bootstrap**.

- Para ello hay que situarse en la carpeta de bootstrap y ejecutar:

~~~
../bootstrap$npm install
~~~

## Default

- Si queremos lanzar **todas las tareas por defecto de grunt** (compilar, minificar, pasar los test, generar documentación...) tenemos que ejecutar lo siguiente

~~~
$ grunt
~~~

## Dist

- Si lo único que queremos es **compilar y minificar el CSS y el JavaScript**, tenemos que ejecutar lo siguiente:

~~~
$ grunt dist
~~~

## Watch

- También podemos **recompilar automaticamente los ficheros Less a CSS cuando salvas los cambios**, ejecutando el siguiente comando:

~~~
$ grunt watch
~~~

- El problema es que **sólo recompila ficheros Less a CSS, no los minifica**.

## Personalizar

- Uno de los ficheros que más se personaliza es **/bootstrap/less/variables.less**, pues en él están las variables más importantes que usa bootstrap.



# Acerca de



## Licencia

- Estas **transparencias** están hechas con:
    - MarkdownSlides: <https://github.com/asanzdiego/markdownslides>

- Estas **transparencias** están bajo una licencia Creative Commons Reconocimiento-CompartirIgual 3.0:
    - <http://creativecommons.org/licenses/by-sa/3.0/es>

## Fuentes

- Transparencias:
    - <https://github.com/asanzdiego/curso-interfaces-web-2014/tree/master/05-bootstrap/slides>

- Código:
    - <https://github.com/asanzdiego/curso-interfaces-web-2014/tree/master/05-bootstrap/src>

## Bibliografía

- Página oficial de Bootstrap:
    - <http://getbootstrap.com>

- Bootstrap sí, pero no
    - <http://bruno.garciaechegaray.com/Bootstrap.The.Melee/presentation>

- Ventajas y desventajas de usar Bootstrap
    - <http://jorgelessin.com/ventajas-y-desventajas-de-usar-bootstrap>
