# Reto 10

## Requerimientos
1. Crea una estructura HTML básica para la página de inicio de la tienda de ropa, con un encabezado, una sección principal, un pie de página y algunos elementos dentro de cada sección.
2. Agrega algunas imágenes de productos y el logotipo de la tienda.
3. Utiliza CSS para dar estilo a la página de la siguiente manera:
- Cambia el color de fondo del encabezado y del pie de página.
- Cambia el tamaño y el color de la fuente del título principal.
- Crea una lista de navegación horizontal en el encabezado y agrega algunos elementos de lista.
- Añade un efecto hover a los elementos de la lista de navegación para que - cambien de color cuando se pasa el cursor sobre ellos.
- Crea una sección de productos y aplica un diseño de cuadrícula para mostrar las imágenes de los productos.
- Agrega un borde alrededor de cada imagen de producto.
- Aplica un efecto hover a cada imagen de producto para que se agrande - ligeramente cuando se pasa el cursor sobre ella.
- Agrega algunos botones de llamado a la acción debajo de cada imagen de - producto.
- Cambia el color y el tamaño de los botones de llamado a la acción.
- Crea una sección de testimonios y utiliza CSS para diseñar un cuadro de - citas.
- Agrega algunas citas dentro del cuadro de citas y utiliza CSS para cambiar la fuente y el tamaño del texto.
- Agrega un pie de página y cambia el color de fondo del mismo.
- Ajusta el margen y el relleno de cada sección para que se vean bien en diferentes tamaños de pantalla.


## Notas
- Abrir index.html para ejecutar la estructura creada. Posteriormente podrán probar los requerimientos del reto.

## index.html
```
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <link rel="stylesheet" href="Style.css" />
      <title>Document</title>
    </head>
```

```  
  <body>
    <header>
      <h1 id="#Home">Tienda 1</h1>
    </header>
```

```
    <nav>
      <ul>
        <li><a href="#Catalogo">Catalogo</a></li>
        <li><a href="#Contacto">Contacto</a></li>
        <li><a href="Testimonios.html">Testimonios</a></li>
      </ul>
    </nav>
```

```
    <main>
      <div class="articles-container">
        <article>
          <h3>Conjunto 2 Piezas para Niño</h3>
          <img src="1.jpg" alt="Producto1" width=50% />
          <button>
            <a href="Producto1.html">Ver</a>
          </button>
        </article>
        <article>
          <h3>Conjunto 3 Piezas para Niño</h3>
          <img src="2.jpg" alt="Producto2" width=50% />
          <button>
            <a href="Producto2.html">Ver</a>
          </button>
        </article>
        <article>
          <h3>Chaqueta térmica</h2>
          <img src="3.png" alt="Producto3" width=50% />
          <button>
            <a href="Producto3.html">Ver</a>
          </button>
        </article>
        <article>
          <h3>Conjunto 2 Piezas - Niño</h3>
          <img src="4.png" alt="Producto4" width=50% />
          <button>
            <a href="Producto4.html">Ver</a>
          </button>
        </article>
        <article>
          <h3>Pijama Carter's</h3>
          <img src="5.png" alt="Producto5" width=50% />
          <button>
            <a href="Producto5.html">Ver</a>
          </button>
        </article>
        <article>
          <h3>Camisa Oshkosh</h3>
          <img src="6.png" alt="Producto6" width=50% />
          <button>
            <a href="Producto6.html">Ver</a>
          </button>
        </article>
      </div>
      

      <h3>Las imágenes son referenciales</h3>
    </main>
```

```
    <footer id="#footer">
      <p id="Contacto">Contáctamos al fono +56999999999</p>
      <a href="#Home">Ir a Inicio</a>
      <img src="Logo.jpg" alt="Logo" width="10%" />
    </footer>
  </body>
</html>
```


## css
```
html, body{
    margin: 0px;
    padding: 0px;
}

header{
    padding: 10px;
}

h1{
    background-image: url(https://fos.com.mx/cdn/shop/articles/negocio_de_ropa.webp?v=1690921572&width=640);
    background-position: center;
    background-size: cover;
    padding: 50px;
    margin: 0px;
    text-align: center;
    font-family: 'Monserrat';
    font-size: 50px;
    color:#9EF8EE;
    text-shadow: 2px 2px 10px #348888;
}


  nav ul li a {
    color: black;
    padding: 5px;
  }
  
  nav ul li a:hover {
    color: blue;
    background-color: #9EF8EE;
    text-decoration: underline;
    border-radius: 5px;
  }


ul{
    margin: 0px;
    padding: 15px;
    background-color: #22BABB;  
}

li{
    list-style: none;
    display: inline;
    padding: 10px;
    text-shadow: none;
    color: black;
}

a{
    text-decoration: none;
}

article{
    margin: 10px;
    padding: 10px;
    background-color: rgb(255, 255, 254);
    border: 2px solid #FA7F08;
    border-radius: 10px;
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

h3{
    margin: 0px;
    padding: 20px;
}

p{
    display: inline-block;
    padding: 0px 100px;
}

main p{
    font-weight: bold;
}

footer{
    padding: 10px;
    background-color: #22BABB;
}

footer img{
    padding-left: 100px;
    padding-top: 10px;
}

h2{
    padding: 20px;
    color: black;
    margin: 5px;
}

.Producto {
    border: 2px solid beige;
    border-radius: 10px;
}


article img{
    border: 2px solid #F24405;
    border-radius: 10px;
    overflow:hidden;
}

article img:hover {
    -webkit-transform:scale(1.2);
    transform:scale(1.2);
}

.articles-container{
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 10px;
    padding: 10px;
}
  
article button {
    border: none;
    background-color:#9EF8EE;
    padding: 10px 10px;
    font-size: 10px;
    cursor: pointer;
    margin: 20px;
}

button:hover {
    background: #22BABB;
}


.container-testimonies{
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 10px;
    padding: 20px;
}

.testimony{
    background: beige;
    padding: 5px;
    text-align: left;
    align-content:flex-start;
}
```

## Testimonios
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="Style.css" />
    <title>Document</title>
  </head>
  <body>
    <header>
      <h1 id="#Home">Tienda 1</h1>
    </header>

    <nav>
      <ul>
        <li><a href="index.html">Catalogo</a></li>
        <li><a href="#Contacto">Contacto</a></li>
        <li><a href="Testimonios.html">Testimonios</a></li>
      </ul>
    </nav>
    <main>
        <h2>Testimonios</h2>
        <div class="container-testimonies">
            <div class="testimony">
                <h4>Usuario 1</h4>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                </p>
            </div>
            <div class="testimony">
                <h4>Usuario 2</h4>
                <p>
                    Consequatur veniam eos illum quasi minima consectetur exercitationem! Dolorem maxime magnam iusto magni?
                </p>
            </div>
            <div class="testimony">
                <h4>Usuario 3</h4>
                <p>
                    Iste vitae voluptatem est, dignissimos assumenda repudiandae nostrum reprehenderit
                </p>
            </div>
            <div class="testimony">
                <h4>Usuario 4</h4>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                </p>
            </div>
        </div>
    </main>

    <footer id="#footer">
      <p id="Contacto">Contáctamos al fono +56999999999</p>
      <a href="#Home">Ir a Inicio</a>
      <img src="Logo.jpg" alt="Logo" width="10%" />
    </footer>
  </body>
</html>
```


## Productos
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="Style.css" />
    <title>Document</title>
  </head>
  <body>
    <header>
      <h1 id="#Home">Tienda 1</h1>
    </header>

    <nav>
      <ul>
        <li><a href="index.html">Catalogo</a></li>
        <li><a href="#Contacto">Contacto</a></li>
        <li><a href="Testimonios.html">Testimonios</a></li>
      </ul>
    </nav>
    <main>
        <h2>Conjunto 2 Piezas para Niño</h2>
        <img src="1.jpg" alt="Producto1" width=50% />
        <p>Conjunto 2 Piezas Camisa y Pantalón Niño Carter's</p>
    </main>

    <footer id="#footer">
      <p id="Contacto">Contáctamos al fono +56999999999</p>
      <a href="#Home">Ir a Inicio</a>
      <img src="Logo.jpg" alt="Logo" width="10%" />
    </footer>
  </body>
</html>
```
