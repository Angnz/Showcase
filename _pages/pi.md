---
permalink: /pi/
layout: page
title: PI
---

# Product showcase. 
## In this very simple Showcase it is possible to view products, choose from a cart, request a price and send a quotation.

##HTML
Explain Skeleton
```

```

##CSS
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

##JS
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