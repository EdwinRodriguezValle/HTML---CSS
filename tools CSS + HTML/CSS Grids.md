CSS GRID

Crea tu primera CSS Grid
/*Convierte cualquier elemento HTML en una cuadrícula al establecer la propiedad display a grid. Esto te da la habilidad de usar todas las demás propiedades asociadas con CSS Grid.

Nota: en CSS Grid, el elemento padre se refiere como el contenedor y sus hijos se llaman elementos.*/

<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}

  .container {
    font-size: 40px;
    width: 100%;
    background: LightGray;
    display: grid; /*aquí el chistesito*/
  }
</style>

<div class="container">
  <div class="d1">1</div>
  <div class="d2">2</div>
  <div class="d3">3</div>
  <div class="d4">4</div>
  <div class="d5">5</div>
</div>


----------------------------------------------------
Agrega columnas con grid-template-columns
/*Crear un simple elemento cuadrícula (grid) no te llevará muy lejos. Necesitas también definir su estructura. Para agregar columnas a la cuadrícula, usa la propiedad grid-template-columns en el contenedor de la cuadrícula como se demuestra a continuación:*/

.container {
  display: grid;
  grid-template-columns: 50px 50px;
}
/*Esto le dará a tu cuadrícula dos columnas que tienen 50px de ancho cada una. El número de parámetros que se le da a la propiedad grid-template-columns indica el número de columnas en la cuadrícula y el valor de cada parámetro indica el ancho de cada columna.*/

<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}

  .container {
    font-size: 40px;
    width: 100%;
    background: LightGray;
    display: grid;
    /* Cambia solo el código debajo de esta línea */

    grid-template-columns: 100px; /*aquí el chiste*/


    /* Cambia solo el código encima de esta línea */
  }
</style>

<div class="container">
  <div class="d1">1</div>
  <div class="d2">2</div>
  <div class="d3">3</div>
  <div class="d4">4</div>
  <div class="d5">5</div>
</div>