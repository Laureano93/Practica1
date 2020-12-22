# Practica Con Flex

- Descripcion Del Proyecto
- Desarrollo Del Proyecto
- Visualizacion Del Proyecto
- Enlaces
- Licencias

---

**Descripcion Del Proyecto**

*Consisten en realizar una pagina web donde se muestra un header(con su
correspondiente informacion), un nav donde se muestra un menu junto con 2 imagenes
con un comentario debajo.
Debajo 3 fotos alineadas con respecto a las 2 de arriba y un footer debajo donde muestro
las redes sociales, licencia y ubicacion de las fotos. Todo esto empleando contenedores y
css3 para que mediante el uso de flex se queden alineadas y quede una buena maquetacion*

## Desarrollo Del Proyecto
*Mediante el visual studio code desarrollo un archivo html que contiene:*

~~~
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Laureano Guillen Dil">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.15.1/css/all.css" integrity="sha384-vp86vTRFVJgpjF9jiIGPEEqYqlDwgyBgEF109VFjmqGmIY/Y4HV4d3Gp2irVfcrp" crossorigin="anonymous">
    <link rel="stylesheet" href="estilos_completar.css">
    <title>maquetacionFLEX_Practica01 Guillen Dil Laureano</title>

</head>

<body>

    <!-- Laureano Guillen Dil -->

    <div class="container">
        <header>

            <h1 class="i1">Ejemplo de maquetacion con flex</h1>
            <h2 class="i2">by Isabel Cayuela Perez para Diseño de Interfaces Web</h2>
        </header>
        <div class="content_wrapper">


            <div class="nav">
                <nav>

                    <ul>

                        <li>Inicio</li>
                        <li>Galeria</li>
                        <li>Productos</li>
                        <li>Clientes</li>
                        <li>Sobre Nosotros</li>
                        <li>Contacto</li>

                    </ul>

                </nav>


            </div>


            <div class="im1">
                <main>

                    <img src="./img/1.jpg" width="580px" height="490px" class="imagen1">

                    <p class="p1">Caballos en libertad, imagen tomada en el campillo a pie de la sierra de las estancias
                    </p>
                    <p class="p1">Almeria. Valerosa y Hera
                    </p>
                    <p class="p1">La sierra de las estancias es un macizo montañoso español que cruza transversalmente el norte
                    </p>
                    <p class="p1">De la provincia de almeria
                    </p>

                </main>


            </div>





            <div class="ar1">
                <article>

                    <img src="./img/2jpg.jpg" width="280px" height="490px" class="imagen2">
                    <p class="p5">Una imagen de luminosa</p>

                </article>


            </div>

        </div>
        <div class="articles">

            <div class="ar2">
            <article>
                <img src="./img/3.jpg" width="300px" height="290px" class="imagen3">
                <p class="p3">Una imagen de valerosa,quiron y rucha</p>

            </article>

            </div>


            <div class="ar2">


            <article>
                <img src="./img/4.jpg" width="300px" height="290px" class="imagen4">
                <p class="p3">Una imagen de favorito</p>

            </article>

        </div>


           <div class="ar2">


            <article>

                <img src="./img/5.jpg" width="300px" height="290px" class="imagen5">
                <p class="p3">Una imagen de valerosa y hera</p>

            </article>

        </div>

        </div>
        <footer>
            <address> 
                Laureano Guillen Dil
            </address>
            <div class="copyright"> 

                  <p class="p4">Todas las fotos realizadas por Isabel Cayuela Perez bajo la licencia CC B-Y-SA</p>

            </div>
            <div class="social"> 
            
                <i class="fab fa-snapchat-square"></i>
                <i class="fab fa-facebook"></i>
                <i class="fab fa-twitter"></i>
            
 
            </div>
        </footer>
    </div>












</body>

</html>
~~~

*Agrego el archivo css con el siguiente codigo:*

~~~

/*Caracteristicas generales: margenes 0, fuente Font google, tamaño de fuente responsive*/

/* BOX-SIZING para calcular directamente todas las dimensiones de las cajas */


/* RESETEO LIMITADO DE PROPIEDADES margen 0*/


/*Aspecto especifico*/
/* classe .container - fuente, color, 80% ancho y centrado*/


/*color de la letra específico*/

/*La cabecera*/

/* El contenedor flex para la primera fila de contenido .content_wrapper. Dirección, El ajuste,
 Alineación horizontal, Alineación vertical   */

/* El menú */

/* El elemento principal main*/

/* Artículo. Imágenes pequeñas */

/* El contenedor flex para la segunda fila de contenido .articles. Dirección, El ajuste,
 Alineación horizontal, Alineación vertical   */

/* Pie de la página */
/* El contenedor flex para la tercera fila de contenido footer. Dirección, El ajuste,
 Alineación horizontal, Alineación vertical   */


@import url('https://fonts.googleapis.com/css2?family=Langar&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Andika+New+Basic&display=swap');



* {

  margin: 0;



}

.container {

  width: 80%;

  text-align: center;


}

.i1 {


  width: 100%;

  max-width: 10000px;

  color: aquamarine;

  font-family: 'Langar', cursive;

}

.i2 {

  width: 100%;

  max-width: 10000px;

  color: blue;

  font-family: 'Andika New Basic', sans-serif;

}


header {

  width: 100%;
  max-width: 1000px;

  padding-bottom: 83px;
  padding-left: 190px;
}

.nav {

  width: 100%;
  height: 100%;
  max-width: 150px;
  max-height: 490px;
  flex: 1 1 30%;


}


.content_wrapper {


  width: 100%;
  max-width: 2000px;

  box-sizing: border-box;

  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-around;
  padding-bottom: 34px;

  flex: 1 1 100%;



}

.content_wrapper li {

  color: green;
  list-style: none;
  padding-bottom: 39px;

}

.im1 {


  flex: 1 1 80%;

}

.p1 {

  width: 100%;
  max-width: 1300px;
  color: aquamarine;

  font-family: 'Langar', cursive;


}




.ar1 {



  flex: 1 1 40%;


}


.p5 {

  width: 100%;
  max-width: 1300px;
  color: aquamarine;

  font-family: 'Langar', cursive;

  font-weight: bold;

  font-size: 27px;



}

.articles{

 


  width: 100%;
  max-width: 2000px;

  box-sizing: border-box;

  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-around;
  flex: 1 1 100%;

  padding-left: 170px;

  padding-bottom: 60px;


}

.ar2{

flex: 1 1 33%;

}



.p3 {

  width: 100%;
  max-width: 1300px;
  color: aquamarine;

  font-family: 'Langar', cursive;

  font-weight: bold;

  font-size: 25px;



}

footer{

  width: 100%;
  max-width: 2000px;
  box-sizing: border-box;

  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-around;
  flex: 1 1 100%;


}

address{

  flex: 1 1 33%;


}

.copyright{


  flex: 1 1 48%;
}

.social{


  flex: 1 1 14%;
}

.p4{

  width: 100%;
  max-width: 1300px;
  color: aquamarine;

  font-family: 'Langar', cursive;

  font-weight: bold;

  font-size: 15px;

}

i{

  font-size: 33px;
}


/*  Ajustar las dos primeras imagenes, dependiendo del ancho maximo de la pantalla se va modificando  */


@media screen and (max-width:1500px) {


  .imagen1 {




    max-width: 480px;



  }


  .imagen2 {



    max-width: 280px;





  }

  


}


@media screen and (max-width:1400px) {



  .imagen1 {




    max-width: 350px;



  }


  .imagen2 {



    max-width: 230px;



  }



  




}



@media screen and (max-width:1350px) {



  .imagen1 {




    max-width: 400px;



  }


  .imagen2 {



    max-width: 260px;



  }


  









}


@media screen and (max-width:1250px) {


  .imagen1 {




    max-width: 340px;



  }


  .imagen2 {



    max-width: 200px;



  }



  





}


@media screen and (max-width:1150px) {




  .imagen1 {




    max-width: 310px;



  }


  .imagen2 {



    max-width: 220px;



  }

  



}


@media screen and (max-width:1050px) {




  .imagen1 {


    width: 300px;



  }

  .imagen2 {


    width: 210px;

  }


  





}





@media screen and (max-width:980px) {






  .imagen1 {


    width: 280px;



  }

  .imagen2 {


    width: 190px;

  }


  




}









@media screen and (max-width:880px) {


  .i1 {

    width: 100%;

    max-width: 10000px;

    color: aquamarine;

    font-family: 'Langar', cursive;

    font-size: 30px;

  }

  .i2 {


    width: 100%;

    max-width: 10000px;

    color: blue;

    font-family: 'Andika New Basic', sans-serif;

    font-size: 16px;

  }




  .imagen1 {


    width: 250px;



  }

  .imagen2 {


    width: 175px;

  }

  

  
}


@media screen and (max-width:750px) {



  .i1 {

    text-align: left;

    width: 100%;

    max-width: 10000px;

    color: aquamarine;

    font-family: 'Langar', cursive;

    font-size: 30px;

  }

  .i2 {

    text-align: left;
    width: 100%;

    max-width: 10000px;

    color: blue;

    font-family: 'Andika New Basic', sans-serif;

    font-size: 16px;

  }






  .imagen1 {


    width: 240px;



  }

  .imagen2 {


    width: 170px;

  }

  

  




}




@media screen and (max-width:700px) {


  .i1 {

    text-align: left;

    width: 100%;

    max-width: 10000px;

    color: aquamarine;

    font-family: 'Langar', cursive;

    font-size: 25px;

  }

  .i2 {

    text-align: left;
    width: 100%;

    max-width: 10000px;

    color: blue;

    font-family: 'Andika New Basic', sans-serif;

    font-size: 13px;

  }







  .imagen1 {


    width: 180px;



  }

  .imagen2 {


    width: 150px;

  }


 



  




}


@media screen and (max-width:650px) {


  .i1 {

    text-align: left;

    width: 100%;

    max-width: 10000px;

    color: aquamarine;

    font-family: 'Langar', cursive;

    font-size: 20px;

  }

  .i2 {

    text-align: left;
    width: 100%;

    max-width: 10000px;

    color: blue;

    font-family: 'Andika New Basic', sans-serif;

    font-size: 10px;

  }




  .imagen1 {


    width: 150px;



  }

  .imagen2 {


    width: 130px;

  }


  


  
} 



/*  Ajustar las 3 imagenes, dependiendo del ancho maximo de la pantalla se va modificando  */



@media screen and (max-width:1400px){


  .imagen3{


    width: 280px;
  }

  .imagen4{


    width: 280px;
  }

  .imagen5{


    width: 280px;
  }




}


@media screen and (max-width:1350px){


  .imagen3{


    width: 260px;
  }

  .imagen4{


    width: 260px;
  }

  .imagen5{


    width: 260px;
  }




}


@media screen and (max-width:1300px){


  .imagen3{


    width: 270px;
  }

  .imagen4{


    width: 270px;
  }

  .imagen5{


    width: 270px;
  }




}


@media screen and (max-width:1250px){


  .imagen3{


    width: 250px;
  }

  .imagen4{


    width: 250px;
  }

  .imagen5{


    width: 250px;
  }




}


@media screen and (max-width:1180px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 140px;
  
  
  }


  .imagen3{


    width: 250px;
  }

  .imagen4{


    width: 250px;
  }

  .imagen5{


    width: 250px;
  }




}


@media screen and (max-width:1140px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 140px;
  
  
  }


  .imagen3{


    width: 240px;
  }

  .imagen4{


    width: 240px;
  }

  .imagen5{


    width: 240px;
  }




}


@media screen and (max-width:1120px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 100px;
  
  
  }


  .imagen3{


    width: 240px;
  }

  .imagen4{


    width: 240px;
  }

  .imagen5{


    width: 240px;
  }




}


@media screen and (max-width:1090px){

  .articles{

  
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 100px;
  
  
  }


  .imagen3{


    width: 230px;
  }

  .imagen4{


    width: 230px;
  }

  .imagen5{


    width: 230px;
  }




}

@media screen and (max-width:980px){

  .articles{

   
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 80px;
  
  
  }


  .imagen3{


    width: 210px;
  }

  .imagen4{


    width: 210px;
  }

  .imagen5{


    width: 210px;
  }




}



@media screen and (max-width:920px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 70px;
  
  
  }


  .imagen3{


    width: 200px;
  }

  .imagen4{


    width: 200px;
  }

  .imagen5{


    width: 200px;
  }




}


@media screen and (max-width:870px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 70px;
  
  
  }


  .imagen3{


    width: 190px;
  }

  .imagen4{


    width: 190px;
  }

  .imagen5{


    width: 190px;
  }




}


@media screen and (max-width:820px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 50px;
  
  
  }


  .imagen3{


    width: 190px;
  }

  .imagen4{


    width: 190px;
  }

  .imagen5{


    width: 190px;
  }




}


@media screen and (max-width:798px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 50px;
  
  
  }


  .imagen3{


    width: 180px;
  }

  .imagen4{


    width: 180px;
  }

  .imagen5{


    width: 180px;
  }




}


@media screen and (max-width:790px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 50px;
  
  
  }


  .imagen3{


    width: 170px;
  }

  .imagen4{


    width: 170px;
  }

  .imagen5{


    width: 170px;
  }




}

@media screen and (max-width:750px){

  .articles{

   
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 30px;
  
  
  }


  .imagen3{


    width: 170px;
  }

  .imagen4{


    width: 170px;
  }

  .imagen5{


    width: 170px;
  }




}





@media screen and (max-width:700px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 30px;
  
  
  }


  .imagen3{


    width: 160px;
  }

  .imagen4{


    width: 160px;
  }

  .imagen5{


    width: 160px;
  }




}

@media screen and (max-width:680px){

  .articles{


  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 10px;
  
  
  }


  .imagen3{


    width: 160px;
  }

  .imagen4{


    width: 160px;
  }

  .imagen5{


    width: 160px;
  }




}


@media screen and (max-width:650px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 5px;
  
  
  }


  .imagen3{


    width: 150px;
  }

  .imagen4{


    width: 150px;
  }

  .imagen5{


    width: 150px;
  }




}


@media screen and (max-width:590px){

  .articles{

  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 0px;
  
  
  }


  .imagen3{


    width: 140px;
  }

  .imagen4{


    width: 140px;
  }

  .imagen5{


    width: 140px;
  }




}


@media screen and (max-width:550px){

  .articles{

    
  
  
    width: 100%;
    max-width: 2000px;
  
    box-sizing: border-box;
  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-around;
  
    padding-left: 0px;
  
  
  }


  .imagen3{


    width: 125px;
  }

  .imagen4{


    width: 125px;
  }

  .imagen5{


    width: 125px;
  }




}



/*  Ajustar el texto de las imagenes de abajo  */

@media  screen and (max-width:650px){

  .p3 {

    width: 100%;
    max-width: 1300px;
    color: aquamarine;
  
    font-family: 'Langar', cursive;
  
    font-weight: bold;
  
    font-size: 15px;
  
  
  
  }



}


/* Ajustar iconos cuando se ajusta la pantalla */


@media  screen and (max-width:650px){

  i {

    
  
    font-size: 18px;
  
  
  
  }



}
~~~

### Visualizacion

![](https://github.com/Laureano93/Practica1/blob/Capture/Capture.png?raw=true)

#### Enlaces
[Enlace Del Proyecto](https://github.com/Laureano93/Practica1/commit/db9f9f80684670cdc3ac5ad22a5cbcb1859230c1)

##### Licencia
[![](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/)

