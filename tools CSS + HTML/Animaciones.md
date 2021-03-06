/*ANIMACIONES EN CSS*/
  
  
  /*Utiliza la propiedad de escala de transformación CSS para cambiar el tamaño de un elemento*/
/*Para cambiar la escala de un elemento, CSS tiene la propiedad transform, junto con su función scale(). En el ejemplo de código siguiente se duplica el tamaño de todos los elementos de párrafo de la página: Aplica a cualquier elemento*/

p {
    transform: scale(2);
  }
  
  /*Utiliza la propiedad de escala de transformación CSS para escalar un elemento al desplazarse*/
  /*La propiedad transform tiene una variedad de funciones que el permiten escalar, mover, rotar, sesgar, etc., sus elementos. Cuando se usa con pseudo-classes como :hover que especifican un cierto estado de un elemento, la propiedad transform puede agregar fácilmente interactividad a sus elementos.*/
  
  Aquí hay un ejemplo para escalar los elementos de párrafo a 2.1 veces su tamaño original:
  
  p:hover {
    transform: scale(2.1);
  }
  
  div:hover{
    transform:scale(1.1);
  }
  
  a:hover{
    transform:scale(1.1);
  }
  /*Nota: La aplicación de una transformación a un elemento div también afectará a cualquier elemento secundario contenido del div.*/
  
  
  /*Utiliza la propiedad de transformación CSS skewX para inclinar un elemento a lo largo del eje X*/
  /*La siguiente función de la propiedad transform es skewX(), que inclinar el elemento seleccionado a lo largo de su eje X (horizontal).
  
  El siguiente código inclina el elemento de párrafo en -32 grados a lo largo del eje X.*/
  
  p {
    transform: skewX(-32deg);
  }
  
  #bottom {
    background-color: blue;
    transform: skewX(24deg);
  }
  
  /*Utiliza la propiedad de transformación CSS skewY para inclinar un elemento a lo largo del eje Y*/
  /* la propiedad skewY() incline un elemento a lo largo del eje Y (vertical).*/
  #top{
    transform: skewY(-10deg);
  }
  
  
  /*Crea un gráfico usando CSS*/
  Al manipular diferentes selectores y propiedades, puedes hacer figuras interesantes. Una de las figuras más fáciles de intentar es la luna creciente. Para este desafío necesitas trabajar con la propiedad box-shadow que aplica la sombra de un elemento, junto con la propiedad border-radius que controla la redondez de las esquinas del elemento.
  
  Crearás un objeto redondo y transparente con una sombra nítida que está ligeramente desplazada hacia un lado - la sombra en realidad va a ser la figura de luna que verás.
  
  Para crear un objeto redondo, la propiedad border-radius se le debe asignar un valor de 50%.
  
  Puede que recuerdes de un desafío anterior que la propiedad box-shadow toma valores para offset-x, offset-y, blur-radius, spread-radius y un valor para el color, en ese orden. Los valores blur-radius y spread-radius son opcionales.
  
  Manipula el elemento cuadrado en el editor para crear la figura de luna. Primero, cambia el background-color a transparent, luego establece la propiedad border-radius en 50% para hacer la forma circular. Finalmente, cambia la propiedad box-shadow para asignar offset-x a 25px, offset-y a 10px, blur-radius a 0, spread-radius a 0 y el color a blue.
  
  .center {
    position: absolute;
    margin: auto;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    width: 100px;
    height: 100px;
    background-color: transparent;
    border-radius: 50px;
    box-shadow: 10px 10px 0px 0px green;
  }
  
  
  /*Crea una forma más compleja usando CSS y HTML*/
  /*Una de las formas más populares en el mundo es la forma del corazón, y en este desafío crearás una usando CSS puro. Pero primero, debes comprender los pseudo-elements ::before y ::after. ::before crea un pseudo-elemento que es el primer hijo del elemento seleccionado; ::after crea un pseudo-elemento que es el último hijo del elemento seleccionado. En el siguiente ejemplo, se utiliza un pseudo-elemento ::before para agregar un rectángulo a un elemento con la clase heart:*/
  
  .heart::before {
    content: "";
    background-color: yellow;
    border-radius: 25%;
    position: absolute;
    height: 50px;
    width: 70px;
    top: -50px;
    left: 5px;
  }
  Para que los pseudo-elements ::before y ::after funcionen correctamente, deben tener una propiedad content definida. Esta propiedad generalmente se usa para agregar cosas como una foto o texto al elemento seleccionado. Cuando se utilizan los pseudo-elements ::before y ::after para crear formas, la propiedad content sigue siendo necesaria, pero se establece en una cadena vacía. En el ejemplo anterior, el elemento con la clase de heart tiene un pseudo-element ::before que produce un rectángulo amarillo con una altura y un ancho de 50px y 70px, respectivamente. Este rectángulo tiene esquinas redondeadas debido a su 25% border-radius y está posicionado absolutamente a 5px desde la izquierda y 50px por encima de la parte superior del elemento.
  
  Transforma el elemento en la pantalla en un corazón. En el selector heart::after, cambia background-color a pink y border-radius a 50%.
  
  A continuación, apunta el elemento con la clase heart (solo heart) y llena la propiedad transform. Utiliza la función rotate() con -45 grados.
  
  Finalmente, en el selector heart::before, establece su propiedad content en una cadena vacía.
  
  <style>
    .heart {
      position: absolute;
      margin: auto;
      top: 0;
      right: 0;
      bottom: 0;
      left: 0;
      background-color: pink;
      height: 50px;
      width: 50px;
      transform: rotate(-45deg) ;
    }
    .heart::after {
      background-color: pink;
      content: "";
      border-radius: 50%;
      position: absolute;
      width: 50px;
      height: 50px;
      top: 0px;
      left: 25px;
    }
    .heart::before {
      content:"" ;
      background-color: pink;
      border-radius: 50%;
      position: absolute;
      width: 50px;
      height: 50px;
      top: -25px;
      left: 0px;
    }
  </style>
  <div class="heart"> </div>
  
  
  /*Aprende como funcionan las propiedades de CSS @keyframes y animación*/
  /*Para animar un elemento, necesitas conocer las propiedades de animación y la regla @keyframes. Las propiedades de animación controlan como debe comportarse la animación y la regla @keyframes controla lo que sucede durante esa animación. Hay ocho propiedades de animación en total. Este desafío lo mantendrá simple y cubrirá primero los dos más importantes:
  
  animation-name establece el nombre de la animación, que luego es utilizada por @keyframes para decirle a CSS que reglas van con que animaciones.
  
  animation-duration establece el tiempo de la animación.
  
  @keyframes es como especificar exactamente lo que sucede dentro de la animación durante la duración. Esto se hace dando propiedades CSS para "marcos" específicos durante la animación, con porcentajes que van del 0% al 100%. Si comparas esto con una película, las propiedades de CSS de 0% es como se muestra el elemento en la escena inicial. Las propiedades de CSS con 100% es como aparece el elemento al final, justo antes de que rueden los créditos. Luego, CSS aplica la magia para hacer la transición del elemento durante la duración dada para representar la escena. Aquí hay un ejemplo para ilustrar el uso de @keyframes y las propiedades de animación:*/
  
  #anim {
    animation-name: colorful;
    animation-duration: 3s;
  }
  
  @keyframes colorful {
    0% {
      background-color: blue;
    }
    100% {
      background-color: yellow;
    }
  }
  /*Para el elemento anim id, el fragmento de codigo anterior establece el animation-name para colorful y establece el animation-duration a 3 segundos. A continuación, la regla @keyframes vincula a las propiedades de animación con el nombre colorful. Establece el color en azul al principio de la animación (0%) que pasara a amarillo al final de la animación (100%). No estás limitado solo a las transiciones de principio a fin, puedes establecer propiedades para el elemento para cualquier porcentaje entre 0% y 100%.
  
  Crea una animación para el elemento con el id rect, estableciendo animation-name en rainbow y animation-duration a 4 segundos. A continuación, declara una regla @keyframes y estableca el background-color al principio de la animación (0%) en azul, el centro de la animación (50%) en verde y el final de la animación (100%) en amarillo.*/
  
  <style>
    div {
      height: 40px;
      width: 70%;
      background: black;
      margin: 50px auto;
      border-radius: 5px;
    }
  
    #rect {
      animation-name: rainbow;
      animation-duration: 4s;
    }
  
    @keyframes rainbow {
      0% {
        background-color: blue;
      }
      50% {
        background-color: green;
      }
      100% {
        background-color: yellow;
      }
    }
  
  </style>
  <div id="rect"></div>
  
  /*Usa animación CSS para cambiar el estado del desplazamiento de un botón*/
  /*Puedes usar CSS @keyframes para cambiar el color de un botón en su estado de desplazamiento.
  
  Aquí hay un ejemplo de como cambiar el ancho de una imagen al pasar sobre ella:*/
  
  <style>
    img {
      width: 30px;
    }
    img:hover {
      animation-name: width;
      animation-duration: 500ms;
    }
  
    @keyframes width {
      100% {
        width: 40px;
      }
    }
  </style>
  
  /*<img src="https://cdn.freecodecamp.org/curriculum/applied-visual-design/google-logo.png" alt="Google's Logo" />
  Ten en cuenta que ms significa milisegundos, donde 1000ms es igual a 1s.
  
  Utiliza CSS @keyframes para cambiar el background-color del elemento button para que se convierta en #4791d0 cuando un usuario pase sobre él. La regla @keyframes solo debe tener una entrada para 100%.*/
  
  <style>
    button {
      border-radius: 5px;
      color: white;
      background-color: #0F5897;
      padding: 5px 10px 8px 10px;
    }
  
    button:hover {
      animation-name: background-color;
      animation-duration: 500ms;
    }
    @keyframes background-color {
      100%{
        background-color:#4791d0;
      }
    }
  
  </style>
  
  <button>Register</button>
  
  /*Modifica el modo de relleno de una animación (animation-fill-mode)*/
  /*Eso es genial, pero aún no funciona bien. Observa como la animación se restablece después de que haya pasado 500ms, haciendo que el botón vuelva al color original. Lo que quieres es que el botón permanezca resaltado.
  
  Esto se puede hacer estableciendo la propiedad animation-fill-mode en forwards. El animation-fill-mode especifica el estilo aplicado a un elemento cuando la animación ha finalizado. Puedes configurarlo así:*/
  
  animation-fill-mode: forwards;
  
  <style>
    button {
      border-radius: 5px;
      color: white;
      background-color: #0F5897;
      padding: 5px 10px 8px 10px;
    }
    button:hover {
      animation-name: background-color;
      animation-duration: 500ms;
      /* Cambia solo el código debajo de esta línea */
  animation-fill-mode: forwards;
      /* Cambia solo el código encima de esta línea */
    }
    @keyframes background-color {
      100% {
        background-color: #4791d0;
      }
    }
  </style>
  <button>Register</button>
  
  
  /*Crear movimiento usando animación CSS*/
  /*Cuando los elementos tienen una position, como fixed o relative, las propiedades de desplazamiento CSS right, left, top y bottom se pueden usar en las reglas de animación para crear movimiento.
  
  Como se muestra en el siguiente ejemplo, puedes empujar el elemento hacia abajo y luego hacia arriba estableciendo la propiedad top fotograma clave (keyframe) a 50% en 50px, pero estableciéndolo en 0px para el primer fotograma clave (0%) y el último a (100%).*/
  
  @keyframes rainbow {
    0% {
      background-color: blue;
      top: 0px;
    }
    50% {
      background-color: green;
      top: 50px;
    }
    100% {
      background-color: yellow;
      top: 0px;
    }
  }
  
  /*Agrega un movimiento horizontal a la animación div. Usando la propiedad desplazamiento left, agrega a la regla @keyframes para que el arcoíris (rainbow) comience en 0 píxeles en 0%, se mueva a 25 píxeles en 50%, y termine en -25 píxeles en 100%. No reemplaces la propiedad top en el editor; la animación debe tener movimiento vertical y horizontal.*/
  
  <style>
    div {
      height: 40px;
      width: 70%;
      background: black;
      margin: 50px auto;
      border-radius: 5px;
      position: relative;
    }
  
    #rect {
      animation-name: rainbow;
      animation-duration: 4s;
    }
  
    @keyframes rainbow {
      0% {
        background-color: blue;
        left: 0px;
  
      }
      50% {
        background-color: green;
        left: 25px;
  
      }
      100% {
        background-color: yellow;
        left: -25px;
  
      }
    }
  </style>
  
  <div id="rect"></div>
  
  /*Crear dirección visual desvaneciendo un elemento de izquierda a derecha*/
  /*Para este desafío, cambiarás la opacidad (opacity) de un elemento animado para que se desvanezca gradualmente a medida que llega al lado derecho de la pantalla.
  
  En la animación mostrada, el elemento redondo con el fondo degradado se mueve hacia la derecha con la marca del 50% de la animación según la regla @keyframes.
  
  Apunta al elemento con el id de ball y agrega la propiedad opacity establecida en 0.1 en 50%, de modo que el elemento se desvanezca a medida que se mueve hacia la derecha.*/
  
  <style>
  
    #ball {
      width: 70px;
      height: 70px;
      margin: 50px auto;
      position: fixed;
      left: 20%;
      border-radius: 50%;
      background: linear-gradient(
        35deg,
        #ccffff,
        #ffcccc
      );
      animation-name: fade;
      animation-duration: 3s;
    }
  
    @keyframes fade {
      50% {
        left: 60%;
        opacity: 0.1;
      }
    }
    }
  
  </style>
  
  <div id="ball"></div>
  
  /*Animar los elementos continuamente utilizando un contador de animaciones infinitas*/
  /*En los desafíos anteriores, vimos cómo utilizar algunas de las propiedades de la animación y la regla @keyframes. Otra propiedad de animación es la animation-iteration-count la cual te permite controlar cuántas veces te gustaría hacer un bucle a través de la animación. Por ejemplo:
  
  animation-iteration-count: 3;
  En este caso, la animación se detendrá después de ejecutarse 3 veces, pero es posible hacer que la animación se ejecute continuamente estableciendo ese valor en infinite.
  
  Para mantener la bola rebotando a la derecha en un bucle continuo, cambia la propiedad animation-iteration-count a infinite.*/
  
  <style>
  
    #ball {
      width: 100px;
      height: 100px;
      margin: 50px auto;
      position: relative;
      border-radius: 50%;
      background: linear-gradient(
        35deg,
        #ccffff,
        #ffcccc
      );
      animation-name: bounce;
      animation-duration: 1s;
      animation-iteration-count: infinite;/*esto controla la veces de la animación */
    }
  
    @keyframes bounce{
      0% {
        top: 0px;
      }
      50% {
        top: 249px;
        width: 130px;
        height: 70px;
      }
      100% {
        top: 0px;
      }
       
    }
  </style>
  <div id="ball"></div>
  
  
  /*Haz latir un corazón con CSS usando un recuento de animación infinita*/
  /*Aquí hay un ejemplo más de animación con la propiedad animation-iteration-count que usa el corazón que diseñaste en un desafío anterior.
  
  La animación del latido de un segundo consta de dos piezas animadas. Los elementos heart (incluyendo las piezas :before y :after) se animan para cambiar el tamaño usando la propiedad transform, y el fondo div se anima para cambiar su color usando la propiedad background.
  
  Mantén el corazón latiendo agregando la propiedad animation-iteration-count tanto para la clase back como para la clase heart y estableciendo el valor en infinite. Los selectores heart:before y heart:after no necesitan ninguna propiedad de animación.*/
  
  <style>
    .back {
      position: fixed;
      padding: 0;
      margin: 0;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: white;
      animation-name: backdiv;
      animation-duration: 1s;
      animation-iteration-count: infinite;
      
  
    }
  
    .heart {
      position: absolute;
      margin: auto;
      top: 0;
      right: 0;
      bottom: 0;
      left: 0;
      background-color: pink;
      height: 50px;
      width: 50px;
      transform: rotate(-45deg);
      animation-name: beat;
      animation-duration: 1s;
      animation-iteration-count: infinite;
  
    }
    .heart:after {
      background-color: pink;
      content: "";
      border-radius: 50%;
      position: absolute;
      width: 50px;
      height: 50px;
      top: 0px;
      left: 25px;
    }
    .heart:before {
      background-color: pink;
      content: "";
      border-radius: 50%;
      position: absolute;
      width: 50px;
      height: 50px;
      top: -25px;
      left: 0px;
    }
  
    @keyframes backdiv {
      50% {
        background: #ffe6f2;
      }
    }
  
    @keyframes beat {
      0% {
        transform: scale(1) rotate(-45deg);
      }
      50% {
        transform: scale(0.6) rotate(-45deg);
      }
    }
  
  </style>
  <div class="back"></div>
  <div class="heart"></div>
  
  /*Elementos animados con fluctuaciones*/
  /*Hay muchas formas de alterar la cantidad de animaciones de elementos similares con animaciones. Hasta ahora, esto se ha logrado al aplicar una propiedad animation-iteration-count y estableciendo reglas @keyframes.
  
  A modo de ilustración, la animación de la derecha consta de dos estrellas, cada una de las cuales disminuye en tamaño y opacidad en la marca del 20% en la regla @keyframes, que crea la animación centelleante. Puede cambiar la regla @keyframes para uno de los elementos, así las estrellas titilan con diferentes ritmos.
  
  Cambia la velocidad de animación del elemento con el nombre de la clase star-1 cambiando su regla @keyframes al 50%.*/
  
  <style>
    .stars {
      background-color: white;
      height: 30px;
      width: 30px;
      border-radius: 50%;
      animation-iteration-count: infinite;
    }
  
    .star-1 {
      margin-top: 15%;
      margin-left: 60%;
      animation-name: twinkle-1;
      animation-duration: 1s;
    }
  
    .star-2 {
      margin-top: 25%;
      margin-left: 25%;
      animation-name: twinkle-2;
      animation-duration: 1s;
    }
  
    @keyframes twinkle-1 {
      50% {
        transform: scale(0.5);
        opacity: 0.5;
      }
    }
  
    @keyframes twinkle-2 {
      20% {
        transform: scale(0.5);
        opacity: 0.5;
      }
    }
  
    #back {
      position: fixed;
      padding: 0;
      margin: 0;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(black, #000099, #66c2ff, #ffcccc, #ffeee6);
    }
  </style>
  
  <div id="back"></div>
  <div class="star-1 stars"></div>
  <div class="star-2 stars"></div>
  
  /*Animar múltiples elementos con ritmos diferentes*/
  /*En el desafío anterior, cambiaste el ritmo de la animación para dos elementos similares animados alterando sus reglas @keyframes. Puedes lograr el mismo objetivo manipulando la animation-duration de múltiples elementos.
  
  En la animación que se ejecuta en el editor de código, hay tres estrellas en el cielo que brillan a la misma velocidad en un ciclo continuo. Para hacerlos titilar con diferentes ritmos, puedes establecer la propiedad animation-duration con diferentes valores para cada elemento.
  
  Establece la animation-duration de los elementos con las clases star-1, star-2y star-3 a 1s, 0.9s y 1.1s, respectivamente.*/
  
  <style>
    .stars {
      background-color: white;
      height: 30px;
      width: 30px;
      border-radius: 50%;
      animation-iteration-count: infinite;
    }
  
    .star-1 {
      margin-top: 15%;
      margin-left: 60%;
      animation-duration: 1s;
      animation-name: twinkle;
    }
  
    .star-2 {
      margin-top: 25%;
      margin-left: 25%;
      animation-duration: 0.9s;
      animation-name: twinkle;
    }
  
    .star-3 {
      margin-top: 10%;
      margin-left: 50%;
      animation-duration: 1.1s;
      animation-name: twinkle;
    }
  
    @keyframes twinkle {
      20% {
        transform: scale(0.5);
        opacity: 0.5;
      }
    }
  
    #back {
      position: fixed;
      padding: 0;
      margin: 0;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(black, #000099, #66c2ff, #ffcccc, #ffeee6);
    }
  </style>
  
  <div id="back"></div>
  <div class="star-1 stars"></div>
  <div class="star-2 stars"></div>
  <div class="star-3 stars"></div>
  
  /*Cambia la duración de las animaciones con palabras clave*/
  /*En las animaciones CSS, la propiedad animation-timing-function controla qué tan rápido un elemento animado cambia sobre la duración total de la animación. Si la animación es un carro moviéndose de un punto A a un punto B en un tiempo establecido (tu animation-duration), la animation-timing-function dicta cómo el carro acelera y desacelera durante el transcurso en marcha.
  
  Existe un número de palabras clave predefinidas disponibles para las opciones populares. Por ejemplo, el valor por defecto es ease, que empieza despacio, acelera en el medio y luego reduce la velocidad de nuevo al final. Otras opciones incluye ease-out, que es rápida al inicio y luego reduce la velocidad, ease-in, que es lenta al inicio y luego acelera al final, o linear, que aplica una velocidad constante a lo largo de la animación.
  
  Para los elementos con id ball1 y ball2, agrega una propiedad animation-timing-function a cada uno y asigna linear a #ball1 y ease-out a #ball2. Nota la diferencia entre cómo los elementos se mueven durante la animación pero terminan juntos, dado que comparten la misma animation-duration de 2 segundos.*/
  
  <style>
  
    .balls {
      border-radius: 50%;
      background: linear-gradient(
        35deg,
        #ccffff,
        #ffcccc
      );
      position: fixed;
      width: 50px;
      height: 50px;
      margin-top: 50px;
      animation-name: bounce;
      animation-duration: 2s;
      animation-iteration-count: infinite;
      animation-timing-function: linear;
    }
    #ball1 {
      left:27%;
      animation-timing-function: linear;
  
    }
    #ball2 {
      left:56%;
      animation-timing-function: ease-out;
  
    }
  
    @keyframes bounce {
      0% {
        top: 0px;
      }
      100% {
        top: 249px;
      }
    }
  
  </style>
  
  <div class="balls" id="ball1"></div>
  <div class="balls" id="ball2"></div>
  
  
  
  
  /*Descubre como funcionan las curvas de Bezier*/
  /*El último desafío introdujo la propiedad animation-timing-function y algunas palabras clave que cambian la velocidad de una animación a lo largo de su duración. CSS ofrece una opción distinta a las palabras clave que proporciona un control aún más fino sobre cómo se desarrolla la animación, a través del uso de curvas Bezier.
  
  En las animaciones CSS, las curvas Bezier se utilizan con la función cubic-bezier. La forma de la curva representa cómo se desarrolla la animación. La curva vive en un sistema de coordenadas de 1 a 1. El eje X de este sistema de coordenadas es la duración de la animación (piénsa en una escala de tiempo), y el eje Y es el cambio en la animación.
  
  La función cubic-bezier consta de cuatro puntos principales que se encuentran en esta cuadrícula de 1 por 1: p0, p1, p2 y p3. p0 y p3 están configurados para ti: son los puntos inicial y final que siempre se encuentran respectivamente en el origen (0, 0) y (1, 1). Establece los valores x e y para los otros dos puntos, y donde los coloca en la cuadrícula determina la forma de la curva para la animación que debe seguir. Esto se hace en CSS declarando los valores x e y de los puntos "anchor" p1 y p2 de la siguiente forma:(x1, y1, x2, y2). Juntando todo, aquí hay un ejemplo de una curva de Bezier en codigo CSS:
  
  animation-timing-function: cubic-bezier(0.25, 0.25, 0.75, 0.75);
  En el ejemplo anterior, los valores x e y son equivalentes para cada punto (x1 = 0.25 = y1 y x2 = 0.75 = y2), que si recuerdas la clase de geometría, da como resultado una línea que se extiende desde el origen hasta el punto (1, 1). Esta animación es un cambio lineal de un elemento durante la duración de una animación, y es lo mismo que usar la palabra clave linear. En otras palabras, cambia a una velocidad constante.
  
  Para el elemento con el id de ball1, cambia el valor de la propiedad animation-timing-function de linear a su valor de función cubic-bezier equivalente. Utiliza los valores de puntos dados en el ejemplo anterior.*/
  
  <style>
  
    .balls{
      border-radius: 50%;
      background: linear-gradient(
        35deg,
        #ccffff,
        #ffcccc
      );
      position: fixed;
      width: 50px;
      height: 50px;
      margin-top: 50px;
      animation-name: bounce;
      animation-duration: 2s;
      animation-iteration-count: infinite;
    }
    #ball1 {
      left: 27%;
      animation-timing-function: cubic-bezier(0.25, 0.25, 0.75, 0.75); /*de este se trata este acápite*/
    }
    #ball2 {
      left: 56%;
      animation-timing-function: ease-out;
    }
  
    @keyframes bounce {
      0% {
        top: 0px;
      }
      100% {
        top: 249px;
      }
    }
  
  </style>
  
  <div class="balls" id="ball1"></div>
  <div class="balls" id="ball2"></div>
  
  
  /*Usa una curva de Bezier para mover un gráfico*/
  /*Un desafío anterior discutió la palabra clave ease-out que describe un cambio de animación que se acelera primero y luego se ralentiza al final de la animación. A la derecha, se muestra la diferencia entre la palabra clave ease-out (para el elemento azul) y la palabra clave linear (para el elemento rojo). Se pueden lograr progresiones de animación similares a la palabra clave ease-out utilizando una función de curva Bezier cúbica personalizada.
  
  En general, el cambio de los puntos de anclaje p1 y p2 impulsa la creación de diferentes curvas Bezier, que controlan como la animación progresa a través del tiempo. Aquí hay un ejemplo de una curva de Bezier que usa valores para imitar el estilo de facilidad:
  
  animation-timing-function: cubic-bezier(0, 0, 0.58, 1);
  Recuerda que todas las funciones cubic-bezier comienzan con p0 en (0, 0) y terminan con p3 en (1, 1). En este ejemplo, la curva se mueve más rápido a través del eje Y (comienza en 0, va a p1 y valor de 0, luego va a p2 y valor de 1) que se mueve a través del eje X (0 para iniciar, luego 0 para p1, hasta 0.58 para p2. Como resultado, el cambio en el elemento animado progresa más rápido que el tiempo de la animación para ese segmento. Hacia el final de la curva, la relación entre el cambio en los valores X e Y se invierte: el valor y se mueve de 1 a 1 (sin cambios), y los valores X se mueven de 0.58 a 1, lo que hace que los cambios de animación progresen más lentamente en comparación con la duración de la animación.
  
  Para ver el efecto de esta curva Bezier en acción, cambia la animation-timing-function del elemento con id de red a una función cubic-bezier con valores x1, y1, x2, y2 establecidos respectivamente en 0, 0, 0.58, 1. Esto hará que ambos elementos progresen a través de la animación de manera similar.*/
  
  <style>
    .balls{
      border-radius: 50%;
      position: fixed;
      width: 50px;
      height: 50px;
      margin-top: 50px;
      animation-name: bounce;
      animation-duration: 2s;
      animation-iteration-count: infinite;
    }
    #red {
      background: red;
      left: 27%;
      animation-timing-function: cubic-bezier(0, 0, 0.58, 1);
    }
    #blue {
      background: blue;
      left: 56%;
      animation-timing-function: ease-out;
    }
    @keyframes bounce {
      0% {
        top: 0px;
      }
      100% {
        top: 249px;
      }
    }
  </style>
  <div class="balls" id= "red"></div>
  <div class="balls" id= "blue"></div>
  
  /*Haz que el movimiento sea más natural usando una curva de Bezier*/
  /*Este desafío anima un elemento para replicar el movimiento de una pelota que se hace rebotes. Los desafíos anteriores cubrirán las curvas cúbicas de Bezier linear y ease-out, sin embargo, ninguna representa el movimiento de rebotes con precisión. Necesitas personalizar una curva de Bezier para esto.
  
  La función animation-timing-function se realiza automáticamente en cada fotograma clave (keyframe) cuando el animation-iteration-count se establece en infinito. Dado que hay una regla de fotogramas clave establecida en el medio de la duración de la animación (en 50%, da como resultado dos progresiones de animación idénticas en el movimiento hacia arriba y hacia abajo de la pelota.
  
  La siguiente curva cúbica de Bezier simula el movimiento de rebotes:
  
  cubic-bezier(0.3, 0.4, 0.5, 1.6);
  Observa que el valor de y2 es mayor que 1. Aunque la curva cúbica de Bezier se mapea en un sistema de coordenadas 1 por 1, y solo puede aceptar valores x de 0 a 1, el valor y se puede establecer en números mayores que uno. Esto da como resultado un movimiento de rebote que es ideal para simular la pelota rebotando.
  
  Cambia el valor de la función animation-timing-function del elemento con el id de green a una función cubic-bezier con valores x1, y1, x2, y2 establecidos respectivamente en 0.311, 0.441, 0.444, 1.649.*/
  
  <style>
    .balls {
      border-radius: 50%;
      position: fixed;
      width: 50px;
      height: 50px;
      top: 60%;
      animation-name: jump;
      animation-duration: 2s;
      animation-iteration-count: infinite;
    }
    #red {
      background: red;
      left: 25%;
      animation-timing-function: linear;
    }
    #blue {
      background: blue;
      left: 50%;
      animation-timing-function: ease-out;
    }
    #green {
      background: green;
      left: 75%;
      animation-timing-function: cubic-bezier(0.311, 0.441, 0.444, 1.649);
    }
  
    @keyframes jump {
      50% {
        top: 10%;
      }
    }
  </style>
  <div class="balls" id="red"></div>
  <div class="balls" id="blue"></div>
  <div class="balls" id="green"></div>