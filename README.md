# LMSGI-02. Proyecto Lunar Landing (HTML y CSS)
#### Descripción de la práctica.
Para realizar el proyexto Lunar Landing se debe desarrollar la primera parte de una aplicación web según el siguiente _StoryBoard_:  
![imagen HTML](storyboard.jpg)  
El objetivo es crear una aplicación web similar (diversas páginas web: _.html, css_ y imágenes), documentando todo el proceso en el presente _README.md_.
#### Desarrollo de la práctica:
En primer lugar se han creado tres archivos de texto plano, modificando sus extensiones para que sean las tres páginas que serán enlazadas y servirán para la práctica. Las tres páginas son:
 * _inicio_html_. Que servirá como página principal y contendrá los elementos del futuro _Lunar Landing_.
 * _creditos.html_. Utilizaré está página para elacionar las web y lugares de donde se han obtenido las imágenes y el apoyo para la tarea. 
 * _intrucciones.html_. Se realizará una breve descripción del juego y sus controles.

Descripción de los elementos contenidas en el _html_ de la página de inicio:
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
 
