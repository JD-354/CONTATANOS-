<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tienda con Sección de Contactos</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" rel="stylesheet">

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

        .contact-section {
            padding: 20px ;
            background-color:rgba(0,0,0,0.1);
        }
        .contact-info {
            padding: 20px;
            border-radius: 20px;
            background-color:rgba(255, 255, 255, 0.1);
            box-shadow: 0 20px 20px rgb(0, 170, 255);
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
    </body>
    <header>
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
          <a class="navbar-brand" href="#">Reloj Maestro</a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item active">
                <a class="nav-link"https://jd-354.github.io/RJ/ ">Inicio</a>
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
          <div class="carousel-inner"></div>
            <div class="carousel-item active">
              <img src="#"alt="Reloj 1"class="d-block w-100" width="0" height="0">
            </div>
            <div class="carousel-item">
              <img src="#" alt="Reloj 2"class="d-block w-100" width="0" height="0">
            </div>
            <div class="carousel-item">
              <img src="#"class="d-block w-100"  alt="Reloj 3" width="0" height="0">
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
        <div class="container text-center">
            <h3 class="mb-0"></h3>
        </div>
    </footer>
    
    <section id="contacto-info" class="contact-section">
        <div class="container">
            <h3 class="mb-3"></h3>
            <div class="row">
                            <li class="mb-3">
                                <i class="bi bi-telephone"></i>
                                <footer class="bg-dark text-white py-4">
                                    <div class="container text-center">
                                        <h3 class="mb-0">PARA CONTATARNOS</h3>
                                    </div>
                                </footer>
                                <section id="contacto" class="contact-section">
                                    <div class="container">
                                        <h3 class="mb-3"></h3>
                                        <div class="row">
                                            <!-- Información de Contacto -->
                                            <div class="mb-3">
                                                <div class="contact-info">
                                                    <h3>Información </h3>
                                                    <ul class="list-unstyled">
                                                        <li class="mb-3">
                                                            <i class="bi bi-geo-alt"></i>
                                                            <strong>Dirección:</strong> Calle Principal #123
                                                        </li>
                                                        <li class="mb-3">
                                                            <i class="bi bi-telephone"></i>
                                                            <strong>Teléfono:</strong> (123) 456-7890
                                                        </li>
                                                        <li class="mb-3">
                                                            <i class="bi bi-envelope"></i>
                                                            <strong>Email:</strong> info@mitienda.com
                                                        </li>
                                                        <li class="mb-3">
                                                            <i class="bi bi-clock"></i>
                                                            <strong>Horario:</strong> Lun-Vie: 9:00 - 18:00
                                                        </li>
                                                    </ul>
                                                </div>
                                            </div>
                                            <!-- Formulario de Contacto -->
                                            <div class="col-md-6">
                                                <div class="contact-info">
                                                    <h3>Llenar</h3>
                                                    <form id="contactForm">
                                                        <div class="mb-3">
                                                            <label for="nombre" class="form-label">Nombre</label>
                                                            <input type="text" class="form-control" id="nombre" required>
                                                        </div>
                                                        <div class="mb-3">
                                                            <label for="email" class="form-label">Email</label>
                                                            <input type="email" class="form-control" id="email" required>
                                                        </div>
                                                        <div class="mb-3">
                                                            <label for="mensaje" class="form-label">Mensaje</label>
                                                            <textarea class="form-control" id="mensaje" rows="4" required></textarea>
                                                        </div>
                                                        <button type="submit" class="btn btn-primary">Enviar Mensaje</button>
                                                    </form>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </section>
                
    
    <!-- Footer -->
    

    <!-- Bootstrap JS -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/js/bootstrap.bundle.min.js"></script>
    
    <!-- Script para el formulario -->
    <script>
        // Manejo del formulario de contacto
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            // Aquí puedes agregar la lógica para enviar el formulario
            alert('Mensaje enviado correctamente!');
            this.reset();
        });

        // Scroll suave para los enlaces de navegación
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
