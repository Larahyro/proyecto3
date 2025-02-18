Proyecto3 Landingpage con HTML y CSS
En la primera version del proyecto trabajé en un archivo HTML y uno CSS separados:
<!--Finalmente la distribución no me gustó y habia intentado colocar un carrousel en el main, pero en el css finalmente no pude ajustar los componentes y cuando lo hice no me gustó, asi que pasé a la siguiente versión>

<body>
    <!-- Header -->
    <header>
        <div class="logo">
            <img src="Logo.png.png" alt="Logo de Al Sur del Mundo">
        </div>
        <nav>
            <ul>
                <li><a href="#main">Conocenos</a></li>
                <li><a href="#products">Travesias y Experiencias</a></li>
                <li><a href="#footer">Comunicate con Nosotros</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main -->
    <section id="main">
        <img src="TdelP.jpg" class= "imagen" alt= "Una de las maravillas del mundo">
        <h1>" Al sur del mundo"</h1>

        <p>Explora destinos únicos y vive experiencias inolvidables desde la Patagonia Chilena/argentina,hasta la Antartica Chilena. 

        </p>

        <button>Descubre más</button>

        </section>

    <!-- Productos -->
    <section class="products">
        <h2>Nuestros Paquetes</h2>
        <div class="product-grid">
            <div class="product">
                <img src="product1.jpg" alt="Producto 1">
                <h3>Paquete 1</h3>
                <p>Cueva del milodon y torres del paine.</p>
            </div>
            <div class="product">
                <img src="product2.jpg" alt="Producto 2">
                <h3>Paquete 2</h3>
                <p>Antartida chile y tierra del fuego.</p>
            </div>
            <div class="product">
                <img src="product3.jpg" alt="Producto 3">
                <h3>Paquete 3</h3>
                <p>trekking por la patagonia.</p>
            </div>
            <div class="product">
                <img src="product4.jpg" alt="Producto 4">
                <h3>Paquete 4</h3>
                <p>arma tu itinerario.</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="footer">
        <p>&copy; 2025 Turismo Al sur del mundo | Todos los derechos reservados</p>
        <p>Contactanos: info@turismoalfindelmundo.com</p>
    </footer>
</body>

<!-- en la segunda y tercera version segui trabajando aparte html y css y fui ajustando el css al contenido que tenia en el HTML, pero al tratar de ajustar todo me di cuenta que habia hecho mal la maqueta, asi que reescribí el codigo completo a un sólo archivo html usando la etiqueta style-->

<!--acá agregué un wave--> 
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#ff8000" fill-opacity="1" d="M0,64L48,74.7C96,85,192,107,288,112C384,117,480,107,576,96C672,85,768,75,864,90.7C960,107,1056,149,1152,154.7C1248,160,1344,128,1392,112L1440,96L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"></path>
      </svg>

<!--y el efecto parallax-->

    <main>
        <section class="sec1"></section>
        <div class="contain"><p>Trekking en el Parque Torres del Paine</p></div>
        <section class="sec2"></section>
        <div class="contain"><p>Navegación a la Isla Magdalena</p></div>
        <section class="sec3"></section>
        <div class="contain"><p>Kayak con Ballenas</p></div>
        <section class="sec4"></section>
        <div class="contain"><p>Atardecer en la Antártica</p></div>       
    </main>


   <!--en la ultima versión queria un footer bonito y dinamico, asi que busqué como hacer que cambiara de color --> 
   footer-enlaces ul li a{
            font-size: 18px;
            text-decoration: none;
            color:#fff;
            display: block;
            margin-bottom: 15px;
            transition: all .3s ease;
    <!-- además le puse iconos-->
    <div class="footer-enlaces">
                    <h5>Comunícate con nosotros</h5>
                    <div class="medios">
                        <a href="#"><i class="fas fa-phone-alt"></i></a>
                        <a href="#"><i class="fas fa-envelope"></i></a>
                        <a href="#"><i class="fab fa-whatsapp"></i></a>
                    </div>
    </div>

    <!-- ahora sólo me falta ajustar el diseño responsivo-->

    <!--separé los archivos en uno HTML y otro CSS, modifiqué la barra de navegacion dejando un estilo hamburguesa-->
    
    <nav class="navbar"> 
            <input type="checkbox" id="menu-toggle">
            <label for="menu-toggle" class="menu-icon">
                <div class="line"></div>
                <div class="line"></div>
                <div class="line"></div>
            </label>
    
     <!--y ajusté con media queries los ajustes al main y footer-->