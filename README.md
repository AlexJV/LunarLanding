# LMSGI-02. Proyecto Lunar Landing (HTML, CSS y JavaScript)
#### Descripción de la práctica.
Para realizar el proyexto Lunar Landing se debe desarrollar la primera parte de una aplicación web según el siguiente _StoryBoard_:  
![imagen HTML](storyboard.jpg)  
El objetivo es crear una aplicación web similar (diversas páginas web: _.html, css_ y imágenes), documentando todo el proceso en el presente _README.md_.
#### Desarrollo de la práctica:
En primer lugar se han creado tres archivos de texto plano, modificando sus extensiones para que sean las tres páginas que serán enlazadas y servirán para la práctica. Las tres páginas son:
 * _inicio_html_. Que servirá como página principal y contendrá los elementos del futuro _Lunar Landing_.
 * _creditos.html_. Utilizaré está página para elacionar las web y lugares de donde se han obtenido las imágenes y el apoyo para la tarea. 
 * _intrucciones.html_. Se realizará una breve descripción del juego y sus controles.

Descripción de los elementos contenidos en el _html_ de la página de inicio:
 * _!DOCTYPE HTML_: Definición del tipo de documento.
 * _html_: Representa la raíz de un documento HTML o XHTML. Todos los demás elementos deben ser descendientes de este elemento.
 * _head_: Representa una colección de metadatos acerca del documento, incluyendo enlaces a, o definiciones de, scripts y hojas de estilo.
 * _link_: Se ha utilizado para enlazar las hojas de estilos CSS externas con el documento HTML actual. En este caso existen dos hojas diferentes en función del tamaño de pantalla del dispositivo. Si tiene 721px de ancho o más, gracias al atributo _media_ aplicará el contenido de la hoja _estilo.css_(Primer _link_), en caso de tener menos de 721px de ancho aplicaría la hoja _estilo m.css_. Con el atributo _href_ le indicamos la ruta hasta la hoja de estilos referenciada.
 * _title_: Define el título del documento, el cual se muestra en la barra de título del navegador o en las pestañas de página. Solamente puede contener texto y cualquier otra etiqueta contenida no será interpretada.
 * _meta_: La usamos para relacionar aquellos metadatos que no pueden ser definidos usando otro elemento _html_. Utilizaremos el atributo _name="description" content=".."_ para describir brevemente el contenido de la página y, pese a que el texto no será visible en el navegador, lo utilizan los buscadores como resumen en sus páginas de resultados.
 * _body_: Para incluir en él todo el contenido principal del domcumento _html_.
 * _nav_: utilizada para contener los enlaces que favorezcan la navegación web y nos dirijan a zonas importantes.
 * _ul_ y _li_: Etiquetas que utilizaremos para crear una lista desordenada que contendrá los enlaces.
 * _div_: utilizada como un contenedor genérico, sin significado especial pero que ayudará a "nombrar" determinados elementos.
 * Atributos _id_ y _class_: Para asignar nombres a un elemento único (_id_) del _html_ o  para asignar un nombre de clase o conjunto de nombres de clases a un elemento (_class_).
 * _img_: La utilizaremos para insertar una imagen con la ayuda de los atributos _src_, donde indicaremos la ruta y _alt_ donde describiremos la imagen para que se muestre en el caso de que ésta no se muestre.

Otros elementos contenidos en las páginas _creditos_ o _instrucciones_:
 * _h1_ o _h3_: Son etiquetas de encabezados de diferentes tamaños.
 * _article_: Utilizada como separador de bloques para realizar divisiones con un nombre para cada una de ellas.
 * _header_: Utilizada para nombrar las cabeceras de algunas de las divisiones antes mencionadas.
 
Utilizando las etiquetas arriba descritas se ha estructurado la página _inicio.html_con dos listas desordenadas, una para mostrar la información del juego, como la altura, fuel o velocidad y la otra con los enlaces para abrir otras páginas.
Así mismo se han introducido dos imágenes en el _html_, una para la nave y otra para el paisaje lunar que servirá de superficie de aterrizaje.
La página _créditos.html_ tiene una estructura similar a la primera, ya que se ha optado por ordenar las fuentes de donde se han obtenido las imágenes utilizadas en la primera y en la segunda lista las referencias.

#### _CSS_. Argumentaciones técnicas y/o estéticas de las páginas creadas.
 
 Para la aplicación del estilo se ha utilizado la hoja _estilo.css_, referenciada en la etiqueta _link_ del _html_.
 Sin entrar en detalles respecto al estilo se describirán las generalidades técnicas y/o estéticas de cada uno de los elementos:
  * Diseño general de la página: Aplicado en la etiqueta _body_. Incluyendo fuente, tamaño y márgenes. Así mismo se aplica una imagen como fondo llamada _Estrellas.jpg_.
  * Menú izquierdo,identificado como "_menuA_", se le aplica una posición absoluta respecto a los elementos generales y un posicionamiento izquierdo en la pantalla con la etiqueta _float_.
  * Menú derecho, identificado como "_menuB_", se le aplica también una posición absoluta, pero en esta ocasión un posicionamiento derecho en la pantalla.
  * Imagen de la nave. Mediante el identificador (_id_) descrito en el _html_ se aplica una disposición central respecto a la pantalla.
  * Respecto al paisaje lunar, que fue identificado con una etiqueta _class_ en el _html_, se le aplica una posición absoluta, que se extienda al 100% de la pantalla y siempre en la parte baja de la misma.
  * En la página de créditos, se aplica similar configuración a los dos menús creados anteriormente (a los que en esta ocasión hemos llamado columnas), si bien éstos últimos se extienden por el 40% de la pantalla respectivamente (_width 40%_).
  * Se ha creado una segunda hoja de estilos, llamada _estilo_m.css_, en la que hemos adaptado el tamaño de las fuentes del texto y las configuraciones y tamaños de los menús, nave y columnas para que se visualicen de forma correcta en pantallas de menos de 721px.
  
#### Añadido JavaScript y adaptaciones del proyecto.

Pasos seguidos en la adaptación:

  * Se incorpora al proyecto el esqueleto conteniendo las instrucciones en JavaScript aportado por el tutor de la asignatura.
  * Añadir el efecto de fuego a la turbina del motor.
    * Nueva imagen para el fuego de la turbina en html e identificada con el div "fuegoimg".
    * En css se escala correctamente y se oculta para que sólo aparezca cuando se active el motor.
    * En js, en las funciones encender y apagar motor se referencia la imagen para que se muestre (block) cuando se requiere.
  * Adaptar el diseño a versiones móviles.
    * Con la ayuda del inspector de Chrome se realizan los ajustes en css para el correcto visionado en cualquier dispositivo.
  * Corregir altitud ya que aumenta en lugar de disminuir cuando se acerca al planeta.
    * Definidas nuevas variables para modificar la altitud.
       * Variable h: acumulará el cálculo de la altitud.
       * Variable alt: acumulará y mostrará el resultado del cálculo en la función  moverNave
    * Definida altitud de inicio en 60.22 para que sea 0 cuando se pose con el suelo lunar.
  * Añadir función de finalización del juego.
    * Se crea la nueva función (finjuego), definiendo como errónea toda velocidad de impacto superior a 7.
    *  Se define el gif que se mostrará sustituyendo a la nave si el vehículo impacta (naveKaput.gif).
    * Se crea en html (oculta en css) una pantalla de información de fin de juego (gameOver), vinculándola también en la función para que se muestre al finalizar.
    * Se añade un contador de intentos.
    * Se crea en html (oculta en css) una pantalla de información en caso de conseguir aterrizar el módulo (victoria). Se vincula a la función con un bulce para mostrarla en caso de que el resto de condiciones no se cumplan.
    * En ambas pantallas de información se añade un botón que permite reiniciar el juego.
  * Añadir función de reinicio.
    * Se crea la nueva función (reinicio) para que vuelva a empezar el juego tras finalizar (victoria o gameOver).
  * Modificar pantallas de instrucciones y créditos para que varíen en versiones móviles.
    * Adaptado css.
  * Actualizar Github con la nueva versión de Lunar Landing.
  * Crear nueva Branch para minify.
    * Modificados css y js adaptandolos a minify.
    * Actualizar Branch minify con el nuevo código.
 
