% Usabilidad Web
% Adolfo Sanz De Diego
% Agosto 2014

# El autor

## Adolfo Sanz De Diego

**Antiguo programador web JEE (6 años)**

Hoy en día:

-  **Profesor de FP (6 años)**:
    - Hardware, Sistemas Operativos
    - Redes, Programación

-  **Formador Freelance (3 años)**:
    - Java, Android
    - JavaScript, jQuery
    - JSF, Spring, Hibernate
    - Groovy & Grails

## Algunos proyectos

Fundador y/o creador:

-  **Hackathon Lovers**: <http://hackathonlovers.com>

-  **Tweets Sentiment**: <http://tweetssentiment.com>

-  **MarkdownSlides**: <https://github.com/asanzdiego/markdownslides>

Co-fundador y/o co-creador:

-  **PeliTweets**: <http://pelitweets.com>

-  **Password Manager Generator**: <http://pasmangen.github.io>

## ¿Donde encontrarme?

Mi nick: **asanzdiego**

-  AboutMe:  <http://about.me/asanzdiego>

-  GitHub:   <http://github.com/asanzdiego>

-  Twitter:  <http://twitter.com/asanzdiego>

-  Blog:     <http://asanzdiego.blogspot.com.es>

-  LinkedIn: <http://www.linkedin.com/in/asanzdiego>

-  Google+:  <http://plus.google.com/+AdolfoSanzDeDiego>

# Introducción

## ¿Qué?

Vamos a ver que es la **usabilidad de un sitio web y como mejorarla**.

## ¿Por qué?

**Mejora en la calidad del producto**: los sistemas que mejor se ajustan a las necesidades del usuario mejoran la productividad y la calidad de las acciones y las decisiones.

**Reducción de los costes de mantenimiento**: los sistemas que son fáciles de usar requieren menos entrenamiento, menos soporte para el usuario y menos mantenimiento.

**Reducción de los costes de producción**: los costes y tiempos de desarrollo totales pueden ser reducidos evitando el sobrediseño y reduciendo el número de cambios posteriores requeridos en el producto. 

**Un caso real**, después de ser rediseñado prestándose especial atención a la usabilidad, el sitio web de IBM incrementó sus ventas en un 400%

## ¿Cómo?

Primero **definiremos varios términos importantes**: usabilidad, accesibilidad, arquitectura de la información, experiencia de usuario y diseño centrado en el usuario.

Luego intentaremos **conocer al usuario**, saber como ve, como piensa y como actúa.

Después veremos como **evitando que el usuario cometa errores, y simplificando el diseño**, podemos mejorar la usabilidad.

También veremos la metodología del **diseño centrado en el usuario**, que se compone de varias fases: planificación, diseño, prototipado, evaluación, implementación y lanzamiento, y mantenimiento y seguimiento.

Seguidamente veremos **los principios de usabilidad y las técnicas de evaluación**: card-sorting, evaluación heurística, test de usuarios, eye-tracking, feedback, analítica web, tests A/B.

Para terminar propondremos varios varios **ejercicios** para realizar en clase en gruposde 3-4.

# Glosario de términos

## Usabilidad

Podemos observar que la usabilidad se compone de dos tipos de atributos:

-  **Atributos cuantificables de forma objetiva**: como son la eficacia o número de errores cometidos por el usuario durante la realización de una tarea, y eficiencia o tiempo empleado por el usuario para la consecución de una tarea.

-  **Atributos cuantificables de forma subjetiva**: como es la satisfacción de uso, medible a través de la interrogación al usuario.

Los usuarios no buscan usabilidad, buscan utilidad, entendida como el **provecho, beneficio e interés que produce su uso**.

Un producto será usable en la medida en que el **beneficio que se obtenga de usarlo justifique el esfuerzo necesario para su uso**.

Pensemos por ejemplo en los **automóviles**: son herramientas que requieren de un gran esfuerzo de aprendizaje y adaptación por parte de sus usuarios, aunque no por ello son percibidos como artefactos poco usables.

La usabilidad **no sólo es relativa a sus usuarios, sino también a los usos**. Por ejemplo, un **microondas** puede ser usado para guardar zapatos, pero no se pensó para eso, por lo tanto puede resultar no usable en ese contexto.

Además, **los objetivos y contextos previstos determinarán la importancia de su usabilidad**. Por ejemplo, un **teléfono móvil** puede ser usado para realizar una llamada de emergencia, o para escuchar las diferentes melodías que incorpora, un objetivo este último para el que la usabilidad puede que no sea tan relevante como para el primero.

## Accesibilidad

La accesibilidad se refiere a la capacidad del sistema a para **facilitar el acceso a todas las personas** en igualdad de condiciones, independientemente de la tecnología o soporte que utilicen y de la discapacidad que puedan presentar.

## Arquitectura Información

Disciplina que busca **organizar espacios de información** con el fin de ayudar a los usuarios a satisfacer sus necesidades de información.

La actividad de organizar **comporta la estructuración, clasificación y rotulado** de los contenidos.

La AI es el elemento que sostiene estructuralmente el contenido, por tanto, debe **definirse en las primeras etapas**, ya que de ella dependerán otros elementos del diseño.

El objetivo principal es **facilitar al usuario la recuperación de información**.

La recuperación de información es **una de las tareas de mayor importancia** para los usuarios.

Una **mala AI dificulta la búsqueda, y a la larga realizar otras tareas** (como comprar).

## Experiencia Usuario

Capacidad de una interfaz de **generar sensaciones y emociones**, en el usuario, durante el proceso de interacción.

## Diseño Centrado Usuario

Proceso de diseño y desarrollo (del sitio web) **conducido por el usuario**, sus necesidades, características e intereses.

# Conocer al usuario

## ¿Cómo ve?

Decidimos qué queremos atender visualmente, pero **nuestra atención se ve interferida involuntariamente y de forma automática por determinadas características visuales**, aún cuando hagan presencia en zonas de visión periférica.

En las interfaces web sucede igual: los usuarios escanearán visualmente la interfaz en busca de propiedades gráficas propias de los objetos deseados –enlaces, textos, imágenes, ...–, y esta **exploración puede verse facilitada si el diseñador enfatiza aquellos elementos potencialmente más relevantes**, o por el contrario entorpecida cuando nada parece visualmente más relevante que el resto.

La capacidad que tiene un elemento visual de atraer la atención del usuario se encuentra en directa **relación con sus diferencias gráficas** respecto a los elementos colindantes.

<div style="text-align:center">![Nos vemos involuntariamente atraídos por lo inusual. Fuente: nosolousabilidad.com](../img/inusual.png)</div>

Un elemento con **mayor tamaño** que el resto, con un **color distinto** a los demás, con una **orientación diferente**, o **en movimiento**, tendrá más probabilidad de atraer nuestra atención.

Esto es algo que comprendieron los **diseñadores de banners**, pero los usuarios aprendieron a ignorar automáticamente todo aquello que, por sus propiedades gráficas (y ubicación), pareciera información publicitaria (lo fuera o no).

La **publicidad contextual**, popularizada por Google, intenta atraer nuestra atención por el camino contrario: en vez de por medio de su diferenciación gráfica, mediante su similitud, de tal forma que el usuario tenga la impresión de que por su aspecto pueda tratarse de contenido de interés.

Mejorar el **diseño visual**:

<div style="text-align:center">![Mejorar el diseño visual. Fuente: nosolousabilidad.com](../img/principios-disenio-visual.png)</div>

**Enfatizar**: implica hacer visible lo relevante, establecer una clara jerarquía visual entre elementos y zonas de la interfaz, de modo que la atención del usuario se vea guiada de forma lógica y secuencial de lo más relevante hacia lo secundario.

**Organizar**: significa establecer relaciones visuales lógicas, que faciliten de este modo al usuario relacionar o diferenciar elementos automáticamente. Por ejemplo, que los enlaces tengan todos una misma caracterización gráfica (color, tipografía, efectos), facilita al usuario que, una vez detectado un enlace, pueda diferenciarlos automáticamente.

**Hacer reconocible**: considerar con especial cuidado el uso de iconos, encabezados, enlaces... de tal forma que se requiera del usuario el menor de los esfuerzos para comprender y predecir el funcionamiento interactivo de la interfaz.

## ¿Cómo piensa?

Cada vez que aprendemos algo extraemos nuestro propio **mapa mental**.

<div style="text-align:center">![Extracción de nuestro propio mapa mental. Fuente: nosolousabilidad.com](../img/extraccion-mapa-mental-2.jpg)</div>

¿Cómo **clasificaríamos** los colores?

¿Primarios, secundarios y terciarios?

¿O cálidos y fríos?

<div style="text-align:center">![Clasificación de los colores](../img/colores.jpg)</div>

¿Cúal de las 2 clasificaciones es mejor para mi interfaz?

Dependerá de nuestros usuarios.

Hay que intentar **adaptar nuestros contenidos a los mapas mentales** de nuestros usuarios.

Un usuario será capaz de identificar la función de cada elemento sólo **si ha aprendido previamente su significado**.

Además **el significado dependerá del contexto**. Un mismo usuario asociará sentidos diferentes a un enlace con el rótulo “Archivos”, en función de si se encuentra visitando un sitio web de noticias, un repositorio de software o la página web de una asociación de Bibliotecas, Museos y Archivos.

¿Cuales de estos formularios de búsqueda no utilizarías para tu interfaz web?

<div style="text-align:center">![Formularios de búsqueda. Fuente: nosolousabilidad.com](../img/busqueda.png)</div>

¿Cuales de estos calendarios no utilizarías para tu interfaz web?

<div style="text-align:center">![Calendarios. Fuente: nosolousabilidad.com](../img/calendarios.png)</div>

## ¿Cómo actúa?

Mecanismo **intuitivo**:

-  se caracteriza por ser muy rápido, susceptible a errores y fundamentalmente emocional

-  se disparan reglas automáticas o heurísticas –adquiridas en base a nuestra experiencia– que nos ofrecen una solución rápida, y nos posibilitan un comportamiento eficiente.

Mecanismo **racional**:

-  es un proceso lineal, lógico, consciente y que requiere esfuerzo y tiempo

-  es menos propenso a errores, además de que podemos –frente a un error– modificar el proceso, corrigiendo el resultado.

Normalmente empleamos el **sistema intuitivo pues nos permite economizar nuestro esfuerzo cognitivo**, y sólo usamos  **sistema racional para las decisiones realmente importantes**.

Esto explica por qué, por ejemplo, ante una ventana de alerta en la que se nos pregunta algo y se nos ofrecen dos posibles respuestas (sí y no), **es frecuente que automáticamente hagamos clic sin leer o procesar el contenido de la pregunta**.

El usuario explorará los ítems y **elegirá el primero que crea se corresponde con el contenido deseado**, aún cuando no todos hayan sido valorados.

La **ordenación alfabética sería una solución universal**, si no fuera porque no siempre somos capaces de verbalizar nuestra necesidad informativa y, aún cuando lo somos, dicha representación sintáctica no tiene por qué coincidir con el término utilizado en la interfaz.

La mejor solución es reducir el número de ítems, **agrupando aquellos semánticamente similares bajo rótulos descriptivos**, de tal forma que el usuario primero explorará los rótulos de cada grupo, y sólo cuando estime que se encuentran relacionados con su necesidad, explorará los ítems contenidos en el grupo.

Los usuarios sean idiotas, sino que **tienen mejores asuntos en los que emplear su esfuerzo cognitivo** que en comprender nuestro diseño. 

No todo a lo que atendemos es procesado racionalmente, lo que **nos lleva a cometer errores** frecuentemente.

# Evitar errores

## Limitar posibilidades

Siempre hay que tener en cuenta que cuantas menos opciones, menos posibilidades de error tendrá el usuario.

<div style="text-align:center">![Limitar posibilidades. Fuente: nosolousabilidad.com](../img/limitar.png)</div>

## Orientar al usuario

Ya sea mostrándole paulatinamente las distintas opciones, o mostrándoles pequeños mensajes informativos.

<div style="text-align:center">![Orientar al usuario. Fuente: nosolousabilidad.com](../img/orientar.png)</div>

## Solicitar confirmación

Antes de realizar una acción que no tiene vuelta atrás, hay que informar al usuario.

<div style="text-align:center">![Solicitar confirmación. Fuente: gmail.com](../img/confirmar.png)</div>

## Evitar la pérdida de información

En caso de error y vuelta atrás, el usuario no debería volver a introducir los datos.

<div style="text-align:center">![Evitar la pérdida de información. Fuente: nosolousabilidad.com](../img/ajax.png)</div>

## Permitir deshacer

Siempre que sea posible, hay que ofrecer al usuario la posibilidad de volver atrás.

<div style="text-align:center">![Permitir deshacer. Fuente: nosolousabilidad.com](../img/anterior-siguiente.png)</div>

## Ofrecer solución automática a los errores

No siempre es posible, pero si es deseable que el propio sistema sea capaz de ofrecer soluciones automáticas.

<div style="text-align:center">![Ofrecer solución automática a los errores. Fuente: nosolousabilidad.com](../img/did-you-mean.png)</div>

## Mensajes de error para humanos

Si aparece un mensaje de error este tiene que ser entendible por el usuario.

<div style="text-align:center">![Mensajes de error para humanos. Fuente: duckduckgo.com](../img/mensaje-error.png)</div>

# Simplicidad

## Reducción

Si prescindimos de un elemento, y el cambio no afecta a la comprensión del usuario, entonces su presencia no era necesaria.

<div style="text-align:center">![Reducción. Fuente: nosolousabilidad.com](../img/reduccion-2.png)</div>

## Espacios vacíos

Cuando separamos elementos en pantalla con espacios vacíos, o cuando eliminamos información irrelevante de ciertas zonas, **estamos guiando la atención del usuario hacia aquello que permanece y es relevante**.

Al contar **con menos elementos valoramos y confiamos más en aquello que es visible**, reforzando su percepción.

## Equilibrio de características

Al incrementar el número de características se observa **un efecto positivo sobre las capacidades percibidas, pero un efecto negativo sobre la usabilidad percibida**.

## Gráfico de Rob Tanenn

<div style="text-align:center">![Gráfico de Rob Tanenn. Fuente: nosolousabilidad.com](../img/grafico-de-rob-tanenn-2.png)</div>

## Organizar, clasificar y ordenar

Organizar, clasificar y ordenar **son también formas de simplificar**.

Por ejemplo, Google no simplifica los resultados de búsqueda por clasificación, sino por ordenación.

# Metodología DCU

## Fases

<div style="text-align:center">![Fases del diseño centrado en el usuario. Fuente: upf.edu](../img/disenio-centrado-usuario.png)</div>

## Planificación

Se basa en la **recogida, análisis y ordenación de toda la información posible**, con el objetivo de tener una base sólida sobre la que poder tomar decisiones de diseño en las siguientes etapas del proceso.

## Diseño

Diseñar o rediseñar, **en base al conocimiento obtenido** en la etapa de planificación, y en las etapas de prototipado y evaluación.

Dividido en varias subfases:

-  Modelado usuario

-  Diseño conceptual

-  Diseño de interacción

-  Diseño visual

-  Definición de estilo

-  Diseño contenidos

### Modelado usuario

Definición de **arquetipos de usuarios** que representan patrones de conducta, objetivos y necesidades.

Estos arquetipos, llamados "**personas**", son descripciones de usuarios, a los que se les da una identidad inventada: fotografía, nombre,... pero con los atributos, características y necesidades del arquetipo basados en información real extraída de la audiencia objetiva del sitio web.

Además se deben definir "**scenarios**" sobre los que poder contextualizar la interacción persona-aplicación web.

<div style="text-align:center">![Arquetipo 'persona'. Fuente: upf.edu](../img/persona.png)</div>

El diseñador **suele imaginarse a sí mismo usando el sitio** y por tanto suele ser incapaz de comprender por qué a alguien le puede resultar difícil, incomodo y hasta frustrante su uso.

Estos arquetipos de usuarios conseguirán que el diseñador **tenga en mente a un usuario 'real'**, con limitaciones, habilidades y necesidades reales.

### Diseño conceptual

Definición del **esquema de organización, funcionamiento y navegación del sitio**.

No se especifica qué apariencia va a tener el sitio, sino que se centra en su arquitectura de información.

### Diseño de interacción

Definir el comportamiento interactivo del sitio web, es decir, qué **acciones se ofrecerán al usuario en cada momento, y cómo responderá la aplicación** a las acciones que realice.

<div style="text-align:center">![Diagrama de diseño de interacción. Fuente: sopadepixels.com](../img/disenio-interaccion.png)</div>

### Diseño visual

Se especifica:

-  **composición** de cada tipo de página,

-  **aspecto y comportamiento** de los elementos de interacción y

-  **presentación** de elementos multimedia.

**“lo bonito” es percibido por el usuario automáticamente como más fácil de usar** (aunque desde un punto de vista objetivo realmente no sea tan fácil de usar).

<div style="text-align:center">![Botones. Fuente: nosolousabilidad.com](../img/botones.png)</div>

Ahora bien, **ofrecer un aspecto gráfico aparentemente tosco y poco cuidado puede aportar valor** en determinados contextos.

La estética, al igual que la usabilidad, es relativa a sus usuarios y contextos de uso.

### Definición de estilo

Es importante mantener una **coherencia y estilo común** entre todas las páginas.

Es útil elaborar una **guía de estilo** que sirva de documento referencia para todo el equipo de desarrollo.

### Diseño contenidos

**Seguir una estructura piramidal**: La parte más importante del mensaje debe ir al principio.

**Evitar ser irrespetuoso**: Intentar no dañar sensibilidades culturales, sociales, políticas, religiosas, o de cualquier otro tipo.

**Permitir una fácil exploración del contenido**: El lector en entornos Web, antes de empezar a leer, suele explorar visualmente el contenido para comprobar si le interesa. Usar los niveles de encabezado (h1, h2, h3, etc.), poner en relieve (negrita y/o distinto color) las partes fundamentales.

**Un párrafo, una idea**: Cada párrafo es un objeto informativo. Se deben trasmitir ideas, mensajes... evitando párrafos vacíos o varios mensajes en un mismo párrafo.

**Ser conciso y preciso**: Al lector no le gusta leer en pantalla. Hay que intentar eliminar los textos superfluos. Las páginas web no son novelas.

**Usar el vocabulario del usuario**: No se debe utilizar el vocabulario de la empresa o institución, sino el del usuario. Además debe ser sencillo y fácilmente comprensible.

**Tono familiar y cercano**: Así el lector prestará más atención. No hay que caer en la ordinariez.

## Prototipado

Algunas herramientas:

-  <http://moqups.com>

-  <http://gomockingbird.com>

-  <http://pencil.evolus.vn>

-  <http://balsamiq.com>

-  <http://www.mockflow.com>

-  <http://wireframe.cc>

-  <http://www.axure.com>

## Evaluación

La usabilidad la podemos mediante varias variables:

-  facilidad de aprendizaje (Learnability)

-  eficiencia

-  facilidad de ser recordado (Memorability)

-  eficacia

-  satisfacción

### Aprendizaje

Dificultad para llevar a cabo tareas básicas **la primera vez que se enfrentan al diseño**.

-  % tareas completadas en el primer intento

-  % de usuarios que completan las tareas en el primer intento

-  % de usuarios que necesitan ayuda en el primer intento

### Efectividad

Dificultad para llevar a cabo tareas concretas **una vez que los usuarios han aprendido el funcionamiento básico**.

-  % tareas completadas

-  % de usuarios que completan las tareas

-  % de usuarios que necesitan ayuda

### Reconocimiento

Dificultad para llevar a cabo tareas concretas **después de un periodo sin hacerlo**.

-  % tareas completadas pasado un cierto tiempo sin usar la interfaz

-  % de usuarios que completan las tareas pasado un cierto tiempo sin usar la interfaz

-  % de usuarios que necesitan ayuda pasado un cierto tiempo sin usar la interfaz

### Eficiencia

**Esfuerzo** que un usuario tiene que hacer para conseguir un objetivo.

-  tiempo en completar cada tarea

-  número de errores cometidos

-  nivel de gravedad de los errores

-  tiempo en recuperarse de los errores

-  clicks para completar la tarea

-  páginas visitas para completar la tarea

-  número de veces que solicita ayuda

### Satisfacción

Variables que tienen que ver más con lo **emocional o subjetivo**.

-  % de usuarios que lo recomendaría a un amigo

-  número de adjetivos positivos (o negativos) que cada usuario da al producto

-  % de usuarios que lo califican más fácil de usar que el de la competencia

-  % de usuarios que expresan satisfacción (o insatisfacción)

## Implementación y lanzamiento

Para controlar la calidad de la implementación se pueden **utilizar validadores** automáticos de código, así como validadores para testar de forma semi-automática el cumplimiento de directrices de accesibilidad en el código.

## Mantenimiento y seguimiento

Un sitio web **no es una entidad estática**, sus contenidos y su audiencia cambian, y por lo tanto requiere de continuos rediseños y mejoras.

Estos **rediseños deben ser muy sutiles**, pues aunque estos cambios estén fundamentados en problemas de usabilidad descubiertos post-lanzamiento, los cambios pueden resultar dramáticos para los actuales usuarios que ya estaban acostumbrados y familiarizados con el actual diseño.

# Principios usabilidad

## Visibilidad estado

El sistema (o sitio web) siempre debe **informar al usuario acerca de lo que está sucediendo**, como por ejemplo, cuando en una interfaz tipo webmail se adjuntan ficheros a un mensaje, el sistema debe informar del hecho mostrando un mensaje de espera.

## Adecuación al mundo real

El sistema debe hablar el **lenguaje del usuario**, huyendo de tecnicismos incomprensibles o mensajes crípticos.

## Libertad y control

El usuario debe tener el control del sistema, ser él el que decida.

Se debe ofrecer siempre una forma de "**salida de emergencia**", como por ejemplo la opción para "saltar" animaciones de introducción

## Consistencia y estándares

Consistencia en el **estilo** (enlaces iguales, pestañas iguales, etc.)

Seguir **estándares de diseño** ampliamente aceptados:

-  usar iconos conocidos y utilizados

-  icono de la empresa con enlace a la home arriba a la izquierda

-  menú en la parte superior

-  opciones a la izquierda o a la derecha

-  pie de página con un resumen del mapa de la web

## Prevención de errores

Mejor que un buen mensaje de error es un **diseño que prevenga** que ocurra el error.

## Reconocimiento antes que recuerdo

Hacer **visibles objetos, acciones y opciones** para que el usuario no tenga por qué recordar información entre distintas secciones o partes del sitio web o aplicación.

El usuario **no tiene por qué recordar** dónde se encontraba cierta información, o cómo se llegaba a determinada página.

## Flexibilidad y eficiencia

El sitio debe ser **fácil de usar para usuarios inexpertos**.

Pero también proporcionar **atajos o aceleradores para usuarios avanzados**.

## Diseño estético y minimalista

Las páginas **no deben contener información irrelevante o innecesaria**.

Cada **información extra compite con la información relevante** y disminuye su visibilidad.

## Manejo de errores

Los mensajes de error deben **expresar claramente cuál ha sido la causa** del problema.

También deben **sugerir las posibles alternativas o soluciones**, como por ejemplo mensajes del tipo "Usted quiso decir...".

Además se debe **guardar el contenido** introducido por el usuario para que no tenga que volver introducirlo y pueda subsanar el error.

## Ayuda y documentación

Aunque es mejor que un sitio web se pueda utilizar sin necesidad de ayuda o documentación, **en sitios web extensos o en procesos de interacción complejos se debe proporcionar información de ayuda** al usuario.

# Técnicas de evaluación

## Card-sorting

Esta técnica consiste en solicitar a un grupo de participantes que **agrupen los conceptos representados en tarjetas** por su similitud semántica.

<div style="text-align:center">![Card-sorting. Fuente: nosolousabilidad.com](../img/card-sorting.png)</div>

En el reclutamiento de participantes debemos asegurarnos de que:

-  los elegidos tienen **perfiles acordes con los usuarios reales** o potenciales del sitio web,

-  **muestran interés** por el tipo de sitio web a evaluar y, 

-  a ser posible, **tienen experiencia usando sitios web de naturaleza similar**.

El que los participantes estén motivados resulta crucial para el éxito de la prueba, por lo que será muy importante ofrecerles algún tipo de **remuneración o recompensa** por su colaboración en la prueba.

El card-sorting **abierto (sin categorias) tiene el objetivo de descubrir qué tipo de categorización o agrupación de los conceptos resultará más natural y acorde con el modelo mental** compartido de la audiencia del sitio web.

El card-sorting **cerrado (con categorias) es recomendable para evaluar si una categorización resulta predecible** para el usuario.

Dado que el abierto ayuda en la toma de decisiones organizativas, y el cerrado evalúa esas decisiones, **el abierto debe preceder al cerrado**.

Ambos tienen propósitos diferentes y complementarios y **su utilización combinada puede ofrecernos una imagen más fiel** el modelo mental del usuario.

Existen **aplicaciones que automatizan y facilitan la recogida de datos y su análisis estadístico**, por lo que son recomendables cuando el propósito es el análisis cuantitativo.

Como desventaja podemos señalar que **los participantes suelen encontrar más divertido el card-sorting manual**, y por tanto suelen estar más concentrados durante la tarea.

Los "conceptos" suelen **representar categorías u opciones de navegación**, y por tanto lo que se pretende es extraer cuál sería la mejor forma de agruparlas o clasificarlas.

Es una prueba destinada a adaptar la arquitectura de información al modelo mental del usuario, por tanto **tiene lugar en etapas tempranas** del proyecto.

## Evaluación heurística

Método de inspección de un sitio web que se basa en el **recorrido y análisis del sitio identificando errores y problemas de diseño**.

Normalmente la lleva a cabo un grupo reducido de evaluadores que, en base a **su propia experiencia**, fundamentándose en reconocidos **principios de usabilidad**, y apoyándose en **guías elaboradas para tal fin**, evalúan de forma independiente el sitio web, contrastando finalmente los resultados con el resto de evaluadores.

El número ideal de evaluadores debe ser entre 3 y 5: **con menos de 3 muchos problemas quedarán sin detectar, y con más de 5 aumentaría el coste** sin ofrecer resultados que los justificasen.

Cada evaluados examinará el diseño de forma independiente, y una vez finalicen, hacenn una puesta en común de los problemas, y elaborarán un **informe final consensuado**.

Cuanto más esperamos para su realización, más costoso resultará la reparación de los errores, por lo que **no sólo debemos realizar este tipo de pruebas una vez implementado, sino también, sobre los prototipos**.

Tiene como ventaja la **facilidad y rapidez** con la que se puede llevar a cabo.

Permite identificar **más problemas de usabilidad menores**, pero menos problemas de usabilidad mayores.

No puede sustituir al test de usuarios, ya que resulta **menos eficaz en la detección de problemas de usabilidad que mayor impacto** tendrán en el usuario final.

Puede reportar **falsas alarmas**, es decir, identificar como un problema de usabilidad aquello que realmente no lo es.

## Test de usuarios

Se basa en la **observación y análisis de cómo un grupo de usuarios reales utiliza el sitio web**, anotando los problemas de uso con los que se encuentran.

El número de participantes que son necesarios para detectar los problemas más importantes de usabilidad de un diseño se encuentra **en torno a 15**.

Es mejor llevar a cabo **3 pruebas, con 5 participantes por cada una, repartidas en diferentes momentos** del proceso de desarrollo.

El **reclutamiento de participantes, y su remuneración, es similar a la técnica de Card-Sorting**, anteriormente mencionada.

La **primera impresión** que se lleve el participante supone una información de gran relevancia para entender la capacidad comunicativa del diseño.

"**Test de 5 segundos**", con o sin objetivo concreto: mostrándole la página durante 5 segundos y preguntándole posteriormente cuál ha sido su primera impresión, qué contenidos cree que ofrece o puede encontrar en ese sitio web.

A continuación solicitaremos al participante una serie de tareas a realizar, analizando los errores que cometa, el tiempo empleado y su satisfacción. Es decir, **medimos tanto la usabilidad objetiva, como la usabilidad subjetiva**.

Requisitos de las tareas:

-  **Ser razonables**: Es decir, tareas típicas que un usuario real llevaría a cabo.

-  **Ser específicas**: La tarea no puede se demasiado genérica, sino que debe describir objetivos concretos.

-  **Ser factibles**: Encomendar al usuario tareas irrealizables no aporta información útil sobre los problemas reales.

Requisitos de las tareas:

-  **Estar descritas en términos de objetivos finales**: La tarea debe contextualizarse bajo un objetivo o motivación mayor.

-  **Duración razonable**: Si la tarea requiere demasiado tiempo, sería recomendable descomponerla en sub-tareas.

Una forma valiosa de obtener información consiste en **solicitar al participante que exprese verbalmente** durante la prueba qué está pensando, qué no entiende, por qué lleva a cabo una acción o duda.

Este protocolo tiene tiene el inconveniente de que el hecho de contar lo que uno hace y por qué lo hace **altera** la forma en la que se hacen las cosas.

Una alternativa consiste en que el participante **primero realiza la tarea y, una vez finalizada, expresa verbalmente** cómo recuerda que ha sido su proceso interactivo.

Cuanto más esperamos para su realización, más costoso resultará la reparación de los errores, por lo que **no sólo debemos realizar este tipo de pruebas una vez implementado, sino también, sobre los prototipos**.

Es una prueba complementaria a la evaluación heurística, pero **es más costosa, por lo que es recomendable realizarla siempre después de una evaluación heurística**.

Sus **resultados son más fiables, y posibilitan el descubrimiento de errores de diseño** imposibles o difíciles de descubrir mediante la evaluación heurística.

## Eye-tracking

Conjunto de tecnologías (hardware y software) que permiten **monitorizar y registrar la forma en la que una persona mira una determinada escena o imagen**, en concreto en qué áreas fija su atención, durante cuánto tiempo y qué orden sigue en su exploración visuales.

<div style="text-align:center">![Eye-tracking. Fuente: nosolousabilidad.com](../img/eye-tracking.png)</div>

Resultan **muy similares a los test con usuarios**, siendo diferente la tecnología usada para registrar el comportamiento del usuario, y siendo diferente lo que se pretende analizar con mayor detalle: la exploración visual del usuario.

Pequeños cambios en estos diseños, pueden hacer que los patrones de exploración varíen, por lo que es una técnica **recomendable sólo sobre diseños elaborados**.

Sigue siendo una **tecnología cara**.

Hay que tener en cuenta que ofrecen **datos cualitativos escondidos bajo la apariencia de datos cuantitativos**: analizar una interfaz con 5 participantes generará una gran cantidad de datos, pero desde el punto de vista estadístico, sigue siendo una muestra de 5 sujetos.

## Feedback

La información más valiosa sobre la usabilidad de un diseño **la obtenemos observando el comportamiento de los usuarios**, no preguntándoles.

Esto no quiere decir que el feedback de usuario no sea útil, sino todo lo contrario, pues nos ayuda a conocer la **satisfacción subjetiva del usuario**.

Esta información puede ser obtenida:

-  **de forma pasiva**: a través de los mensajes enviados por los usuarios

-  **de forma activa**: por medio de entrevistas, cuestionarios y encuestas

Las opiniones expresadas por los usuarios indican posibles problemas de usabilidad, pero **no son en sí mismas la respuesta a los problemas**.

Si un usuario envía un email preguntando por qué desde la home no encuentra un enlace al recurso X, no significa que debamos implementar este enlace, sino que posiblemente el recurso X sea poco visible o de difícil localización.

No se deben hacer preguntas del tipo "¿Preferiría que el diseño fuera de tal forma?", sino del tipo **"¿Ha tenido algún problema para localizar el recurso X?" ó "¿Le ha resultado fácil el uso de la herramienta X?"**.

## Analítica Web

Es una técnica que sólo puede llevarse a cabo **una vez que el sitio web ha sido lanzado** y es usado diariamente.

Se trata de una **técnica fiable y muy económica**, pues no hay sesgo ni necesidad de invertir en la identificación y reclutamiento de participantes.

Se trata de una información muy valiosa que puede servirnos para la **toma de decisiones sobre el rediseño** en sitios web implementados.

Existen muy diversas formas de aprovechar los datos a fin de mejorar la usabilidad:

-  **identificar los usuarios** de nuestra web (edad, sexo, estudios, etc.)

-  analizar dónde **hacen clic**,

-  comprobar **las horas de mayor uso** de nuestra web,

-  analizar que páginas de nuestro site son las **más visitadas**,

-  comparar dos páginas con la misma función pero diferente diseño (**Test A/B**),

Existen muy diversas formas de aprovechar los datos a fin de mejorar la usabilidad:

-  analizar las **rutas de navegación** que siguen los usuarios,

-  detectar donde se producen mayor número de **errores**,

-  analizar **las consultas** que hacen los usuarios en el buscador interno,

-  conocer **de donde llegan** los usuarios a nuestra página, 

-  etc.

## Test A/B

Consiste en **comparar dos versiones** de una misma página y ver cuál funciona mejor.

Se divide el tráfico de la página, de tal forma que **el un porcentaje vea la versión A y el otro la versión B**.

La alternativa que consiga **el objetivo buscado en más usuarios gana**.

<div style="text-align:center">![Test A/B. Fuente: elultimoblog.com](../img/test-a-b.jpg)</div>

**Cualquier elemento** de una página web (versión A) es susceptible de ser cambiado para generar una alternativa (versión B).

Puedes probar **títulos, subtítulos, o entradillas** alternativas para tus contenidos, puedes jugar con diferentes versiones de **color** y texto del botón de compra, puedes variar el **tamaño** de las ofertas, de los precios, del **orden** del menú...

**Identifica un problema o un punto de mejora**. “Muy pocos usuarios de los que vienen a mi web acaban visitando la página de precios de mi servicio, donde tengo el botón de comprar”.

**Investiga qué hacen los demás y cómo lo hacen**. Mira las páginas de inicio de tu competencia y aprende cómo otros incitan, desde su página de inicio, a visitar la página de precios.

**Plantea una posible solución**. “Si pongo un botón aquí haciendo hincapié en que las dos primeras semanas son gratis, creo que conseguiré aumentar las visitas a la página de precios.”

**Define la métrica para determinar el éxito del test**. Dependiendo del objetivo, podremos elegir: la tasa de conversión, la tasa de rebote, número de clicks, incluso si testamos una página de atención al cliente podemos poner como métrica el número de llamadas, o el número de mails.

**Crea la alternativa e inicia el experimento**. Crea la versión B con la solución que intuyes es mejor.

**Analiza los resultados**. Pasado un cierto tiempo, si la solución alternativa:

-  es mejor, establece esa alternativa como la versión por defecto

-  iguales, quédate con la que más te guste

-  es peor, has evitado integrar en tu web un cambio que te perjudicaría

Una herramienta gratuita y muy popular es **Google Website Optimizer**:

-  <http://www.google.com/websiteoptimizer>

Existen **otras alternativas** más completas, aunque de pago:

-  <http://www.ricardotayar.com/2012/01/15/herramientas-software-ab-testing-multivariante/>

# Ejercicios

## Normas generales

Dividir la clase en grupos de 3-4

Dividir los grupos en 2: izquierda y derecha

Cuando haya que puntuar:

-  1 punto: muy mal

-  2 puntos: mal

-  3 puntos: bien

-  4 puntos: muy bien

Una vez terminado el ejercicio se harán públicos los resultados y se comentarán en clase

## Card-sorting abierto

Grupo izquierda: usuarios

-  Hacen lo que les digan los diseñadores

Grupo derecha: evaluadores

-  Identificar items de una tienda de informática

-  Poner items en Post-It

-  Pasar Post-It a usuarios y que hagan agrupación libre

-  Después de resultados escoger categorías principales

## Card-sorting cerrado

Grupo izquierda: evaluadores

-  Pasar categorías y Post-It a usuarios y que hagan agrupación por categoría

-  Después de resultados hacer mapa mental de items

Grupo derecha: usuarios

-  Hacen lo que les digan los diseñadores

## Checklist de usabilidad

Los 2 grupos utilizarán la hoja de cálculo proporcionada en:

-  <http://olgacarreras.blogspot.com.es/2011/07/sirius-nueva-sistema-para-la-evaluacion.html>

Grupo izquierda: evaluará

-  <http://www.pccomponentes.com>

-  Poner los datos de varios evaluadores en común

Grupo derecha: evaluará

-  <http://www.latiendadeinformaticaonline.com>

-  Poner los datos de varios evaluadores en común

## Evaluación heurística

Grupo izquierda: maquetadores

-  Hacer prototipo de la tienda (las pantallas que hagan falta)

Grupo derecha: evaluadores

-  Consensuar puntos importantes a evaluar

-  Una vez terminados los prototipos, puntuarlos

-  Poner los datos de varios evaluadores en común

## Test de usuarios

Grupo izquierda: evaluadores

-  Consensuar puntos importantes a evaluar

-  Dar ordenes a los usuarios para hacer el test de los 5 segundos

-  Después de preguntar a los usuarios, puntuar los prototipos

-  Poner los datos de varios evaluadores en común

Grupo derecha: usuarios

-  Hacen lo que les digan los diseñadores

Grupo izquierda: usuarios

-  Hacen lo que les digan los diseñadores

Grupo derecha: evaluadores

-  Consensuar puntos importantes a evaluar

-  Dar ordenes a los usuarios para testear los prototipos

-  Después de observar como usan los usuarios los prototipos, puntuarlos

-  Poner los datos de varios evaluadores en común

## Test A/B

El profesor cogerá un prototipo y hará una pequeña modificación

El profesor enseñará los 2 prototipos a los alumnos

Los alumnos votarán a mano alzada cual les parece mejor

# Acerca de

## Licencia

Estas **transparencias** están hechas con:

-  MarkdownSlides: <https://github.com/asanzdiego/markdownslides>

Estas **transparencias** están bajo una licencia Creative Commons Reconocimiento-CompartirIgual 3.0:

-  <http://creativecommons.org/licenses/by-sa/3.0/es>

## Fuentes

Transparencias:

-  <https://github.com/asanzdiego/curso-interfaces-web-2014/01-usabilidad/slides>

Código:

-  <https://github.com/asanzdiego/curso-interfaces-web-2014/01-usabilidad/src>

## Bibliografía

Diseño Web Centrado en el Usuario: Usabilidad y Arquitectura de la Información

-  <http://www.upf.edu/hipertextnet/numero-2/diseno_web.html>

Informe APIE sobre Usabilidad

-  <http://www.nosolousabilidad.com/manual/index.htm>

Unas notas sobre Usabilidad

-  <http://www.slideshare.net/betabeers/usabilidad-18953630>

Pruebas de Usabilidad

-  <http://www.slideshare.net/pecesama/pruebas-de-usabilidad-10112899>

Métodos de Usabilidad y Diseño Centrado en el Usuario

-  <http://www.slideshare.net/GUINALIU/mtodos-de-evaluacin-de-usabilidad>

Prototipado

-  <http://www.slideshare.net/olgacarreras/prototipado-14077585>

Usabilidad y diseño centrado en la experiencia del usuario

-  <http://www.slideshare.net/laceves/usabilidad-y-diseo-centrado-en-la-experiencia-del-usuario>

¿A qué esperas para usar Test A/B en tu web? ¡Tu competencia ya lo hace!

-  <http://www.elultimoblog.com/test-ab/>
