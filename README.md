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
                <a class="nav-link" href="https://jd-354.github.io/RJ/">Inicio</a>
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
              <img src="https://watchfluence.com/wp-content/uploads/2024/04/v2-agkrn-0u4x7-1024x702.jpg"alt="Reloj 1" class="d-block w-100"width="600" height="300">
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
