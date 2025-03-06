<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>bootstrap 4 navbar</title>
  <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0"><link rel='stylesheet' href='https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/css/bootstrap.min.css'>
<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.10.2/css/all.css'><link rel="stylesheet" href="./style.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

<style>/* inicio navbar */
@import url('https://fonts.googleapis.com/css?family=Roboto');

body {
	font-family: 'Roboto', sans-serif;
}

* {
	margin: 0;
	padding: 0;
}

i {
	margin-right: 10px;
}

/*----------bootstrap-navbar-css------------*/
.navbar-logo {
	padding: 15px;
	color: #ffffff; /* Blanco */
}

.navbar-mainbg {
	background-color: #3182CE; /* Azul Claro */
	padding: 0px;
}

#navbarSupportedContent {
	overflow: hidden;
	position: relative;
}

#navbarSupportedContent ul {
	padding: 0px;
	margin: 0px;
}

#navbarSupportedContent ul li a i {
	margin-right: 10px;
}

#navbarSupportedContent li {
	list-style-type: none;
	float: left;
}

#navbarSupportedContent ul li a {
	color: #ffffff; /* Blanco para el texto */
	text-decoration: none;
	font-size: 15px;
	display: block;
	padding: 20px 20px;
	transition-duration: 0.6s;
	transition-timing-function: cubic-bezier(0.68, -0.55, 0.265, 1.55);
	position: relative;
}

#navbarSupportedContent > ul > li.active > a {
	color: #2D3748; /* Gris oscuro */
	background-color: transparent;
	transition: all 0.7s;
}

#navbarSupportedContent a:not(:only-child):after {
	content: "\f105";
	position: absolute;
	right: 20px;
	top: 10px;
	font-size: 14px;
	font-family: "Font Awesome 5 Free";
	display: inline-block;
	padding-right: 3px;
	vertical-align: middle;
	font-weight: 900;
	transition: 0.5s;
}

#navbarSupportedContent .active > a:not(:only-child):after {
	transform: rotate(90deg);
}

.hori-selector {
	display: inline-block;
	position: absolute;
	height: 100%;
	top: 0px;
	left: 0px;
	transition-duration: 0.6s;
	transition-timing-function: cubic-bezier(0.68, -0.55, 0.265, 1.55);
	background-color: #ffffff; /* Blanco */
	border-top-left-radius: 15px;
	border-top-right-radius: 15px;
	margin-top: 10px;
}

.hori-selector .right,
.hori-selector .left {
	position: absolute;
	width: 25px;
	height: 25px;
	background-color: #ffffff; /* Blanco */
	bottom: 10px;
}

.hori-selector .right {
	right: -25px;
}

.hori-selector .left {
	left: -25px;
}

.hori-selector .right:before,
.hori-selector .left:before {
	content: '';
	position: absolute;
	width: 50px;
	height: 50px;
	border-radius: 50%;
	background-color: #3182CE; /* Azul Claro */
}

.hori-selector .right:before {
	bottom: 0;
	right: -25px;
}

.hori-selector .left:before {
	bottom: 0;
	left: -25px;
}

@media (min-width: 992px) {
	.navbar-expand-custom {
		-ms-flex-flow: row nowrap;
		flex-flow: row nowrap;
		-ms-flex-pack: start;
		justify-content: flex-start;
	}

	.navbar-expand-custom .navbar-nav {
		-ms-flex-direction: row;
		flex-direction: row;
	}

	.navbar-expand-custom .navbar-toggler {
		display: none;
	}

	.navbar-expand-custom .navbar-collapse {
		display: -ms-flexbox !important;
		display: flex !important;
		-ms-flex-preferred-size: auto;
		flex-basis: auto;
	}
}

@media (max-width: 991px) {
	#navbarSupportedContent ul li a {
		padding: 12px 30px;
	}

	.hori-selector {
		margin-top: 0px;
		margin-left: 10px;
		border-radius: 0;
		border-top-left-radius: 25px;
		border-bottom-left-radius: 25px;
	}

	.hori-selector .left,
	.hori-selector .right {
		right: 10px;
	}

	.hori-selector .left {
		top: -25px;
		left: auto;
	}

	.hori-selector .right {
		bottom: -25px;
	}

	.hori-selector .left:before {
		left: -25px;
		top: -25px;
	}

	.hori-selector .right:before {
		bottom: -25px;
		left: -25px;
	}
}
#logo {
  height: 30px;  /* Ajusta la altura según lo que necesites */
  width: auto;   /* Asegura que el logo mantenga sus proporciones */
}

/* fin de la navbar */
#carouselExampleIndicators .carousel-inner {
    height: 80%; /* Asegura que el contenedor interno del carrusel tenga altura completa */
}

#carouselExampleIndicators .carousel-item {
    height: 80%; /* Asegura que cada item del carrusel ocupe toda la altura */
}

#carouselExampleIndicators .carousel-item img {
    height: 800%; /* La imagen ocupa toda la altura */
    width: 100%; /* La imagen ocupa toda la anchura */
    object-fit: cover; /* Asegura que la imagen se recorte correctamente sin deformarse */
}
body-recuadro {
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 50px;
    background-color: #f8f8f8;
}

h2-recuadro {
    margin-bottom: 20px;
}

.contenedor-recuadro {
    display: flex;
    flex-wrap: wrap;
    justify-content: center; /* Centra los elementos horizontalmente */
    gap: 10px; /* Reduce la separación entre los recuadros */
    max-width: 800px; /* Limita el ancho total */
    margin: 0 auto; /* Centra el contenedor */
}


.opcion-recuadro {
    width: 200px; /* Tamaño uniforme */
    padding: 50px; /* Reduce espacio interno */
    background: ;
    border-radius: 20px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1) ; 
    cursor: pointer;
    transition: transform 0.2s, box-shadow 0.2s;
    text-align: center;
}

.opcion-recuadro:hover {
    transform: translateY(-3px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

.icono-recuadro {
    font-size: 35px; /* Reduce el tamaño del icono */
    color: #007bff;
    margin-bottom: 5px;
}

.titulo-recuadro {
    font-size: 16px;
    margin-bottom: 3px;
}

.descripcion-recuadro {
    font-size: 13px;
    color: #666;
}

</style>

</head>
<body>
<!-- navbar -->
<nav class="navbar navbar-expand-custom navbar-mainbg">

<a class="navbar-brand navbar-logo" href="#">
  <img id="logo" src="https://www.ug.edu.ec/wp-content/uploads/2023/05/cropped-ug-color-horizontal-1-196x43.png" alt="Logo">
</a>

        <button class="navbar-toggler" type="button" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <i class="fas fa-bars text-white"></i>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto">
                <div class="hori-selector"><div class="left"></div><div class="right"></div></div>
                <li class="nav-item">
                    <a class="nav-link" href="javascript:void(0);"><i class="far fa-chart-bar"></i>Ejes Estrategicos</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="javascript:void(0);"><i class="far fa-copy"></i>ODS</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="javascript:void(0);"><i class="far fa-address-book"></i>Contactanos</a>
                </li>
            </ul>
        </div>
    </nav>
<!-- fin de la navbar -->
  <script src='https://code.jquery.com/jquery-3.4.1.min.js'></script>
<script src='https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js'></script>
<script src='https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/js/bootstrap.min.js'></script><script  src="./script.js"></script>
<div class="container mt-5">
    <!-- Carrusel -->

<!-- Fin del Carrusel -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
<div class="d-flex flex-column flex-md-row justify-content-center align-items-center text-center" style="height: 22vh; width: 100%; padding: 20px;">
  <!-- Imagen -->
  <img src="https://campusnivelacion.ug.edu.ec/pluginfile.php/1/core_admin/logocompact/300x300/1731967065/logo-192x192%281%29%281%29.png" 
  alt="Imagen" width="100" height="100" class="me-3">
  <!-- Línea divisoria -->
  <div style="height: 100px; width: 2px; background-color: #3182ce;"></div> 	

  <!-- Texto a la derecha -->
  <p class="ms-4 mb-0" style="max-width: 60%; color: #333333; font-size: 1.1em; line-height: 1.6;">
    La Universidad de Guayaquil es una universidad pública localizada en la ciudad de Guayaquil en la República del Ecuador. Es la universidad más grande del país y la más antigua de la ciudad, además de tener seis extensiones universitarias en varias partes del país.
  </p>
</div>

<div class="d-flex flex-column justify-content-center align-items-center text-center" style="height: 28vh; padding: 20px;">
  <!-- Título en negrita -->
  <p class="mb-3" style="color: #203c6d; font-weight: bold; font-size: 1.5em; text-transform: uppercase;">Misión.</p>

  <!-- Texto debajo del título centrado -->
  <div class="text-center" style="max-width: 80%; color: #000000; font-size: 1.1em; line-height: 1.6;">
    La Universidad de Guayaquil es una universidad pública localizada en la ciudad de Guayaquil en la República del Ecuador. Es la universidad más grande del país y la más antigua de la ciudad, además de tener seis extensiones universitarias en varias partes del país.
  </div>
</div>
<hr style="border: 1px solid #3182ce; width: 100%; margin: 20px auto;">
<body class="body-recuadro">
    <h2 class="h2-recuadro">Selecciona una opción para comenzar</h2>

<div class="contenedor-recuadro">
    <!-- Primera fila -->
    <div class="opcion-recuadro">
        <i class="fa fa-file icono-recuadro"></i>
        <h3 class="titulo-recuadro">Sitio en Blanco</h3>
        <p class="descripcion-recuadro">Construye un sitio desde cero</p>
    </div>
    <div class="opcion-recuadro">
        <i class="fa fa-th-large icono-recuadro"></i>
        <h3 class="titulo-recuadro">Plantilla</h3>
        <p class="descripcion-recuadro">Empieza con un diseño predefinido</p>
    </div>
    <div class="opcion-recuadro">
        <i class="fa fa-play-circle icono-recuadro"></i>
        <h3 class="titulo-recuadro">Tutorial</h3>
        <p class="descripcion-recuadro">Aprende lo básico con una guía</p>
    </div>

    <!-- Segunda fila -->
    <div class="opcion-recuadro">
        <i class="fa fa-th-large icono-recuadro"></i>
        <h3 class="titulo-recuadro">Plantilla</h3>
        <p class="descripcion-recuadro">Empieza con un diseño predefinido</p>
    </div>
    <div class="opcion-recuadro">
        <i class="fa fa-th-large icono-recuadro"></i>
        <h3 class="titulo-recuadro">Plantilla</h3>
        <p class="descripcion-recuadro">Empieza con un diseño predefinido</p>
    </div>
    <div class="opcion-recuadro">
        <i class="fa fa-play-circle icono-recuadro"></i>
        <h3 class="titulo-recuadro">Tutorial</h3>
        <p class="descripcion-recuadro">Aprende lo básico con una guía</p>
    </div>
</div>








</body>
<!-- Footer -->
<div class="container">
  <footer class="d-flex flex-wrap justify-content-between align-items-center py-3 my-4 border-top">
    <p class="col-md-4 mb-0 text-body-secondary">&copy; 2025 J.JTech Company </p>
	<a href="/" class="col-md-4 d-flex align-items-center justify-content-center mb-3 mb-md-0 me-md-auto link-body-emphasis text-decoration-none">
  <img src="https://campusnivelacion.ug.edu.ec/pluginfile.php/1/core_admin/logocompact/300x300/1731967065/logo-192x192%281%29%281%29.png" alt="Logo" width="80" height="80">
</a>
<ul class="nav">
  <li class="nav-item">
    <a href="https://instagram.com/tu_usuario" class="nav-link px-2 text-body-secondary" target="_blank" rel="noopener">
      <i class="fab fa-instagram" style="font-size: 22px;"></i>
    </a>
  </li>
  <li class="nav-item">
    <a href="https://www.tiktok.com/@tu_usuario" class="nav-link px-2 text-body-secondary" target="_blank" rel="noopener">
      <i class="fab fa-tiktok" style="font-size: 22px;"></i>
    </a>
  </li>
  <li class="nav-item">
    <a href="https://www.facebook.com/tu_usuario" class="nav-link px-2 text-body-secondary" target="_blank" rel="noopener">
      <i class="fab fa-facebook" style="font-size: 22px;"></i>
    </a>
  </li>
  <li class="nav-item">
    <a href="https://www.twitter.com/tu_usuario" class="nav-link px-2 text-body-secondary" target="_blank" rel="noopener">
      <i class="fab fa-twitter" style="font-size: 22px;"></i>
    </a>
  </li>
</ul>


  </footer>
</div>
<!-- Fin del Footer -->

<script>
    // ---------Responsive-navbar-active-animation-----------
function test(){
	var tabsNewAnim = $('#navbarSupportedContent');
	var selectorNewAnim = $('#navbarSupportedContent').find('li').length;
	var activeItemNewAnim = tabsNewAnim.find('.active');
	var activeWidthNewAnimHeight = activeItemNewAnim.innerHeight();
	var activeWidthNewAnimWidth = activeItemNewAnim.innerWidth();
	var itemPosNewAnimTop = activeItemNewAnim.position();
	var itemPosNewAnimLeft = activeItemNewAnim.position();
	$(".hori-selector").css({
		"top":itemPosNewAnimTop.top + "px", 
		"left":itemPosNewAnimLeft.left + "px",
		"height": activeWidthNewAnimHeight + "px",
		"width": activeWidthNewAnimWidth + "px"
	});
	$("#navbarSupportedContent").on("click","li",function(e){
		$('#navbarSupportedContent ul li').removeClass("active");
		$(this).addClass('active');
		var activeWidthNewAnimHeight = $(this).innerHeight();
		var activeWidthNewAnimWidth = $(this).innerWidth();
		var itemPosNewAnimTop = $(this).position();
		var itemPosNewAnimLeft = $(this).position();
		$(".hori-selector").css({
			"top":itemPosNewAnimTop.top + "px", 
			"left":itemPosNewAnimLeft.left + "px",
			"height": activeWidthNewAnimHeight + "px",
			"width": activeWidthNewAnimWidth + "px"
		});
	});
}
$(document).ready(function(){
	setTimeout(function(){ test(); });
});
$(window).on('resize', function(){
	setTimeout(function(){ test(); }, 500);
});
$(".navbar-toggler").click(function(){
	$(".navbar-collapse").slideToggle(300);
	setTimeout(function(){ test(); });
});



// --------------add active class-on another-page move----------
jQuery(document).ready(function($){
	// Get current path and find target link
	var path = window.location.pathname.split("/").pop();

	// Account for home page with empty path
	if ( path == '' ) {
		path = 'index.html';
	}

	var target = $('#navbarSupportedContent ul li a[href="'+path+'"]');
	// Add active class to target link
	target.parent().addClass('active');
});




// Add active class on another page linked
// ==========================================
// $(window).on('load',function () {
//     var current = location.pathname;
//     console.log(current);
//     $('#navbarSupportedContent ul li a').each(function(){
//         var $this = $(this);
//         // if the current path is like this link, make it active
//         if($this.attr('href').indexOf(current) !== -1){
//             $this.parent().addClass('active');
//             $this.parents('.menu-submenu').addClass('show-dropdown');
//             $this.parents('.menu-submenu').parent().addClass('active');
//         }else{
//             $this.parent().removeClass('active');
//         }
//     })
// });
</script>
</html>

