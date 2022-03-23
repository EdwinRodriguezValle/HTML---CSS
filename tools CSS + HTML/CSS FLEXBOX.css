CSS FLEXBOX

Utiliza display: flex para posicionar dos cajas
/*Esta sección utiliza estilos de desafío alternos para mostrar cómo usar CSS para posicionar elementos de una manera flexible. En primer lugar, un desafío explicará la teoría, luego un desafío práctico utilizando un simple componente de tweet aplicará el concepto de flexbox.

Colocar la propiedad CSS display: flex; en un elemento te permite usar otras propiedades flex para construir una página responsiva.*/

<style>
  #box-container {
    height: 500px;
    display: flex; /*aquí el show. si no pones esto todo se pone en una columna*/ Fijate que pone al padre container.

  }

  #box-1 {
    background-color: dodgerblue;
    width: 50%;
    height: 50%;
  }

  #box-2 {
    background-color: orangered;
    width: 50%;
    height: 50%;
  }
</style>
<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>

----------------------------------------------------
Agrega superpoderes flex al tweet incrustado
/*A la derecha está el tweet incrustado que se utilizará como ejemplo práctico. Algunos de los elementos lucirían mejor con una disposición diferente. El último desafío demostró display: flex. Aquí la agregaras a varios componentes en el tweet incrustado para empezar a ajustar su posición.

Agrega la propiedad CSS display: flex a todos los siguientes elementos (ten en cuenta que los selectores ya están configurados en el CSS):

El encabezado header, el .profile-name del encabezado, el .follow-btn del encabezado, el h3 y h4 del encabezado, el footer, y el .stats del pie de página (footer).*/

display flex: te ayuda a mover como tu quieras dentro del contenedor.

<style>
  body {
    font-family: Arial, sans-serif;
  }
  header {
display: flex;
  }
  header .profile-thumbnail {
    width: 50px;
    height: 50px;
    border-radius: 4px;
  }
  header .profile-name {
    display: flex;

    margin-left: 10px;
  }
  header .follow-btn {
display: flex;
    margin: 0 0 0 auto;
  }
  header .follow-btn button {
    border: 0;
    border-radius: 3px;
    padding: 5px;
    
  }
  header h3, header h4 {
display: flex;
    margin: 0;
  }
  #inner p {
    margin-bottom: 10px;
    font-size: 20px;
  }
  #inner hr {
    margin: 20px 0;
    border-style: solid;
    opacity: 0.1;
  }
  footer {
display: flex
  }
  footer .stats {
display: flex;
    font-size: 15px;
  }
  footer .stats strong {
    font-size: 18px;
  }
  footer .stats .likes {
    margin-left: 10px;
  }
  footer .cta {
    margin-left: auto;
  }
  footer .cta button {
    border: 0;
    background: transparent;
  }
</style>
<header>
  <img src="https://freecodecamp.s3.amazonaws.com/quincy-twitter-photo.jpg" alt="Quincy Larson's profile picture" class="profile-thumbnail">
  <div class="profile-name">
    <h3>Quincy Larson</h3>
    <h4>@ossia</h4>
  </div>
  <div class="follow-btn">
    <button>Follow</button>
  </div>
</header>
<div id="inner">
  <p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>
  <span class="date">1:32 PM - 12 Jan 2018</span>
  <hr>
</div>
<footer>
  <div class="stats">
    <div class="Retweets">
      <strong>107</strong> Retweets
    </div>
    <div class="likes">
      <strong>431</strong> Likes
    </div>
  </div>
  <div class="cta">
    <button class="share-btn">Share</button>
    <button class="retweet-btn">Retweet</button>
    <button class="like-btn">Like</button>
  </div>
</footer>

--------------------------------------

Utiliza la propiedad flex-direction para hacer una fila
/*Agregando display: flex a un elemento lo convierte en un contenedor flexible. Esto permite alinear cualquier elemento secundario de ese elemento en filas o columnas. Para ello, agrega la propiedad flex-direction al elemento principal y configúralo en fila o columna. La creación de una fila alineara los elementos secundarios horizontalmente, y la creación de una columna alineara los elementos secundarios verticalmente.*/

h1{flex-direction: row} /*Esto puede ser*/

Otras opciones para flex-direction son row-reverse y column-reverse.*/

Nota: El valor predeterminado para la propiedad flex-direction es row.
<style>
  #box-container {
    display: flex;
    height: 500px;
    flex-direction:row-reverse; /*aquí el chiste cambia de posiciones> También puedes poner solo como filo o coluna */
    

  }
  #box-1 {
    background-color: dodgerblue;
    width: 50%;
    height: 50%;
  }

  #box-2 {
    background-color: orangered;
    width: 50%;
    height: 50%;
  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>

--------------------------------
Aplica la propiedad flex-direction para crear filas en el tweet Insertado
/*El header y footer en el ejemplo de tweet insertado tienen elementos secundarios que podrían organizarse como filas usando la propiedad flex-direction. Esto le dice a CSS que alinee los hijos horizontalmente.

Agrega la propiedad CSS flex-direction tanto al header como al footer y establece el valor en row.*/

pueden ir también juntos flex-direction y display:flex dentro de un mismo selector u elemento.

<style>
  body {
    font-family: Arial, sans-serif;
  }
  header {
    display: flex;
    flex-direction: row;

  }
  header .profile-thumbnail {
    width: 50px;
    height: 50px;
    border-radius: 4px;
  }
  header .profile-name {
    display: flex;
    margin-left: 10px;
  }
  header .follow-btn {
    display: flex;
    margin: 0 0 0 auto;
  }
  header .follow-btn button {
    border: 0;
    border-radius: 3px;
    padding: 5px;
  }
  header h3, header h4 {
    display: flex;
    margin: 0;
  }
  #inner p {
    margin-bottom: 10px;
    font-size: 20px;
  }
  #inner hr {
    margin: 20px 0;
    border-style: solid;
    opacity: 0.1;
  }
  footer {
    display: flex;
    flex-direction: row;

  }
  footer .stats {
    display: flex;
    font-size: 15px;
  }
  footer .stats strong {
    font-size: 18px;
  }
  footer .stats .likes {
    margin-left: 10px;
  }
  footer .cta {
    margin-left: auto;
  }
  footer .cta button {
    border: 0;
    background: transparent;
  }
</style>
<header>
  <img src="https://freecodecamp.s3.amazonaws.com/quincy-twitter-photo.jpg" alt="Quincy Larson's profile picture" class="profile-thumbnail">
  <div class="profile-name">
    <h3>Quincy Larson</h3>
    <h4>@ossia</h4>
  </div>
  <div class="follow-btn">
    <button>Follow</button>
  </div>
</header>
<div id="inner">
  <p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>
  <span class="date">1:32 PM - 12 Jan 2018</span>
  <hr>
</div>
<footer>
  <div class="stats">
    <div class="Retweets">
      <strong>107</strong> Retweets
    </div>
    <div class="likes">
      <strong>431</strong> Likes
    </div>
  </div>
  <div class="cta">
    <button class="share-btn">Share</button>
    <button class="retweet-btn">Retweet</button>
    <button class="like-btn">Like</button>
  </div>
</footer>


----------------------------------------------------------------
Utiliza la propiedad flex-direction para hacer una columna
/*Los dos últimos desafíos usaron la propiedad flex-direction establecida en row. Esta propiedad también puede crear una columna apilando verticalmente los hijos de un contenedor flex.*/

Agrega la propiedad CSS flex-direction al elemento #box-container y asígnale un valor de column.

<style>
  #box-container {
    display: flex;
    height: 500px;
    flex-direction:column; /*aquí el chiste*/

  }
  #box-1 {
    background-color: dodgerblue;
    width: 50%;
    height: 50%;
  }

  #box-2 {
    background-color: orangered;
    width: 50%;
    height: 50%;
  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>

-------------------------------------------------

Aplica la propiedad flex-direction para crear columnas en el tweet insertado
/*El header y footer del tweet insertado usaron previamente la propiedad flex-direction con un valor de fila. De manera similar, los elementos dentro del elemento .profile-name funcionarían bien apilados como una columna.

Agrega la propiedad CSS flex-direction al elemento .profile-name del título y establezca el valor en column.*/

<style>
  body {
    font-family: Arial, sans-serif;
  }
  header, footer {
    display: flex;
    flex-direction: row;
  }
  header .profile-thumbnail {
    width: 50px;
    height: 50px;
    border-radius: 4px;
  }
  header .profile-name {
    display: flex; /*funcionan juntos display:flex y flex-direction*/
    flex-direction: column;

    margin-left: 10px;
  }
  header .follow-btn {
    display: flex;
    margin: 0 0 0 auto;
  }
  header .follow-btn button {
    border: 0;
    border-radius: 3px;
    padding: 5px;
  }
  header h3, header h4 {
    display: flex;
    margin: 0;
  }
  #inner p {
    margin-bottom: 10px;
    font-size: 20px;
  }
  #inner hr {
    margin: 20px 0;
    border-style: solid;
    opacity: 0.1;
  }
  footer .stats {
    display: flex;
    font-size: 15px;
  }
  footer .stats strong {
    font-size: 18px;
  }
  footer .stats .likes {
    margin-left: 10px;
  }
  footer .cta {
    margin-left: auto;
  }
  footer .cta button {
    border: 0;
    background: transparent;
  }
</style>
<header>
  <img src="https://freecodecamp.s3.amazonaws.com/quincy-twitter-photo.jpg" alt="Quincy Larson's profile picture" class="profile-thumbnail">
  <div class="profile-name">
    <h3>Quincy Larson</h3>
    <h4>@ossia</h4>
  </div>
  <div class="follow-btn">
    <button>Follow</button>
  </div>
</header>
<div id="inner">
  <p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>
  <span class="date">1:32 PM - 12 Jan 2018</span>
  <hr>
</div>
<footer>
  <div class="stats">
    <div class="Retweets">
      <strong>107</strong> Retweets
    </div>
    <div class="likes">
      <strong>431</strong> Likes
    </div>
  </div>
  <div class="cta">
    <button class="share-btn">Share</button>
    <button class="retweet-btn">Retweet</button>
    <button class="like-btn">Like</button>
  </div>
</footer>


-------------------------------------------------------------------------------
Alinea elementos mediante la propiedad justify-content
/*Algunas veces los elementos flexibles dentro de un contenedor flexible no llenan todo el espacio del contenedor. Es común querer indicarle al CSS cómo alinear y espaciar los elementos flexibles de una determinada manera. Afortunadamente, la propiedad justify-content tiene varias opciones para hacer esto. Pero primero, hay que entender alguna terminología importante antes de revisar dichas opciones.

Aquí hay una imagen útil que muestra una fila para ilustrar los conceptos siguientes.

Recuerda que establecer un contenedor flexible como fila coloca los elementos flexibles uno al lado del otro de izquierda a derecha. Un contenedor flexible establecido como columna coloca los elementos flexibles apilados verticalmente de arriba a abajo. Para cada uno, la dirección en la que están dispuestos los elementos flexibles se llama el eje principal. Para una fila, esta es una línea horizontal que recorta cada elemento. Y para una columna, el eje principal es una línea vertical a través de los elementos.

Hay varias opciones para espaciar los elementos flexibles a lo largo de la línea que representa el eje principal. Uno de los más utilizados es justify-content: center;, el cual alinea hacia el centro todos los elementos flexibles dentro del contenedor flexible. Otras opciones incluyen:*/

flex-start: /*alinea los elementos con el inicio del contenedor flex. Para una fila, esto empuja los elementos a la izquierda del contenedor. Para una columna, esto empuja los elementos a la parte superior del contenedor. Esta es la alineación predeterminada si no se especifica ningún tipo de justify-content.*/
flex-end: /*alinea los elementos con el final del contenedor flex. Para una fila, esto empuja los elementos a la derecha del contenedor. Para una columna, esto empuja los elementos a la parte inferior del contenedor.*/
space-between: /*alinea los elementos en el centro del eje principal, con un espacio extra entre los elementos. Los primeros y últimos elementos son empujados hasta el borde del contenedor flexible. Por ejemplo, en una fila el primer elemento está en el lado izquierdo del contenedor, el último elemento está en el lado derecho del contenedor, luego el espacio restante se distribuye uniformemente entre los demás elementos.*/
space-around: /*similar a space-between pero los primeros y últimos elementos no están fijados en los bordes del contenedor, el espacio se distribuye alrededor de todos los elementos con la mitad de un espacio en ambos extremos del contenedor flexible.*/
space-evenly: /*Distribuye el espacio de manera uniforme entre los elementos flexibles con un espacio completo en ambos extremos del contenedor flexible
Un ejemplo ayuda a mostrar esta propiedad en acción. Agrega la propiedad CSS justify-content al elemento #box-container y asígnale un valor de*/
center.*/


<style>
  #box-container {
    background: gray;
    display: flex;
    height: 500px;
    justify-content: center; /*aquí como funciona, solo hay que cambiar center por los otros para ue hagan lo que tienen que hacer */

  }
  #box-1 {
    background-color: dodgerblue;
    width: 25%;
    height: 100%;
  }

  #box-2 {
    background-color: orangered;
    width: 25%;
    height: 100%;
  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>


---------------------------------------------------------------------------------------------------

Utiliza la propiedad justify-content en el tweet Insertado
/*El último desafío mostró un ejemplo de la propiedad justify-content. Para el tweet insertado, esta propiedad se puede aplicar para alinear los elementos en el .profile-name.*/
<style>
  body {
    font-family: Arial, sans-serif;
  }
  header, footer {
    display: flex;
    flex-direction: row;
  }
  header .profile-thumbnail {
    width: 50px;
    height: 50px;
    border-radius: 4px;
  }
  header .profile-name {
    display: flex;
    flex-direction: column;
    justify-content: space-around; /*aquí el chiste*/

    margin-left: 10px;
  }
  header .follow-btn {
    display: flex;
    margin: 0 0 0 auto;
  }
  header .follow-btn button {
    border: 0;
    border-radius: 3px;
    padding: 5px;
  }
  header h3, header h4 {
    display: flex;
    margin: 0;
  }
  #inner p {
    margin-bottom: 10px;
    font-size: 20px;
  }
  #inner hr {
    margin: 20px 0;
    border-style: solid;
    opacity: 0.1;
  }
  footer .stats {
    display: flex;
    font-size: 15px;
  }
  footer .stats strong {
    font-size: 18px;
  }
  footer .stats .likes {
    margin-left: 10px;
  }
  footer .cta {
    margin-left: auto;
  }
  footer .cta button {
    border: 0;
    background: transparent;
  }
</style>
<header>
  <img src="https://freecodecamp.s3.amazonaws.com/quincy-twitter-photo.jpg" alt="Quincy Larson's profile picture" class="profile-thumbnail">
  <div class="profile-name">
    <h3>Quincy Larson</h3>
    <h4>@ossia</h4>
  </div>
  <div class="follow-btn">
    <button>Follow</button>
  </div>
</header>
<div id="inner">
  <p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>
  <span class="date">1:32 PM - 12 Jan 2018</span>
  <hr>
</div>
<footer>
  <div class="stats">
    <div class="Retweets">
      <strong>107</strong> Retweets
    </div>
    <div class="likes">
      <strong>431</strong> Likes
    </div>
  </div>
  <div class="cta">
    <button class="share-btn">Share</button>
    <button class="retweet-btn">Retweet</button>
    <button class="like-btn">Like</button>
  </div>
</footer>

--------------------------------------------------------------------------------------------------------------
Alinea elementos mediante la propiedad align-items
/*La propiedad align-items es similar a justify-content. Recuerda que la propiedad justify-content alineó los elementos flexibles a lo largo del eje principal. Para las filas, el eje principal es una línea horizontal y para las columnas es una vertical.

Los contenedores flexibles también tienen un eje transversal que es el opuesto al eje principal. Para las filas, el eje transversal es vertical y para las columnas, el eje transversal es horizontal.

CSS ofrece la propiedad align-items para alinear elementos flexibles a lo largo del eje transversal. Para una fila, le indica al CSS como empujar los elementos en toda la fila hacia arriba o hacia abajo dentro del contenedor. Y para una columna, como empujar todos los elementos hacia la izquierda o hacia la derecha dentro del contenedor.

Los diferentes valores disponibles para align-items incluyen:*/

flex-start: /*alinea los elementos con el inicio del contenedor flexible. Para las filas, esto alinea los elementos a la parte superior del contenedor. Para las columnas, esto alinea los elementos a la parte izquierda del contenedor.*/
flex-end: /*alinea los elementos con el final del contenedor flexible. Para las filas, esto alinea los elementos a la parte inferior del contenedor. Para las columnas, esto alinea los elementos a la parte derecha del contenedor.*/
center: /*alinea los elementos hacia el centro. Para las filas, esto alinea los elementos verticalmente (igual espacio por encima y por debajo de los elementos). Para columnas, esto las alinea horizontalmente (igual espacio a la izquierda y a la derecha de los elementos).*/
stretch: /*estira los elementos para llenar el contenedor flexible. Por ejemplo, los elementos de filas son estirados para llenar el contenedor flexible de arriba hacia abajo. Este es el valor predeterminado si no se especifica ningún tipo de align-items.*/
baseline: /*alinea los elementos con sus líneas base. Una línea base es un concepto de texto, piensa en ella como la línea en la que se sitúan las letras.*/
Un ejemplo ayuda a mostrar esta propiedad en acción. Agrega la propiedad CSS align-items al elemento #box-container y asígnale un valor de center.

Extra
Prueba las otras opciones de la propiedad align-items en el editor de código para ver sus diferencias. Pero ten en cuenta que un valor de center es el único que superará este desafío.

<style>
  #box-container {
    background: gray;
    display: flex;
    height: 500px;
    align-items:center; /*aquí el show* Alina en el eje horizontal minetras que justify-content en el eje vertical*/

  }
  #box-1 {
    background-color: dodgerblue;
    width: 200px;
    font-size: 24px;
  }

  #box-2 {
    background-color: orangered;
    width: 200px;
    font-size: 18px;
  }
</style>

<div id="box-container">
  <div id="box-1"><p>Hello</p></div>
  <div id="box-2"><p>Goodbye</p></div>
</div>

-------------------------------------------------------------------------------------------------------------
Utiliza la propiedad align-items en el tweet insertado
/*El último desafío introdujo la propiedad align-items y dio un ejemplo. Esta propiedad se puede aplicar a unos cuantos elementos del tweet insertado para alinear los elementos flexibles dentro de ellos.*/

<style>
  body {
    font-family: Arial, sans-serif;
  }
  header, footer {
    display: flex;
    flex-direction: row;
  }
  header .profile-thumbnail {
    width: 50px;
    height: 50px;
    border-radius: 4px;
  }
  header .profile-name {
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-left: 10px;
  }
  header .follow-btn {
    display: flex;
    align-items:center; /* aquí el show*/

    margin: 0 0 0 auto;
  }
  header .follow-btn button {
    border: 0;
    border-radius: 3px;
    padding: 5px;
  }
  header h3, header h4 {
    display: flex;
    margin: 0;
  }
  #inner p {
    margin-bottom: 10px;
    font-size: 20px;
  }
  #inner hr {
    margin: 20px 0;
    border-style: solid;
    opacity: 0.1;
  }
  footer .stats {
    display: flex;
    font-size: 15px;
  }
  footer .stats strong {
    font-size: 18px;
  }
  footer .stats .likes {
    margin-left: 10px;
  }
  footer .cta {
    margin-left: auto;
  }
  footer .cta button {
    border: 0;
    background: transparent;
  }
</style>
<header>
  <img src="https://freecodecamp.s3.amazonaws.com/quincy-twitter-photo.jpg" alt="Quincy Larson's profile picture" class="profile-thumbnail">
  <div class="profile-name">
    <h3>Quincy Larson</h3>
    <h4>@ossia</h4>
  </div>
  <div class="follow-btn">
    <button>Follow</button>
  </div>
</header>
<div id="inner">
  <p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>
  <span class="date">1:32 PM - 12 Jan 2018</span>
  <hr>
</div>
<footer>
  <div class="stats">
    <div class="Retweets">
      <strong>107</strong> Retweets
    </div>
    <div class="likes">
      <strong>431</strong> Likes
    </div>
  </div>
  <div class="cta">
    <button class="share-btn">Share</button>
    <button class="retweet-btn">Retweet</button>
    <button class="like-btn">Like</button>
  </div>
</footer>



-------------------------------------------------------------------------------------------------------

Usa la propiedad flex-wrap para envolver una fila o columna
/*CSS flexbox tiene una característica para dividir un elemento flexible en varias filas (o columnas). De forma predeterminada, un contenedor flexible encajará todos los elementos flexibles juntos. Por ejemplo, una fila estará completa en una sola línea.

Sin embargo, usar la propiedad flex-wrap le indica al CSS que envuelva los elementos. Esto significa que los elementos extra se mueven hacia una nueva fila o columna. El punto de ruptura donde ocurre la envoltura depende del tamaño de los elementos y del tamaño del contenedor.

CSS también tiene opciones para la dirección de la envoltura:*/

nowrap: /*esta es la configuración predeterminada, y no envuelve elementos.*/
wrap: /*envuelve elementos en múltiples líneas de arriba a abajo si están en filas y de izquierda a derecha si están en columnas.*/
wrap-reverse: /*envuelve elementos en múltiples líneas de abajo hacia arriba si están en filas y de derecha a izquierda si están en columnas.*/

<style>
  #box-container {
    background: gray;
    display: flex;
    height: 100%;
    flex-wrap:wrap;

  }
  #box-1 {
    background-color: dodgerblue;
    width: 25%;
    height: 50%;
  }

  #box-2 {
    background-color: orangered;
    width: 25%;
    height: 50%;
  }
  #box-3 {
    background-color: violet;
    width: 25%;
    height: 50%;
  }
  #box-4 {
    background-color: yellow;
    width: 25%;
    height: 50%;
  }
  #box-5 {
    background-color: green;
    width: 25%;
    height: 50%;
  }
  #box-6 {
    background-color: black;
    width: 25%;
    height: 50%;
  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
  <div id="box-3"></div>
  <div id="box-4"></div>
  <div id="box-5"></div>
  <div id="box-6"></div>
</div>



-------------------------------------------------------------------------------------------------------------
Utiliza la propiedad flex-shrink para reducir elementos
/*Hasta ahora, todas las propiedades en los desafíos se aplican al contenedor flexible (el padre de los elementos flex). Sin embargo, hay varias propiedades útiles para los elementos flex.

La primera es la propiedad flex-shrink. Cuando se usa, permite que un elemento se contraiga si el contenedor flex es demasiado pequeño. Los elementos se reducen cuando el ancho del contenedor principal es menor que el ancho combinado de todos los elementos flex dentro del él.

La propiedad flex-shrink toma números como valores. Cuando mayor sea el número, más se reducirá en comparación con los otros elementos en el contenedor. */Por ejemplo, si un elemento tiene un flex-shrink con valor de 1 y el otro tiene un flex-shrink con valor de 3, el que tiene el valor de 3 se reducirá tres veces más que el otro.

El que tiene menos valor en números más alto se reduce las veces que ese numero indica

<style>
  #box-container {
    display: flex;
    height: 500px;
    
  }
  #box-1 {
    background-color: dodgerblue;
    width: 100%;
    height: 200px;
    flex-shrink:1; /*aquí el chiste*/

  }

  #box-2 {
    background-color: orangered;
    width: 100%;
    height: 200px;
    flex-shrink:2; /*aquí el chiste*/

  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>

-----------------------------------------------
Use the flex-grow Property to Expand Items
/*The opposite of flex-shrink is the flex-grow property. Recall that flex-shrink controls the size of the items when the container shrinks. The flex-grow property controls the size of items when the parent container expands.

Using a similar example from the last challenge, if one item has a flex-grow value of 1 and the other has a flex-grow value of 3, the one with the value of 3 will grow three times as much as the other.*/

<style>
  #box-container {
    display: flex;
    height: 500px;
  }

  #box-1 {
    background-color: dodgerblue;
    height: 200px;
    flex-grow:1; /*aquí el chiste*/

  }

  #box-2 {
    background-color: orangered;
    height: 200px;
    flex-grow:2;  /*Aquí el chiste*/

  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>


------------------------------------------

Use the flex-basis Property to Set the Initial Size of an Item
/*The flex-basis property specifies the initial size of the item before CSS makes adjustments with flex-shrink or flex-grow.

The units used by the flex-basis property are the same as other size properties (px, em, %, etc.). The value auto sizes items based on the content.

Set the initial size of the boxes using flex-basis. Add the CSS property flex-basis to both #box-1 and #box-2. Give #box-1 a value of 10em and #box-2 a value of 20em.*/

<style>
  #box-container {
    display: flex;
    height: 500px;
  }

  #box-1 {
    background-color: dodgerblue;
    height: 200px;
    flex-basis: 10em;/*aquí el chiste de la historia */

  }

  #box-2 {
    background-color: orangered;
    height: 200px;
    flex-basis:20em; /*aquí el chiste de la historia */

  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>

-------------------------

Usa la propiedad abreviada FLEX
/*Hay un atajo disponible para establecer varias propiedades flex a la vez. Las propiedades flex-grow, flex-shrink, y flex-basis pueden establecerse utilizando la propiedad flex.

Por ejemplo, flex: 1 0 10px; establecerá las propiedades del elemento en flex-grow: 1;, flex-shrink: 0;, y flex-basis: 10px;.

La configuración predeterminada de la propiedad es flex: 0 1 auto;.

Agrega la propiedad CSS flex tanto a #box-1 como a #box-2. Dale a #box-1 los valores para que su flex-grow sea 2, su flex-shrink sea 2, y su flex-basis sea 150px. Dale a #box-2 los valores para que su flex-grow sea 1, su flex-shrink sea 1, y su flex-basis sea 150px.

Estos valores causarán que para llenar el espacio extra #box-1 crezca el doble de #box-2 cuando el contenedor sea mayor que 300px y se reduzca al doble de #box-2 cuando el contenedor sea menor de 300px. 300px es el tamaño combinado de los valores de flex-basis de las dos cajas.*/


<style>
  #box-container {
    display: flex;
    height: 500px;
  }
  #box-1 {
    background-color: dodgerblue;
    flex:2 2 150px;/*aquí el chiste*/

    height: 200px;
  }

  #box-2 {
    background-color: orangered;
    flex: 1 1 150px;/*aquí el chiste*/

    height: 200px;
  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>


------------------------------------------------------
Usa la propiedad ORDER para reorganizar los elementos
/*La propiedad order se utiliza para indicarle a CSS el orden en que aparecen los elementos flexibles en el contenedor flex. Por defecto, los elementos aparecerán en el mismo orden que vienen en el HTML de origen. La propiedad toma números como valores, y se pueden usar números negativos.*/

<style>
  #box-container {
    display: flex;
    height: 500px;
  }
  #box-1 {
    background-color: dodgerblue;
    order:2;/*aquí el chiste*/


    height: 200px;
    width: 200px;
  }

  #box-2 {
    background-color: orangered;
    order:1; /*Aquí el chiste*/

    height: 200px;
    width: 200px;
  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>

-------------------------------------------------------------------

Usa la propiedad align-self

/*La última propiedad para elementos flexibles es align-self. Esta propiedad te permite ajustar la alineación de cada elemento individualmente, en lugar de ajustarlos todos a la vez. Esto es útil ya que otras técnicas comunes de ajuste usan las propiedades */ CSS float, clear, y vertical-align, las cuales no funcionan en elementos flexibles.

align-self acepta los mismos valores que align-items y reemplazará cualquier valor establecido por la propiedad align-items. 

<style>
  #box-container {
    display: flex;
    height: 500px;
  }
  #box-1 {
    background-color: dodgerblue;
    align-self: center;

    height: 200px;
    width: 200px;
  }

  #box-2 {
    background-color: orangered;
    align-self:flex-end;

    height: 200px;
    width: 200px;
  }
</style>

<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>