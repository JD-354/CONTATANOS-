<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Reloj Maestro - Tienda de Relojes</title>
      <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>
       <style>
        .card-img-top {
          height: 200px;
          object-fit: cover;
        }

        body {
            font-family: 'Arial', sans-serif;
            overflow-x: hidden;
            background: linear-gradient(45deg,rgba(255, 255, 255, 0.1) , black);;
      }

      .navbar-brand img{ max-height: 500px;
      }
      .navbar-brand {
            font-size: 1.5rem;
            font-weight: bold;
            color: #fff;
            text-shadow: 0 0 20px rgba(0, 255, 255, 0.5);
        }


        /* Tablets */
        @media screen and (max-width: 768px) {
            .menu {
                display: none;
                width: 100%;
                position: absolute;
                top: 60px;
                left: 0;
                background: var(--primary-color);
                flex-direction: column;
                text-align: center;
            }

            .menu.active {
                display: flex;
            }

            .menu li {
                padding: 1rem;
                border-top: 100px solid rgba(255,255,255,0.1);
            }

            .menu-toggle {
                display: block;
            }

            .grid-container {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        /* Móviles */
        @media screen and (max-width: 480px) {
            .grid-container {
                grid-template-columns: 1fr;
            }
        }

      </style>
    </head>
    <body>
      <header>
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
          <a class="navbar-brand" href="#">Reloj Maestro</a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item active">
                <a class="nav-link" href="#">Inicio</a>
              </li>
              <li class="nav-item">
            <a class="nav-link" href="https://jd-354.github.io/SOBRE-NOSOTROS-/">Sobre Nosotros</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="https://jd-354.github.io/CONTATANOS-/">Contacto</a>
              </li>
            </ul>
          </div>
        </nav>
        <img src="https://blog-inolvidable.joyeriasbizzarro.com/hubfs/2024_MIDO_Blog_BannerHome_Desk.jpg"  class="d-block w-100" width="350" height="350">
      </header>
    
      <main>
        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
          <ol class="carousel-indicators">
            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
          </ol>
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img src="https://cdn.vox-cdn.com/thumbor/7kUDwyC7FvCDI_tjFcLTHjMxITc=/0x0:1053x773/1200x628/filters:focal(526x386:527x387)/cdn.vox-cdn.com/uploads/chorus_asset/file/15086412/hp-michael-bastian.0.0.1417555656.jpg" class="d-block w-100" alt="Reloj 1"width="600" height="300">
            </div>
            <div class="carousel-item">
              <img src="https://macrotehnicus.ro/wp-content/uploads/2021/10/11-cele-mai-bune-smartwatch-uri.jpg" class="d-block w-100" alt="Reloj 2"width="300" height="300">
            </div>
            <div class="carousel-item">
              <img src="https://static.runnea.com/images/202308/mejores-relojes-deportivos-hombre-listado-apertura-bene-1200x572x80xX.jpg?1" " class="d-block w-100" alt="Reloj 3" width="500" height="300">
            </div>
          </div>
          <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
    
        <div class="container my-5">
          <h2 class="text-center mb-4">Nuestros Relojes</h2>
          <div class="row">
            <div class="col-md-4 mb-4">
              <div class="card h-100">
                <img src="https://www.dhresource.com/0x0/f2/albu/g3/M01/A9/54/rBVaHVZJziSAN7e0AAGNU6CoJXo680.jpg" class="card-img-top" alt="Reloj 1">
                <div class="card-body">
                  <h5 class="card-title">Reloj Clásico</h5>
                  <p class="card-text">Reloj de diseño clásico con caja de acero inoxidable y correa de cuero.</p>
                  <p class="card-text font-weight-bold">$129.99</p>
                  <a href="#" class="btn btn-primary">Comprar Ahora</a>
                </div>
              </div>
            </div>
            <div class="col-md-4 mb-4">
              <div class="card h-100">
                <img src="https://www.relojesdeportivos.com.es/wp-content/uploads/2020/02/que-es-un-reloj-deportivo-768x768.jpg" class="card-img-top" alt="Reloj 2">
                <div class="card-body">
                  <h5 class="card-title">Reloj Deportivo</h5>
                  <p class="card-text">Reloj resistente al agua con funciones de cronógrafo y caja de titanio.</p>
                  <p class="card-text font-weight-bold">$199.99</p>
                  <a href="#" class="btn btn-primary">Comprar Ahora</a>
                </div>
              </div>
            </div>
            <div class="col-md-4 mb-4">
              <div class="card h-100">
                <img src="https://pic4.zhimg.com/v2-bada9daca9fba2e3d88a9e446231dbeb_r.jpg" class="card-img-top" alt="Reloj 3">
                <div class="card-body">
                  <h5 class="card-title">Reloj de Lujo</h5>
                  <p class="card-text">Reloj de diseño elegante con caja de oro rosa y correa de piel.</p>
                  <p class="card-text font-weight-bold">$499.99</p>
                  <a href="#" class="btn btn-primary">Comprar Ahora</a>
                </div>
              </div>
            </div>
          </div>
        </div>
    
        <div class="container my-5">
          <h2 class="text-center mb-4">Testimonios de Nuestros Clientes</h2>
          <div class="row">
            <div class="col-md-4 mb-4">
              <div class="card h-100">
                <div class="card-body">
                  <p class="card-text">"¡Excelente calidad y diseño! Mi nuevo reloj es hermoso y funciona perfectamente."</p>
                  <p class="card-text font-weight-bold">- Juan Pérez</p>
                </div>
              </div>
            </div>
            <div class="col-md-4 mb-4">
              <div class="card h-100">
                <div class="card-body">
                  <p class="card-text">"Estoy muy satisfecho con mi compra. El servicio al cliente fue excepcional y el envío fue rápido."</p>
                  <p class="card-text font-weight-bold">- María Gómez</p>
                </div>
              </div>
            </div>
            <div class="col-md-4 mb-4">
              <div class="card h-100">
                <div class="card-body">
                  <p class="card-text">"¡Me encanta mi nuevo reloj! Es elegante, cómodo y supera todas mis expectativas."</p>
                  <p class="card-text font-weight-bold">- Carlos Sánchez</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </main>
    
      <footer class="bg-dark text-white py-4">
        <div class="container">
          <div class="row">
            <div class="col-md-6">
              <p>&copy; 2024 Reloj Maestro. Todos los derechos reservados.</p>
            </div>
            <div class="col-md-6 text-md-right">
              <a href="#" class="text-white mr-3">Sobre Nosotros</a>
              <a href="#" class="text-white mr-3">Contacto</a>
              <a href="#" class="text-white">Política de Privacidad</a>
            </div>
          </div>
        </div>
      </footer>
    
      <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
      <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
      <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
        
