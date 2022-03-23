Responsive Web Design Principles

-----------------------

/*Crea un media query*/

/*Las consultas de medios (Media Queries) son una nueva técnica introducida en CSS3 que cambia la presentación de contenido basado en diferentes tamaños de viewport. El viewport es el área visible del usuario de una página web, y es diferente dependiendo del dispositivo utilizado para acceder al sitio.

Las consultas de medios se basan en un tipo de medio, y si ese tipo de medio coincide con el tipo de dispositivo en el que se muestra el documento, los estilos se aplican. Puedes tener tantos selectores y estilos dentro de tu consultas de medios como desees.

Aquí hay un ejemplo de una consulta multimedia que devuelve el contenido cuando el ancho del dispositivo es menor o igual a 100px:*/

@media (max-width: 100px) { /* CSS Rules */ }
y la siguiente consultas de medios devuelve el contenido cuando la altura del dispositivo es mayor o igual a 350px:

@media (min-height: 350px) { /* CSS Rules */ }
Recuerda, el CSS dentro de las consultas de medios se aplica sólo si el tipo de medio coincide con el del dispositivo que se está usando.


/*Aquí puedes poner algunas cosas extras más*/
El media querry funciona como cualquier otro selector

@mdia all (max-width: 100px) { /* CSS Rules */ } 


/* el all es para indicar que va apliacar a todo tipo de pantalla. Pero si lo ignoras en automatico toma el valor all. */ Puedes usar como cualquer selector y darle todas las reglas que quieras de CSS.

@media (orientation: landscape){
    title{
        color: red;
    }
} /*esto cambiaa cuando la altura se pone horizontal, se ajusta a las indicaciones que le pones dentro de la reglas*/


 @media(orientation: portrait){/* aqui las reglas*/} Indica que es horizontal los cambios que se van a plicar.
@media(orientation:landscape) and (max-width: 100px){/reglas de CCS*/} /* Con esto puedes combinar lo que quieras segun tu quieras*/ 
and /*Es un concatenador*/
, /es un o */ 




/*Agrega una consultas de medios, de forma que la etiqueta p tenga un font-size de 10px cuando la altura del dispositivo sea menor o igual a 800px.*/



<style>
  p {
    font-size: 20px;
  }

  /* Cambia solo el código debajo de esta línea */
     
  }

@media (max-height: 800px){ 
    p {
    font-size: 10px;
      }
  }

  /* Cambia solo el código encima de esta línea */
</style>

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus quis tempus massa. Aenean erat nisl, gravida vel vestibulum cursus, interdum sit amet lectus. Sed sit amet quam nibh. Suspendisse quis tincidunt nulla. In hac habitasse platea dictumst. Ut sit amet pretium nisl. Vivamus vel mi sem. Aenean sit amet consectetur sem. Suspendisse pretium, purus et gravida consequat, nunc ligula ultricies diam, at aliquet velit libero a dui.</p>


------------------
Haz una imagen responsiva
/*Hacer imágenes responsivas con CSS es realmente simple. Sólo tienes que agregar estas propiedades a una imagen:*/

img {
  max-width: 100%;
  height: auto;
}

 /*otro ejemplo*/
 <style>
.responsive-img {
max-width: 100%; /* aquí el asunto*/
  display: block; /* aquí*/
  height: auto; /* aquí*/

}

img {
  width: 600px;
}
</style>

<img class="responsive-img" src="https://s3.amazonaws.com/freecodecamp/FCCStickerPack.jpg" alt="freeCodeCamp stickers set">
<img src="https://s3.amazonaws.com/freecodecamp/FCCStickerPack.jpg" alt="freeCodeCamp stickers set">


/*El ancho máximo max-width de 100% se asegurará de que la imagen nunca es más ancha que el contenedor en el que se encuentra. y la altura height de auto hará que la imagen mantenga su relación de aspecto original.*/


--------------------

Usa una imagen retina para pantallas de alta resolución
/*Con el aumento de los dispositivos conectados a Internet, sus tamaños y especificaciones varían, y las pantallas que utilizan podrían ser diferentes tanto externa como internamente. La densidad de píxeles es un aspecto que puede ser diferente de un dispositivo a otro, esta densidad se conoce como Pixel Por Pulgada, en inglés "pixels per inch" (PPI) o Puntos por Pulgada, en inglés "dots per inch" (DPI). La pantalla más famosa que aprovecha esto es la conocida como "Pantalla Retina" en los últimos portátiles Apple MacBook Pro, y recientemente en los ordenadores iMac. Debido a la diferencia en la densidad de píxeles entre las pantallas de "Retina" y "No Retina", algunas imágenes que no han sido hechas con una pantalla de alta resolución en mente podrían verse "pixeladas" cuando se muestran en una pantalla de alta resolución.

La forma más sencilla de hacer que tus imágenes aparezcan correctamente en pantallas de alta resolución, tales como la "pantalla retina" de las MacBook Pros es definir sus valores de ancho width y de altura height como sólo la mitad de lo que es el archivo original. Aquí hay un ejemplo de una imagen que solo utiliza la mitad de la altura y ancho originales:*/

<style>
  img { height: 250px; width: 250px; }
</style>

<img src="coolPic500x500" alt="A most excellent picture">


/*Aquí otro ejemplo */

<style>
img{
  height:100px;
  width:100px;
}
</style>

<img src="https://s3.amazonaws.com/freecodecamp/FCCStickers-CamperBot200x200.jpg" alt="freeCodeCamp sticker that says 'Because CamperBot Cares'">


/*Establece el width y height de la etiqueta img a la mitad de sus valores originales. En este caso, tanto el height original como el width original son de 200px.*/

----------------------------
 
Haz tipografía responsiva
/*En lugar de usar em o px para dimensionar texto, puedes usar unidades de viewport para obtener una tipografía responsiva. Las unidades de viewport, como los porcentajes, son unidades relativas, pero se basan en objetos diferentes. Las unidades de viewport son relativas a las dimensiones del viewport (ancho o alto) de un dispositivo, y los porcentajes son relativos al tamaño del elemento contenedor padre.

Las cuatro diferentes unidades de viewport son:*/

vw (viewport width): 10vw sería el 10% del ancho del viewport.
vh (viewport height): 3vh sería el 3% del alto del viewport.
vmin (viewport mínimo): 70vmin sería el 70% de la dimensión más pequeña del viewport (altura o ancho).
vmax (viewport máximo): 100vmax sería el 100% de la dimensión más grande del viewport (altura o ancho).
Aquí hay un ejemplo que establece una etiqueta body al 30% del ancho del viewport.

body { width: 30vw; }
/*Establece el ancho width de la etiqueta h2 al 80% del ancho del viewport y el ancho width del párrafo como el 75% de la dimensión más pequeña del viewport.*/

/*aquí otro ejemplo*/
<style>
h2{
  width:80 vw;
}
p{
  width:75vmin;
}
</style>

<h2>Importantus Ipsum</h2>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus quis tempus massa. Aenean erat nisl, gravida vel vestibulum cursus, interdum sit amet lectus. Sed sit amet quam nibh. Suspendisse quis tincidunt nulla. In hac habitasse platea dictumst. Ut sit amet pretium nisl. Vivamus vel mi sem. Aenean sit amet consectetur sem. Suspendisse pretium, purus et gravida consequat, nunc ligula ultricies diam, at aliquet velit libero a dui.</p>

