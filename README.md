# Oliver-CSS3-Responsive
usando css3 y repsonsive
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, user-scalable=no">
    <link rel="stylesheet" href="css/estilos.css">
    <link href="https://fonts.googleapis.com/css?family=Dancing+Script" rel="stylesheet">
    <title>Paisajes</title>
    <style>
    /*selector de fuente o tipo de letra general para toda las paginas*/
*{
  font-family: 'Dancing Script', cursive;
}
/*decoracion de cabecera y enlaces*/
.cabecera{
  display: flex;
  flex-direction: column;
  width: 100%;
}
.contenedor{
  background-color: #5b7989;
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
  width: 100%;
}
div .titulo  {
  width: 100%;
  color: white;
  text-align: left;
  font-size: 16px;
  padding-top: 1%;
  padding-left: 2%;
  margin-bottom: -20px;
  text-shadow: 2px 2px #02010a;
}
div .enlaces{
word-spacing: 20px;
text-align: right;

}

a h1{
  color: white;
  display: inline-block;
  padding-right: 5%;
  padding-bottom: .25%;
  margin-top: -10%;
}
/*fin de la decoracion header*/
/*///////////////////////////////////////////////////////////*/
/*sombra de imagenes en general///////////////////////*/
div div img{
  box-shadow: 2px 2px #02010a;
}
/*///////////////////////////////////////////////////////////*/
/*DECORACION IMAGEN CENTRAL///////////////////////*/
.principal .primero div img{
  width: 90%;
}
.principal .primero{
  background-color: #82c3a6;
  text-align: center;
  padding: 2%;
}
/*///////////////////////////////////////////////////////////*/
/*DECORACION IMAGENES IZQUIERDO Y DERECHO///////////////////////*/
#segundo{
  background-color: #d5c75f;
  display: inline-flex;
  flex-direction: row;
  padding-top: 3%;
  padding-left: 2%;
}
#segundo div img{
  width: 100%;
  box-shadow: 2px 2px #82c3a6;
}
.retrato, .paisaje{
  padding: 2%;
  text-align: center;
  width: 45%;
}
#pie_retrato, #pie_paisaje{
  color: black;
}

/*footer decoration////////////////////////////////////////*/
.piepie{
  width: 100%;
  height: 100%;

}
.icon{
  width: 20px;
  height: 20px;
}

section{
  width: 100%;
}
article{
  width: 25%;
  display: inline-block;
  float: left;
  background-color: #C6d5c5;
  border-bottom-right-radius: 10px;
  border-bottom-left-radius: 10px;
  padding-left: 0px;
  text-align: center;

}
article ul h1{
  margin-bottom: 0px;
  font-size: 25px;
}
ul li{
  list-style: none;
  margin-top: -1px;
  font-size: 20px;
}
li a{
  color: inherit;
  text-decoration: none;
  font-size: 20px;
  text-align: center;
}
/*/////ANIMACIONES INICIO////////*//*//////////////////////////*/
.izquierda{
  border: 2px #82c3a6;
  -webkit-transition: -webkit-transform 1s ease-out;
  -moz-transition: -moz-transform 1s ease-out;
   transition: transform 1s ease-out;
 }
.izquierda:hover {
  -webkit-transform: rotate(10deg);
  -moz-transform: rotate(10deg);
   transform: rotate(10deg);
}
/*//////////////////////////////////////////////////////////*/
.derecha{
  border: 2px #82c3a6;
  animation-name: derecha-animacion;
  animation-duration: 4s;
  -webkit-animation-delay: 2s;
  -moz-animation-delay: 2s;
  -o-animation-delay: 2s;
  animation-delay: 2s;
}
.derecha:hover {
  -webkit-transform: translateX(10px);
  -moz-transform: translateX(10px);
   transform: translateX(10px);
}
/*/////////////////////////////////////////////////*/
/*decoracion retratos/////////////////////*/
.firstfile, .secondfile{
  background-color: #d5c75f;
  display: inline-flex;
  flex-direction: row;
  padding-top: 2%;
  padding-left: 1%;
  padding-bottom: 2%;
}
.container div img{
  width: 100%;
}
.retrato1, .retrato2, .retrato3,
.retrato4, .retrato5, .retrato6 {
  padding: 2%;
  text-align: center;
  width: 100%;
}
.retrato1, .paisaje1{
  -webkit-filter: blur(10px);
  filter: blur(10px);
}
.retrato2, .retrato4, .retrato6,
.paisaje2, .paisaje4, .paisaje6{
  -webkit-filter: grayscale(100%);
  -filter: grayscale(100%);
}
.retrato3, .paisaje3{
  -webkit-filter: sepia(90%);
  filter: sepia(90%);
}
/*/////////////////////////////////////////////////////*/
/*decoracion paisajes/////////////////////*/
/* .firstfile, .secondfile{
  background-color: #d5c75f;
  display: inline-flex;
  flex-direction: row;
  padding-top: 3%;
  padding-left: 1%;
  padding-bottom: 1%;
}
.container div img{
  width: 100%;
} */
.paisaje1, .paisaje2, .paisaje3,
.paisaje4, .paisaje5, .paisaje6 {
  padding: 2%;
  text-align: center;
  width: 100%;
}
/*/////////////////////////////////////////////////////*/
</style>
    
  </head>
  <body>

    <header>
      <div class="cabecera">

        <div class="contenedor">

          <div class="titulo">
            <h1>Comenzando con la fotografía</h1>
            <div class="enlaces">
            <a href="index.html"><h1> Inicio</h1></a>
            <a href="paisajes.html"><h1> Paisajes</h1></a>
            <a href="retratos.html"><h1> Retratos</h1></a>
          </div>
        </div>
      </div>
    </header>

    <div class="container">

      <div class="firstfile">
          <div class="paisaje1"><img src="img/paisaje1.jpg"></div>
          <div class="paisaje2"><img src="img/paisaje2.jpg"></div>
          <div class="paisaje3"><img src="img/paisaje3.jpg"></div>
      </div>

      <div class="secondfile">
          <div class="paisaje4"><img src="img/paisaje4.jpg"></div>
          <div class="paisaje5"><img src="img/paisaje5.jpg"></div>
          <div class="paisaje6"><img src="img/paisaje6.jpg"></div>
      </div>
    </div>

  </body>
  <footer>
    <article class="piepie">

    <section class="footpag">
      <article class="contactos">
        <h1>Contactos</h1>
          <ul>
            <li>oliverperu@outlook.com</li>
            <li>Teléfono: 945202936</li>
            <li>Whatsapp: 945202936</li>
          </ul>
      </article>
    </section>

    <section class="footpag">
      <article class="terminos">
        <h1>Términos</h1>
          <ul>
            <li>Términos</li>
            <li>Condiciones</li>
            <li>Penalidades</li>
          </ul>
      </article>
    </section>
    <section class="footpag">
      <article class="redes">
        <h1>Redes Sociales</h1>
          <ul>
            <li><a href="https://github.com/OliverM24"><img src="icon/github.png" class="icon">GitHub </a></li>
            <li><a href="https://twitter.com/Oliver_UPC"><img src="icon/twitter.png" class="icon">Twitter </a></li>
            <li><a href="https://web.facebook.com/huamanlazo24"><img src="icon/facebook.png" class="icon">Facebook </a></li>
          </ul>
      </article>
    </section>

    <section class="footpag">
      <article class="derechos">
        <h1>Derechos</h1>
          <ul>
            <li> Oliver Muñoz </li>
            <li>Huamanlazo</li>
            <li>&copy;2018</li>
          </ul>
      </article>
    </section>
  </article>
  </footer>
</html>
