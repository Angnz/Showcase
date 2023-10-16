---
permalink: /ssc/
layout: page
title: ":Simple showcase"
---
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #1F4172;
        margin: 2em;
        padding: 1em;
    }
    
    .site-header, .footer-heading{ /*site-header is the Webpage Banner and  text*/
        Color: #132043;
        font-family: Arial, sans-serif;
        background-color: #363062;
        color:#F99417;
        border-top:0px;
        border-bottom: 0px;
        
    }
    
    .site-title, .site-title:visited {
        color: #F99417;
    }
    
    .site-title:hover {
        text-decoration: none;
    }
    
    .site-nav .page-link{
        font-family: 'Courier New', Courier, monospace;
        color: #F99417;
        line-height: 1.5;
    }
    
    a {
        color: #FDF0F0;
    }
    
    a:visited {
        color: #00FF00;
    }
    
    .page-content{
        font-family: 'Courier New', Courier, monospace;
        color: #FDF0F0;
        line-height: 1.5;
        overflow-x: auto;
    }

     pre, code {
      background-color: transparent;
      color: black;
      font-family: 'Courier New', monospace;
      }

    </style>

<hr>

## With this Simple Showcase is possible to view products, choose from a cart, request a price and send a quotation.
In this minimalist WordPress showcase, products are displayed, and users can interact by selecting items from a shopping cart, soliciting pricing information, and initiating the quotation process. The system relies on Contact Form 7 for form generation, while the essential CSS and JavaScript resources are enqueued and invoked from the functions.php file to ensure the link betweee styling and interactive behavior. Automated updates might break the links in functions.php

## HTML

Explain Skeleton
{% highlight html %}
<!-- GRUPO Productos -->

<div id="seccion1_id" class="seccion1">
    <h3 class="categoria_productos">Porcelana Fría</h3>
    <div class="">
        <p>Los productos hechos en porcelana fría son delicados y detallados, ideales para decorar cualquier espacio del hogar u oficina.</p>
    </div>
    <div id="categoria1">
    </div>

    <h3 class="categoria_productos">Foamy</h3>
    <div class="">
        <p>
            Los productos hechos en Foamy son coloridos, divertidos y versátiles. Estos artículos pueden ser utilizados para decorar, para manualidades, como souvenirs y regalos. Estas manualidades son únicas y hechas a mano, lo que significa que cada pieza es única y personalizada.
        </p>
    </div>
    <div id="categoria2">
    </div>

    <h3 class="categoria_productos">Novios</h3>
    <p>
            texto para Novios DESCRIPCION
        </p>
    <div id="categoria3">
    </div>

     



</div> <!-- seccion1 End -->
<!-- Productos END-->


<div id="seccion2_id" class="seccion2">

<!-- ELEJIR SI DESEA ENVIO O NO -->
<h3 class="categoria_productos">servicios</h3>
       <p>
            texto para Servicios DESCRIPCION
        </p>
    <div id="categoria4">
    </div>



    <h2 id="datosdecontacto"><a href="#datosdecontacto">2. Sus datos de contacto</a></h2>

    <!-- Datos Personales-->
    <label> <b>Nombre</b> (Requerido)
        [text* your-name placeholder "Nombre"] </label>

    <label> <b>Apellido</b> (Requerido)
        [text* apellido placeholder "Apellido"]</label>

    <label> <b>Email</b> (Requerido)
        [email* your-email placeholder "nombre@ejemplo.com"] </label>

    <label> <b>Telefono</b> (Requerido)
        <i class="nota">*No olvide su código de país</i>
        [tel* telefono placeholder "ejemplo: +56 123456789 "]
    </label>

    <label> <b>Fecha aproximada para el pedido? </b>(Opcional)
        <i class="nota">*Atención en la disponibilidad de la agenda para los pedidos</i>
        [date date-531 min:45days ]
    </label>

    <!-- Datos delivery-->
    <!-- <h2 id="enviarpedido"><a href="#enviarpedido">3. Enviar Pedido</a></h2> -->
   
    <!-- Delivry as a product -->
    <!-- <h3 class="categoria_productos">Envio</h3> -->
    <!-- <div id="categoria4"></div> -->

    <!-- <div><p class="envio_msg" id="mensaje-envio"></p></div> -->
    <!-- Datos delivery END-->

</hr>
    <!-- Info for Delivery -->
    <b>Datos para la entrega del pedido (Nacional)</b>
    <label>Calle (Requerido)<br>
        [text* calle id:adress_calle]</label>
    <label>Numero (Requerido)<br>
        [text* numero id:adress_numero]</label>
    <label>Comuna (Requerido)<br>
        [text* comuna id:adress_comuna]</label>
    <label>Código postal (Requerido)<br>
        [text* ciudad id:adress_codigo]</label>
    <label>Ciudad (Requerido)<br>
        [text* ciudad id:adress_ciudad]</label>    
    <label>Región (Requerido)<br>    
        [select* region id:id:adress_region "Región de Tarapacá " "Región de Antofagasta " "Región de Atacama " "Región de Coquimbo " "Región de Valparaíso " "Región Metropolitana de Santiago " "Región del Libertador General Bernardo O’Higgins " "Región del Maule " "Región del Ñuble " "Región del Biobío " "Región de La Araucanía " "Región de Los Ríos " "Región de Los Lagos " "Región de Aysén del General Carlos Ibáñez del Campo " "Región de Magallanes y la Antártica Chilena"]</label>
    <label>País (Requerido)<br>
        [text* adress_pais readonly "Chile"]</label>


    <label>Indicaciones adicionales para la entrega<br>
        [textarea additional-instructions x2]</label><br>


    <!-- Datos delivery END-->
    <!-- Datos Personales END-->


            <div id="tocheckout_id">
                <p class="enviar_Panel">Siguiente</p>
            </div>
</div><!-- seccion2 End -->



    <div id="seccion3_id" class="seccion3">

<h2 id="checkout"><a href="#checkout">3. Enviar el pedido</a></h2>

        <label>
            <b>Le gustaría recibir E-mails (Newsletters) con futuras promociones e infromación de Petita Ideas...?
            </b></label>
        </br>
        [radio radio-175 use_label_element default:2 "Si, me gustaría recibir E-mails con futuras promociones e información de Petita Ideas..." "No, no deseo recibir futuras promociones e información de Petita Ideas a mi dirección de correo electrónico"]

        <label> <b>Envienos un mensaje</b>
            [textarea your-message minlength:5 maxlength:300 x1 placeholder "Ejemplo: EL producto 2.1 tiene me gustaría en rojo..."]</label>
        [count your-message down ]



        <label>
            [acceptance acceptance-31] He leído y acepto las <a href="http://petitaideas.com/privacy-policy/"
                target="_blank">políticas de privacidad</a> [/acceptance]<p><i class="nota">Recivirá un email de confirmación con su pedido (revise su carpeta de "SPAM"). La finalidad de la información recopilada se limita exclusivamente a la comunicación entre el cliente y Petita Ideas. Para más detalles visite nuestra páguina de <a href="http://petitaideas.com/politica-de-privacidad-espanol/" target="_blank">políticas de privacidad</a>. sección: "Sus datos de contacto"</i></p></label>


           <div id="atras_id"><p class="enviar_Panel">volver a datos de contácto</p></div>           
            <div> 


                    <p style="display: none !important;"><label>&#916;<textarea name="_wpcf7_ak_hp_textarea" cols="45" rows="8" maxlength="100"></textarea></label><input type="hidden" id="ak_js_1" name="_wpcf7_ak_js"value="181" />
                     <script>document.getElementById("ak_js_1").setAttribute("value", (new Date()).getTime());</script></p>

                    <div class="wpcf7-response-output" aria-hidden="true"></div>
                    <label>[submit "Enviar"]</label>
                    <!-- sección final END -->


            </div>


    </div><!-- seccion3 End -->


                    [textarea Listadecarritoemail id:listacarrito 3x8 readonly hidden ]
                    [textarea Totaldelcarrito id:ListaCarritoTotal 3x1 readonly hidden ]



<div class="carrito-float">
    <!-- Carrito Flotante -->
    <a id="boton-carrito" href=#><img id="carritoIcon" class="carritoCompra" src="http://petitaideas.com/wp-content/uploads/2023/05/shopping-bag-color-icon.png" alt="carrito de compra">

    <i class="fas fa-shopping-cart"></i>

    <span class="num-items"></span>
    </a>
</div>



<div id="panel-carrito">
    <!-- PANEL CARRITO -->
    <!-- Carrito de compras -->
    <div class="carritoStyle">
        <div class="header_carrito">
            <h2>Carrito de compras</h2>
        </div>
        <div class="productos_en_carrito"><ul id="carrito"></ul></div>  
        <div id="seccioncarrito_id" class="seccioncarrito">
            <b>Total: CLP<span id="total"></span></b>
            (Total en Pesos Chilenos)
            
            <!-- Carrito de compras END-->
            <div id="cerrarPanel_id">
                <p class="cerrarPanel">Volver a la tienda</p>
            </div>
            <div id="enviarPanel_id">
                <p class="enviar_Panel">Datos de contácto</p>
            </div>
        </div>
    </div>
</div>
{% endhighlight %}


## PHP
Explanation PHP

```
/*My Code for online shop - To add in functions.php in wordpress*/


function function_css() {
    // Enqueue the CSS file
    wp_enqueue_style('function_css', '/wp-includes/css/custom-css/yourcss.css');
}
add_action('wp_enqueue_scripts', 'petitaideas_os_css');


function function_css() {
    // Check if the current page is the "test" page
    if (is_page('yourpageid')) {
        // Enqueue the script only if the current page is "test"
        wp_register_script('function_css', '/wp-includes/js/custom-scripts/yourjs.js', array('jquery'), '1', true );
        wp_enqueue_script('function_css');
    }
}
add_action('wp_enqueue_scripts','function_css');


/*My Code for online shop END*/
```



## JS

Explain JS
```
//----------------------------------------------
// 1.-Productos y CAtegorias
//----------------------------------------------



/*version 2 con precio formateado*/
  
let carrito = [];
let checkiVacio;
const productos = [
  {
    nombre: "Porcelana <br > Rapunzel",
    precio: 30000,
    imagen: "",
    descripcion: "Figura de porcelana fría de Rapunzel, detallada y delicada, ideal para decorar habitaciones de cuentos de hadas.<br><br>Altura: 15cm<br>Peso: 400grm<br>Base decorativa no incluida",
    categoria: 1
  },
  {
    nombre: "Porcelana <br > Mujer costurera",
    precio: 20000,
    imagen: "",
    descripcion: "Figurita de porcelana fría de una mujer sentada frente a una máquina de coser, con detalles realistas y colores vivos.<br><br>Altura: 10cm<br>Peso: 400grm<br>Base decorativa no incluida",
    categoria: 1
  },
  {
    nombre: "Porcelana <br > Novios",
    precio: 19990,
    imagen: "",
    descripcion: "Novios en porcelana<br>12cm<br>Base no incluida",
    categoria: 1
  },
  {
    nombre: "Producto 2.1 <br > Product Name",
    precio: 15500,
    imagen: "",
    descripcion: "Descripción del producto 3",
    categoria: 2
  },
  {
    nombre: "Producto 2.2 <br > Product Name",
    precio: 12500,
    imagen: "",
    descripcion: "Descripción del producto 4",
    categoria: 2
  },
  {
    nombre: "Producto 2.3 <br > Product Name",
    precio: 6000,
    imagen: "",
    descripcion: "Descripción del producto 6",
    categoria: 2
  },
  {
    nombre: "Foamy <br > Product Name",
    precio: 10500,
    imagen: "",
    descripcion: "Descripción del producto 5",
    categoria: 3
  },
  {
    nombre: "Porcelana <br > Product Name",
    precio: 13550,
    imagen: "",
    descripcion: "Novios en porcelana<br>12cm<br>Base no incluida",
    categoria: 3
  },
  {
    nombre: "*Envio por Correo (Nacional)*",
    precio: 6000,
    imagen: "",
    descripcion: "Se envia a todo el territorio nacional<br >El precio del envio se paga junto con el total<br > ",
    categoria: 4
  }

];

// Agregar productos a sus categorías
productos.forEach(producto => {
  let productoHTML = `<div>
      <h3 class="nombre_producto">${producto.nombre}</h3>
      <img class="img_producto" src="${producto.imagen}" alt="${producto.nombre}">
      <p class="descripcion_producto">${producto.descripcion}</p>
      <p class="precio_producto">Precio CLP: $${producto.precio.toLocaleString()}</p>
      <button onclick="agregarProducto(event, '${producto.nombre}', ${producto.precio},'${producto.imagen}')">Agregar al carrito</button>
<p class="info_producto">CLP = PESO CHILENO</p>
  </div>`;
  switch (producto.categoria) {
    case 1:
      document.getElementById("categoria1").innerHTML += productoHTML;
      break;
    case 2:
      document.getElementById("categoria2").innerHTML += productoHTML;
      break;
    case 3:
      document.getElementById("categoria3").innerHTML += productoHTML;
      break;
    case 4:
      document.getElementById("categoria4").innerHTML += productoHTML;
      break;
    default:
      break;
  }
});

//----------------------------------------------
// 2.-AGREGAR PRODUCTO AL CARRITO / Carrito
//----------------------------------------------

const agregarProducto = (event, nombre, precio, imagen) => {
    event.preventDefault();
 
    if (nombre === "*Envio por Correo (Nacional)*") {

    // Verificar si el producto ya está en el carrito
    const productoExistente = carrito.find(producto => producto.nombre === nombre);
    if (productoExistente) {
      // Mostrar el mensaje de envío
      const mensajeEnvio = document.getElementById("mensaje-envio");
      mensajeEnvio.textContent = "Aviso: El envío ya se ha agregado! Revise su carrito de compras.";
      mensajeEnvio.style.display = "block";
      // Ocultar el mensaje después de 3 segundos
      setTimeout(() => {
        mensajeEnvio.style.display = "none";
      }, 3000);
      return;
    }
  }

  carrito.push({ nombre, precio, imagen });
    actualizarCarrito();

  // Agregar clase al botón
  // event.target.classList.add("btn-agregar");
  // Eliminar clase después de un tiempo
  // setTimeout(() => {
  //   event.target.classList.remove("mensaje-envio")
  // }, 500);

};


//----------------------------------------------
// 3.-FUNCIONES DE ACTUALIZACION CARRITO
//----------------------------------------------
// Declara la variable checkiVacio fuera de la función actualizarCarrito para almacenar total de manera global
const actualizarCarrito = () => {
  let lista = "";
  let total = 0;

  // Ordfena lis productos alfabeticamente
  carrito.sort((a, b) => a.nombre.localeCompare(b.nombre));
  for (let i = 0; i < carrito.length; i++) {
    lista += `<li> <img src="${carrito[i].imagen}" width="50px"><div id="prod_nomebrecarrito">${carrito[i].nombre}</div> <div id="prod_precioencarrito">$${formatearNumero(carrito[i].precio)}</div> <button onclick='quitarProducto(${i})'>Quitar</button></li>`;
    total += carrito[i].precio; 
  }

  document.getElementById("carrito").innerHTML = lista;
  document.getElementById("total").innerHTML = `$${formatearNumero(total)}`;

  // toma el valor de total
  checkiVacio = total;

  // Actualizar la lista de carrito en el formulario de contacto
  actualizarListaCarrito();
  actualizarListaCarritoTotal(total);

  //muestra el contenido de Total
   // window.alert();

  //Check si el carrito esta vacio, asi depliega el boton de Enviar pedido
  if (checkiVacio === 0) {
    enviarPanel.classList.add('esconder');
    //window.alert('Carrito está vacío');
  } else {
    enviarPanel.classList.remove('esconder');
  }

};


//actializar Lista en el formulario
const actualizarListaCarrito = () => {
    let lista = "";
  for (let i = 0; i < carrito.length; i++) {
    lista += `${carrito[i].nombre} - $${carrito[i].precio.toLocaleString()}\n`;
  }
  document.getElementById("listacarrito").value = lista;
}


//actializar total en el formulario
const actualizarListaCarritoTotal = (total) => {
  document.getElementById("ListaCarritoTotal").value = `$${formatearNumero(total)}`;
  // Actualizar el número de artículos en el carrito al cargar la página
  actualizarNumItems();
};


// Mostrar el número de artículos en el carrito
function actualizarNumItems() {
  const numItems = carrito.length;
  const numItemsEl = document.querySelector('.num-items');
  numItemsEl.innerText = numItems;
  //sacudir el carrito cuando se agrega un numero
}


// Agrego formato al precio
const formatearNumero = (numero) => {
  return new Intl.NumberFormat('es-CL', { style: 'decimal', minimumFractionDigits: 0, maximumFractionDigits: 2 }).format(numero);
};


//----------------------------------------------
// 4. panel carruito
//----------------------------------------------

// quitar producto
const quitarProducto = (index) => {
  carrito.splice(index, 1);
  actualizarCarrito();   
};

var botonCarrito = document.getElementById('boton-carrito');
var panelCarrito = document.getElementById('panel-carrito');
var cerrarPanel = document.getElementById('cerrarPanel_id');
var enviarPanel = document.getElementById('enviarPanel_id');
var tocheckout_btn = document.getElementById('tocheckout_id');
var todatoscontacto_btn = document.getElementById('atras_id');

// Seleccionar secciones 1, 2, 3
 const seccion1 = document.querySelector('#seccion1_id');
 const seccion2 = document.querySelector('#seccion2_id');
 const seccion3 = document.querySelector('#seccion3_id');

 seccion1.style.display = 'block';
 seccion2.style.display = 'none';
 seccion3.style.display = 'none';


// Boton carrito. Funciones al click

botonCarrito.addEventListener('click', function (e) {
  e.preventDefault();
  actualizarCarrito();

   // Actualizo carrito para que apareca con valor 0
  panelCarrito.classList.toggle('mostrar');
  
  if (panelCarrito.classList.contains('mostrar')) {
    document.body.style.overflow = 'hidden';
  } else { 
    document.body.style.overflow = 'initial';
  }

  

});

// Al cerrar el panel, que vuelva a la tienda online y active el scrolling
cerrarPanel.addEventListener('click', function (e) {
  panelCarrito.classList.toggle('mostrar');
  document.body.style.overflow = 'initial';
  seccion1.style.display = 'block';
  seccion2.style.display = 'none';
  seccion3.style.display = 'none';
  // seccion1.scrollIntoView({ behavior: 'smooth' });

});

// Este aplica a cunando precionas el boton "enciar pedido" naranjo
enviarPanel.addEventListener('click', function (e) {
  panelCarrito.classList.toggle('mostrar');
  document.body.style.overflow = 'initial';
  seccion1.style.display = 'none';
  seccion2.style.display = 'block';
  seccion3.style.display = 'none';
  seccion2.scrollIntoView({ behavior: 'smooth' });
  
});

// Al precoionar el btn de "Atrás" en el check out
todatoscontacto_btn.addEventListener('click', function (e) {
  // panelCarrito.classList.toggle('mostrar');
  // document.body.style.overflow = 'initial';
  seccion1.style.display = 'none';
  seccion2.style.display = 'block';
  seccion3.style.display = 'none';
  seccion2.scrollIntoView({ behavior: 'smooth' });
  
});

// Al precoionar el btn de proceder a check out
tocheckout_btn.addEventListener('click',function(e){

  seccion1.style.display = 'none';
  seccion2.style.display = 'none';
  seccion3.style.display = 'block';
  seccion3.scrollIntoView({ behavior: 'smooth' });
});





actualizarCarrito();

// Animar boton feedback
const btnAgregar = document.querySelector('.btn-agregar');
btnAgregar.addEventListener('click', () => {
  btnAgregar.classList.add('shake');
  setTimeout(() => {
    btnAgregar.classList.remove('shake');
  }, 100);
});


```


## CSS

Explain CSS
```
/* CSS para pantallas grandes */

@media screen and (min-width: 640px) {

  #categoria1,
  #categoria2,
  #categoria3,
  #categoria4 {
    display: flex;
    flex-wrap: wrap;
    justify-content: left;
  }

  #categoria1>div,
  #categoria2>div,
  #categoria3>div,
  #categoria4>div {
    background-color: whitesmoke;
    margin: 5px;
    padding: 5px;
    text-align: center;
    flex-basis: calc(33.33% - 20px);
  }
}


/* quitar la flecha hacia arriba */
.back-to-top {
  display: none;
}


/*VISTA EN MOVILES*/

/* quitar la flecha hacia arriba */
.back-to-top {
  display: none;
}

@media screen and (max-width: 640px) {

  #categoria1,
  #categoria2,
  #categoria3,
  #categoria4 {

    flex-wrap: wrap;
    justify-content: left;
  }

  #categoria1>div,
  #categoria2>div,
  #categoria3>div,
  #categoria4>div {
    background-color: whitesmoke;
    margin: 5px;
    padding: 5px;
    text-align: center;
    flex-basis: calc(33.33% - 20px);
  }

  .img_producto {

    width: 350px;
  }

}


/* ESTILO NOMBRES Y TITULOS PRODUCTOS */
.categoria_productos {
  font-size: 40px;
}

.nombre_producto {
  font-size: 20px;
}

.descripcion_producto {
  margin-top: 10px;
  padding: 5px;
}

.precio_producto {
  font-weight: bold
}




/* Estilos para el carrito */

.subrajado {
  border-bottom: 1px solid black;
  padding-bottom: 10px;
}

#carrito {
  padding 10px;
  margin-bottom: 20px;
}

#carrito li {
  margin-bottom: 10px;
  display: flex;
  justify-content: space-between;
}

#prod_precioencarrito{

}


#carrito button {
  background-color: orangered;
  color: white;
  border: none;
  padding: 5px;
  cursor: pointer;
  font-weight: bold
}


/*Estilo para el boton agregar al carrito*/
#btn_product {

font-size: 50px;
/* background-color: red; */
/*osition: absolute;*/
/* bottom: 0; */
}

.info_producto {
  font-style: italic;
  color: gray;
  font-size: 12px;
}


/* Estilos para el total */
#total {
/*  border-bottom: solid 1px green;*/
  font-weight: bold;
  font-size: 20px;
  color: green;
}


/* Estilos para la lista de carrito en el formulario */
#listacarrito,
#ListaCarritoTotal {
  background-color: whitesmoke;
  display: flex;
  flex-wrap: wrap;
  flex-basis: calc(33.33% - 20px);
  display: none;
/*  visibility: hidden;*/
  border: white;
}

/*  .btn-agregar {
  background-color: #2ecc71;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
  transition: all 0.1s ease-in-out;
  animation: shake 0.2s;
}*/

/*.btn-agregar:hover {
  background-color: #27ae60;
}
*/

/*Carrito aflotante*/

.carrito-float {
  position: fixed;
  bottom: 20px;
  right: 30px;
  z-index: 8888;
}

.carrito-float a {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 50px;
  height: 50px;
  background-color: transparent;
  border-radius: 50%;
  color: transparent;
  font-size: 24px;
  text-decoration: none;

}

.carrito-float a:hover {
  background-color: transparent;
  text-decoration: none;


}

/*.shake-animation {
  animation: shake 0.2s;
  animation-iteration-count: 2s;
}

@keyframes shake {
  0% {
    transform: rotate(0deg);
  }

  25% {
    transform: rotate(5deg);
  }

  50% {
    transform: rotate(0eg);
  }

  75% {
    transform: rotate(-5deg);
  }

  100% {
    transform: rotate(0deg);
  }
}
*/

/* Los numeros de la bolsita de compras */
.num-items {
  position: absolute;
  top: 0;
  right: 0;
  background-color: #F00;
  color: #fff;
  font-size: 14px;
  font-weight: bold;
  width: 20px;
  height: 20px;
  line-height: 20px;
  text-align: center;
  border-radius: 50%;
}

/*MENU ENVIO*/

#mensaje-envio {
  flex-wrap: wrap;
  justify-content: left;
  color: darkorange;
  display: none;
}

.envio_msg {

  padding-top: 10px;
  padding-left: 5px;
  border-left: solid 1px darkorange;

}

/*MENU CARRITO FLOTANTE*/



#panel-carrito {
  transition: right 0.3s ease;
  position: fixed;
  top: 0;
  right: -90%;  
  width: 90%;
  height: 100%;
  padding-left: 0px;
  background-color: #fff;
  z-index: 9999;
}

.header_carrito{
  padding-left:20px ;
  z-index: 9999;
  height: 10vh; /* 33% del alto de la ventana */
  width: 100%; /* Ancho al 100% de la ventana */
  overflow-y: auto; /* Scroll vertical */
  background-color: white; 
  box-sizing: border-box;   
  }

.productos_en_carrito{
  padding-top: 10px;
  background-color: red;
  height: 60vh; /* 33% del alto de la ventana */
  width: 100%; /* Ancho al 100% de la ventana */
  overflow-y: auto; /* Scroll vertical */
  overscroll-behavior: contain;
  background-color: white; 
  border: 1px solid #ddd;
  z-index: 9999;
}


.seccioncarrito{
/*  Seccion donde va elprecio y los botones para volver y proseguir*/
  
  position: absolute;
  background: rgb(251,251,251);
  background: -moz-linear-gradient(0deg, rgba(251,251,251,1) 0%, rgba(255,255,255,1) 88%, rgba(0,0,0,0) 100%);
  background: -webkit-linear-gradient(0deg, rgba(251,251,251,1) 0%, rgba(255,255,255,1) 88%, rgba(0,0,0,0) 100%);
  background: linear-gradient(0deg, rgba(251,251,251,1) 0%, rgba(255,255,255,1) 88%, rgba(0,0,0,0) 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#fbfbfb",endColorstr="#000000",GradientType=1);
  margin: 0px;
  bottom:0%;
  width: 100%;
  height: 23vh; /* 33% del alto de la ventana */
  padding-left: 10px;
  z-index: 9999;
}

#panel-carrito.mostrar {
  background-color: white;
  border-left: solid 1px lightgrey;
/*  padding-left: 20px;*/
/*  padding-right: 10px;*/
  right: 0;
}

.carritoStyle li {
  font-size: 1em;
  border-bottom: solid 1px lightgrey;
}

#boton-carrito {
  position: relative;
}

#boton-carrito .num-items {
  position: absolute;
  top: -5px;
  right: -5px;
  background-color: #f00;
  color: #fff;
  font-size: 12px;
  width: 18px;
  height: 18px;
  line-height: 18px;
  text-align: center;
  border-radius: 50%;
}

.custom-logo {
  width: 20px;
}

#cerrarPanel_id,
#enviarPanel_id {
  cursor: pointer;
  }


/*Articulos en el panel*/

ul#carrito li #prod_nomebrecarrito {
  justify-content: right;
  text-align: left;

/*  background-color: greenyellow;*/
}

#prod_precioencarrito{
/*  margin-left: 10px;
 /*justify-content: right;
  flex-wrap: right;*/
/*   background-color: greenyellow;*/
}

#prod_nomebrecarrito{
/*  margin-right: 5px;*/
/*  text-align: left;*/
/*   background-color: powderblue;*/
}

.cerrarPanel {
  background: linear-gradient(to right, #196BCA, #6433E0);
  background-color: #196BCA;
  color: #fff;
  font-family: Trebuchet MS;
  font-size: 18px;
  font-weight: 800;
  font-style: normal;
  text-decoration: none;
  margin-bottom: 5px;
  padding: 10px 10px;
  border: 0px solid #000;
  border-radius: 10px;
}

.enviar_Panel {

  background: linear-gradient(to right, #f12711, #f5af19);
  background-color: #196BCA;
  color: #fff;
  font-family: Trebuchet MS;
  font-size: 18px;
  font-weight: 800;
  font-style: normal;
  text-decoration: none;
  padding: 10px 10px;
  border: 0px solid #000;
  border-radius: 10px;
  cursor: pointer;
}

.esconder {
 visibility: hidden;
 background-color: lightblue;
  }


/*BTN snimacion feedback*/
.shake {
  animation: shake 0.2s;
}




/*

FUTURO ESTILO DE BOTONES
#button{

 background: linear-gradient(to right,#6433e0 ,#196bca);
 background-color: #6433e0;
 color: #fff;
 font-family: Trebuchet MS;
 font-size: 18px;
 font-weight: 800;
 font-style: normal;
 text-decoration: none;
 padding: 14px 15px;
 border: 0px solid #000;
 border-radius: 10px;
 display: inline-flex;
 justify-content: center;
 align-items: center;

}

*/

.button-swing {
  color: #65b5f6;
  background-color: transparent;
  border: 1px solid #65b5f6;
  border-radius: 4px;
  padding: 0 16px;
  cursor: pointer;
  transition: all 0.2s ease-in-out;
}

.button-swing:focus {
  animation: swing 1s ease;
  animation-iteration-count: 1;
}

@keyframes swing {
  0% { transform: translate(0, 0) rotate(0deg); }
  25% { transform: translate(5px, 5px) rotate(5deg); }
  50% { transform: translate(0, 0) rotate(0eg); }
  75% { transform: translate(-5px, 5px) rotate(-5deg); }
  100% { transform: translate(0, 0) rotate(0deg); }
}



/* ----------------------------------------------
 * Generated by Animista on 2023-8-21 18:59:28
 * Licensed under FreeBSD License.
 * See http://animista.net/license for more info. 
 * w: http://animista.net, t: @cssanimista
 * ---------------------------------------------- */

/**
 * ----------------------------------------
 * animation rotate-hor-center
 * ----------------------------------------
 */


 .rotate-hor-center{animation:rotate-hor-center .5s cubic-bezier(.455,.03,.515,.955) both}
 
@-webkit-keyframes rotate-hor-center {
  0% {
    -webkit-transform: rotateX(0);
            transform: rotateX(0);
  }
  100% {
    -webkit-transform: rotateX(-360deg);
            transform: rotateX(-360deg);
  }
}
@keyframes rotate-hor-center {
  0% {
    -webkit-transform: rotateX(0);
            transform: rotateX(0);
  }
  100% {
    -webkit-transform: rotateX(-360deg);
            transform: rotateX(-360deg);
  }
}

```



[Download the files hier](https://github.com/Angnz/PI_OS.git) 

https://github.com/Angnz/PI_OS.git)
