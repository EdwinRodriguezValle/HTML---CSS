/* CODE KHAN ACADEMI*//*____________________________________________________________________________________*/



/* La a se usa para anclar a conexiones website*/
<a></a>
<a href="#" <img src="https://cdn.kastatic.org/third_party/javascript-khansrc/live-editor/build/images/cute/StoneBlock.png" alt ="techo" width=100% height="50">

/* targe sirve para abrir el link en una nueva pagina*/
<a  target="_blank" href="#" <img src="https://cdn.kastatic.org/third_party/javascript-khansrc/live-editor/build/images/cute/StoneBlock.png" alt ="techo" width=100% height="50">



/*Link externos con al a y el target para direccionar a página en blanco, y a src para direccionar a un imagen*/
 <a target="_blank" href="https://www.cedla.nl/">" src="<img src="https://www.kasandbox.org/programming-images/cute/Heart.png">University of Utrecht</a>


 /* para hacer saltos internos. Tienes que conectar con el id de la parte al cual quieres saltar. Se construye con la propiedad tale*/

        <a href="#kangaroos">Locomotion</a>,
        <a href="#diet">Diet</a>

/*Como crear y llenar tablas en HTML*/
        <body>

        <h1>My Pets</h1>
        
        <ul>
            <li>Black & white (rabbit)</li>
            <li>Daemon (cat)</li>
            <li>Angel (cat)</li>
        </ul>
        
        <table>
            <thead>
                <tr>
                    <th>Pet name</th>
                    <th>Species</th>
                    <th>Color</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Black & white</td>
                    <td>rabbit</td>
                    <td>black and white</td>
                </tr>
                <tr>
                    <td>Daemon</td>
                    <td>cat</td>
                    <td>black</td>
                </tr>
                <tr>
                    <td>Angel</td>
                    <td>cat</td>
                    <td>orange</td>
                </tr>
            </tbody>
        </table>
        
    </body>
    

/*CSS GARDEN: Tercer bloque/
/* con font-size. Puedes cambiar en pixseles y tambien con "em" puedes hacer que sea dos veces más grande que el cuerpo o relativo a la página*/
 style
 h2{
  font-size: 10px;
 }
 h1{
   font-size:10em;

  }
  /* font-wide*/

  h1{
    font-weight: 10px;
    font-style: italic; /*se usa para cambiar estilos de normal a itlaic, negrita,tec*/
    font:100px italic red; /*también se puede hacer de esa manera*/
  }
  p{
    line-height: 1.5em; /* sirve para especificar la altura*/
    font-style:italic;
    text-decoration: line-through; /*sirve par subrayar el texto*/
    text-align: center;
    text-decoration: none;/*sirve para remover surayados de hiperlinks*/
  }

  /*CSS grouping elements. Sirve para agrupar y hacer cambios rápidos entre ellos esta <span></span>, <div></div>, */

  /*<div> /*agrupa bloques */
 /* <span> /*estos sirve para agrupar elementos*/

  /*Ajustar la caja de contenido y el contenido*/
  #official-info {
    background: rgb(230, 230, 230);
    width: 70%;
    height: 180px; 
    overflow: auto; /* Esto ajusta el texto al tama;o de la caja, puede ser hiddin, overflow */
    margin:auto; /*creo una caja centrada */
    padding: 10px;
    border-collapse: separate;
  }


  /* Float y clear*/

  #hopper-pic {
    width: 100px;
    float: left; /*siempre funciona con left, right y tiene que ir acompa;ado por un width y su porcentaje*/
    margin-right: 6px;
    margin-bottom: 6px;
  
    
}
#hopper-footer {
    background-color: rgb(232, 232, 232);
    padding: 6px;
    clear: both; /*clear sirve para indicar que un elemento no se sobre escriba o no se amontone */

}

/*dar formato solo a ciertas clases en un selector como parrafo o h*/
p.warning{
  color:violet; /*esto dará color solo a los parrafos que tenga la etiqueta warning. Esta es una manera de dar formato fácil*/
}
/*SELECCIÓN DESCENDIENTE*/
<title>CSS descendant selectors</title>
<style>
    .orange {
        background-color: orange;
    }
    
    .yellow {
        background-color: yellow;
    }
    
    .purple {
        background-color: purple;
        color: white;
    }
    
    p .purple { /*de esta manera puedes seleccionar un bloque gandre de elementos dentro de su contenedor*/
        color: purple;
        background-color: transparent;
    }
    
    ul li strong{
      font-size-adjust: 10px;
    }
    ul.spacey li strong {/*esta manera de seleccionar es más espcifico*/
        line-height: 2em;
    }
</style>
</head>
<body>

<h1>Carrot Facts</h1>

<p>Colors that carrots come in:</p>
<ul class="spacey">
    <li>
        <strong class="orange">Orange</strong>
    </li>
    <li>
        <strong class="purple">Purple</strong>
    </li>
    <li>
        <strong class="yellow">Yellow</strong>
    </li>
</ul>

<p>Did you know? Carrots were <strong class="purple">purple</strong> before the 17th century, but then were cultivated by Dutch farmers until they became the sweet orange carrots that we know today.</p>

</body>

/*AGRUPAR SELECTORES. Para darles el mismo estilo se agrupan usando comas*/

h1, h2{
  color: violet;
}


/*Seudo clases*/
<title>CSS dynamic pseudo-classes</title>
        <style>
            body {
                font-family: sans-serif;
            }
            
            h1, h2 {
                font-family: cursive;
            }
            
            a:link {
                color: red;/*formatea el link y dar color*/
            }
            a:visited {
                color: orange; /*marca en un color especifico las aréas vistadas por el usuario*/
            }
            a:hover { 
                background-color: rgb(255, 214, 255); /*colorea el area donde pasas con el mause*/
            }  
            a:active {
                background-color: rgb(255, 214, 255);/*formatea el area por donde estan los link*/
            } 
            a:focus {
                background-color: rgb(255, 214, 255); /*salta el lugar donde esta importante o puedes darle formato*/
            } 
            /*se puede usar también de esta manera*/
            h1:hover, h2:hover{
              color:blue;
            }
        </style>

/*Usar estilos de CSS externos*/

<link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/pamelafox/69f97167ba32e3473cda/raw/336006010d620847f275b0bd25bbf7c665b2e1a1/hopper.css">

/*coger fuentes en linea*/
<link href='https://fonts.googleapis.com/css?family=Josefin+Sans' rel='stylesheet' type='text/css'>
        <style>

/*FRECODECAMP. VISUAL DESIGN*/

p{
  
text-align: justify; /*spaces the text so that each line has equal width.*/

text-align: center; /*centers the text*/

text-align: right; /*right-aligns the text*/

text-align: left; /*a la izquierda*/

text-decoration: underline;/*subrraya*/
<u></u> /*subrraya también en html */

text-decoration: line-through;/*Subrraya el texto*/
<s></s>/*en html*/

<hr> /* para poner lineas en HTML, se cierra solo*/


}


img {
  width: 220px; /* Ajusta el ancho de un elemento*/
  height: 20px; /* controlo el alto, cuando alto quieres el elemento*/
}


/*AJUSTE DE COLORES */

/*Aprende sobre colores complementarios. El círculo cromático es una herramienta útil para observar cómo los colores están relacionados entre sí - es un círculo donde los tonos similares están juntos y los tonos diferentes alejados. Cuando dos colores opuestos están juntos en el círculo, se los llama colores complementarios. Se caracterizan porque si se combinan, se cancelan así mismos y crean un color gris. Sin embargo, al ubicarse juntos, estos colores parecen más brillantes y producen un contraste visual fuerte.*/
rojo (#FF0000) y cian (#00FFFF)
verde(#00FF00) y magenta (#FF00FF)
azul (#0000FF) y amarillo (#FFFF00)



/*Aprende sobre colores terciarios. Los monitores y las pantallas crean diferentes colores al combinar cantidades de luz roja, verde y azul. Esto se conoce como modelo aditivo de color RGB en la teoría de moderna de color. Rojo (R), verde (G) y azul (B) «por sus siglas en inglés» son colores primarios. Al combinar dos colores primarios se los colores secundarios cian (G + B), magenta (R + B) y amarillo (R + G). Ya viste estos colores en los desafíos de colores complementarios. Estos colores secundarios son el complemento del color primario no utilizado en su creación y están frente a ese color primario en el círculo cromático. Por ejemplo, el magenta está compuesto de rojo y azul y es el complemento del verde.

Los colores terciarios se forman al combinar dos colores primarios con uno de sus vecinos de color secundario. Por ejemplo, entre el modelo de color RGB, rojo (primario) y amarillo (secundario) forman naranja (terciario). Esto añade seis colores a un círculo cromático simple para un total de doce.

Hay varios métodos para seleccionar colores diferentes que resultan de una combinación armoniosa en diseño. Un ejemplo que puede usar colores terciarios es el esquema de color complementario dividido. Este esquema comienza con un color base, luego lo empareja con los dos colores que están adyacentes a su complemento. Los tres colores proporcionan un fuerte contraste visual en un diseño, pero son más sutiles que utilizar dos colores complementarios.

Aquí hay tres colores creados usando el esquema de dividir-complemento:*/

Color	Código hexadecimal
anaranjado	#FF7F00
cian	#00FFFF
frambuesa	#FF007F


 /*rgba() color*/
p{
background-color: rgba(45, 45, 45, 0.1)
  r = red
  g = green
  b = blue
  a = alpha/level of opacity
}

  /* hsl()= High Saturation Light*/
 
p{
hsl(180, 90%, 20%);

}





/*Tamano de la fuente*/
p{
font-size:0pc; /*controla el tamano de la fuente, también puede ser grande, mediano o corto*/
font-weight: bold;/*estos convierte en negrita */
<strong> </strong>/*dentro de html lo pone el negrita*/

font-style: italic;/* pone en italics*/
<em></em> /*en html */
}

/* La propiedad *box-shadow  Genera sobra en la caja*/
p{

  - offset-x /*(how far to push the shadow horizontally from the element),*/
  - offset-y /*(how far to push the shadow vertically from the element),*/
  - blur-radius, 
  - spread-radius and,
  - color, in that order.

  Multiple box-shadows can be created by using commas to separate properties of each box-shadow element.
  box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
}

/*opacidad. Decrease the Opacity of an Element. Aplica a todo tipo de elementos*/
A value of 1 is opaque, which isn't transparent at all.
A value of 0.5 is half see-through.
A value of 0 is completely transparent.
 
p{
  opacity: 0.5;
}

/*Transformadores de texto */

p{
  text-transform: lowercase;
}

-lowercase	
-uppercase	"TRANSFORM ME"
-capitalize	"Transform Me"
-initial	Use the default value
-inherit	Use the text-transform value from the parent element
-none	Default: Use the original text

/*Se recomeinda agrupar los selectores para tener una visibilidad general. Asi se recomeinda darles formato*/

<h1>This is h1 text</h1>
<h2>This is h2 text</h2>
<h3>This is h3 text</h3>
<h4>This is h4 text</h4>
<h5>This is h5 text</h5>
<h6>This is h6 text</h6>

Set the font-weight of the h1 tag to 800px.
Set the font-weight of the h2 tag to 600.
Set the font-weight of the h3 tag to 500.
Set the font-weight of the h4 tag to 400.
Set the font-weight of the h5 tag to 300.
Set the font-weight of the h6 tag to 200.

/*controla la altura de los lineas */
p{
  line-height: 25px;
}


/* Para cambiar de color un elemento cunaod pasas por encima el mause*/
a:hover {
  color: red;
}


/*POSICIONAMIENTO */
RELATIVO: Mueve elemento dentro de su caja padre independientemente de los otro elementos de esa caja, pero solo dentro de esa caja y funciona con top or bottom, and left or right. Ver ejemplo, así funciona.


Cuando la posición de un elemento se establece a relative, te permite especificar como CSS lo moverá relativo a su posición actual dentro del flujo normal de la página. Se empareja con las propiedades de desplazamiento CSS de left o right, y top o bottom. Estas dicen cuántos pixeles, porcentajes, o ems se debe mover el elemento lejos de donde esté normalmente posicionado. El siguiente ejemplo mueve el párrafo 10 pixeles lejos de la parte inferior:

p {
  position: relative;
  bottom: 10px;
  top: 10px;
  left:10px;
  right:10px;
}
Cambiando la posición de un elemento a relative no lo quita del flujo normal; otros elementos a su alrededor aún se comportarán como si dicho elemento estuviera en su posición predeterminada.

Nota: el posicionamiento te da mucha flexibilidad y poder sobre el diseño visual de una página. Es bueno recordar que no importa la posición de los elementos, el lenguaje de marcado HTML subyacente debe organizarse y tener sentido cuando se lee de arriba a abajo. Así es como los usuarios con discapacidades visuales (que dependen de dispositivos de asistencia como lectores de pantalla) acceden a tu contenido.


/* posicion: te permite mover un elemento en relación a su contener. Puedes mover arriba, abajo, derecha e izquierda. Solo se va mover este elemento mientras que los otros dentro d ela caja van a mantener su posición original. Solo mueve el elemento al cual le asignas la posición relativa. el resto se queda. ///  Hay que entender que mueve en dirección hacia la dirección que se le indica*/

p {
  position: relative;
  top: 10px;
  left:10px;
}

/*Bloquea un elemento con relación a su padre con el posicionamiento absoluto. Position absoluta bloquea el elemento  en relación con su contenedor principal, o sea  solo el elemento de posicionamiento absoluto no se mueve mientras el resto de los elementos del contendor si lo hacen. Recuerda que los otros elementos lo ignoran y se va sobreponer otro elementos sobre este elemento */ 

/*La siguiente opción para la propiedad CSS position es absolute, que bloquea el elemento en su lugar en relación con su contenedor principal. A diferencia de la posición relative, esto elimina el elemento del flujo normal del documento, por lo que los elementos circundantes lo ignoran. Las propiedades de desplazamiento de CSS (superior o inferior e izquierda o derecha) se utilizan para ajustar la posición.

Un matiz del posicionamiento absoluto es que estará bloqueado en relación con su antepasado posicionado más cercano. Si olvidas agregar una regla de posición al elemento principal, (esto generalmente se hace usando position: relative;), el navegador seguirá buscando en la jerarquía de elementos y, en última instancia tomará por defecto la etiqueta body.*/


P{
position: absolute; 
right: 50px; 
top:50px;

}

/*Bloquea un elemento a la ventana del navegador con el posicionamiento fijo. */

/*El siguiente esquema de diseño que ofrece CSS es la posición fixed, que es un tipo de posicionamiento absoluto que bloquea un elemento relativo a la ventana del navegador. Similar al posicionamiento absoluto, se usa con las propiedades de desplazamiento CSS y también elimina el elemento del flujo normal del documento. Otros elementos ya no "se dan cuenta" de donde se coloca, lo que puede requerir algunos ajustes de diseño en otros lugares.

Una diferencia clave entre las posiciones fixed y absolute es que un elemento con una posición fija (fixed) no se moverá cuando el usuario se desplace.*/

#navbar {

position:fixed;
top:0px;
left:0px;
width: 100%;
background-color: #767676;
  }

  /*-Empuja elementos hacia la izquierda o hacia la derecha con la propiedad float. Los elementos flotantes se eliminan del flujo normal de un documento y se empujan a left o right de su elemento padre contenedor. Se usa comúnmente con la propiedad width para especificar cuanto espacio horizontal requiere el elemento flotante.-*/

  /*La siguiente herramienta de posicionamiento en realidad no usa position, sino que establece la propiedad float de un elemento. Los elementos flotantes se eliminan del flujo normal de un documento y se empujan a left o right de su elemento padre contenedor. Se usa comúnmente con la propiedad width para especificar cuanto espacio horizontal requiere el elemento flotante.*/

  #left {
    float: left;
          width: 50%;
        }
        
        #right {
    float: right;
          width: 40%;
        }



/*-Cambia la posición de los elementos superpuestos con la propiedad z-index. Cuando los elementos son posicionados para superponerse (i.e. usando position: absolute | relative | fixed | sticky), el elemento que viene después dentro del marcado HTML aparecerá, por defecto, encima de los otros elementos. Sin embargo, la propiedad z-index puede especificar el orden de cómo los elementos están apilados unos sobre otros.-*/

.first {
background-color: red;
position: absolute;
z-index: 2;/*más alto el index z sube más alto en la pila */
}

/*-Centra un elemento horizontalmente usando la propiedad margin. Otra técnica de posicionamiento consiste en centrar un elemento de bloque horizontalmente. Una manera de hacer esto es que margin tenga valor auto.

Este método también funciona para imágenes. Las imágenes son elementos en línea de forma predeterminada, pero se pueden cambiar a elementos de bloque cuando se establece la propiedad display en block.-*/

div {
background-color: blue;
height: 100px;
width: 100px;
margin: auto;
display: block; /* esto  hace que todo se desplace en bloque*/ /*no siempre se necesita */

}


/*Esto te permite construir cajas con color degrados: Recuerda que la dirección de la mezcla cambia en función a los grados que le pongas de 0 a 360. Puedes escoger la cantidad de colores que quieras. Coge cualquier tipo de input de color*/
div{
   
  width: 70%;
  height: 400px;
   background: repeating-linear-gradient(
    90deg,
    yellow 0px,
    blue 40px,
    green 40px,
    red 80px
  );
}
div{
  background: repeating-linear-gradient(
    0deg,
    yellow 0px,
    blue 40px,
    green 40px,
    red 80px
  );
}
div{
  background: linear-gradient(90deg, red, yellow, rgb(204, 204, 255));
}


/*Crea textura agregando un patrón sutil como imagen de fondo*/
/*Una forma de agregar textura e interés a un fondo y hacer que se destaque más es agregar un patrón sutil. La clave está en el balance, dado que no querrás que el fondo destaque demasiado y quite atención al primer plano. La propiedad background acepta la función url() para enlazar una imagen de la textura o patrón elegido. El enlace es cubierto entre comillas dentro del paréntesis. Puedes poner una foto o lo que quieras*/


  body {
background: url(https://cdn-media-1.freecodecamp.org/imgr/MJAkxbh.png);
  }


  /*Utiliza la propiedad de escala de transformación CSS para cambiar el tamaño de un elemento*/
/*Para cambiar la escala de un elemento, CSS tiene la propiedad transform, junto con su función scale(). En el ejemplo de código siguiente se duplica el tamaño de todos los elementos de párrafo de la página: Aplica a cualquier elemento*/
