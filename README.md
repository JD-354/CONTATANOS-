<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tienda con Sección de Contactos</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(45deg, #1a1a1a, #2c3e50);
        }

        .card {
            position: relative;
            width: 750px;
            height: 450px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 25px 45px rgba(0, 0, 0, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.2);
            display: flex;
            align-items: center;
            transition: 0.5s;
            overflow: hidden;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 35px 65px rgba(0, 0, 0, 0.3);
        }

        .card::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at right top, 
                rgba(1, 67, 255, 0.3),
                transparent 40%);
            pointer-events: none;
        }

        .left-section {
            width: 40%;
            height: 100%;
            background: rgba(255, 255, 255, 0.1);
            padding: 40px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border-right: 1px solid rgba(255, 255, 255, 0.1);
        }

        .profile-img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 3px solid rgba(255, 255, 255, 0.2);
            overflow: hidden;
            margin-bottom: 20px;
            transition: 0.5s;
        }

        .profile-img:hover {
            transform: scale(1.1);
            border-color: #0088ff;
        }

        .profile-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .right-section {
            width: 60%;
            padding: 40px;
            color: white;
        }

        .name {
            font-size: 2.5em;
            margin-bottom: 10px;
            font-weight: 700;
            background: linear-gradient(45deg, #fff, #0088ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .title {
            font-size: 1.2em;
            color: #0088ff;
            margin-bottom: 20px;
            font-weight: 500;
        }

        html {
            scroll-behavior: smooth; /* Para scroll suave */
        }
        .contact-section {
            padding: 90px ;
            background-color:rgba(0,0,0,0.1);
        }
        .contact-info {
            padding: 20px;
            border-radius: 9px;
            background-color: rgba(1, 67, 255, 0.3);
            box-shadow: 0 20px 20px rgba(0,0,0,0.1);
        }

        .mb-3{column-rule-color: #fff;}
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
        <div class="container">
            <a class="navbar-brand" href="#">Mi Tienda</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#inicio">Inicio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contacto">Contacto</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" data-bs-toggle="modal" data-bs-target="#contactModal" 
                           style="cursor: pointer;">Contacto Modal</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>


    <footer class="bg-dark text-white py-4">
        <div class="container text-center">
            <h3 class="mb-0">Bienvenidos a nuestra tienda</h3>
        </div>
    </footer>
    <section id="contacto" class="contact-section">
        <div class="container">
            <h3 class="mb-3">Contáctanos</h3>
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

    <!-- Modal de Contacto -->
    <div class="modal fade" id="contactModal" tabindex="-1" aria-labelledby="contactModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="contactModalLabel">Contacto Rápido</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="mb-3">
                            <label for="modalNombre" class="form-label">Nombre</label>
                            <input type="text" class="form-control" id="modalNombre" required>
                        </div>
                        <div class="mb-3">
                            <label for="modalEmail" class="form-label">Email</label>
                            <input type="email" class="form-control" id="modalEmail" required>
                        </div>
                        <div class="mb-3">
                            <label for="modalMensaje" class="form-label">Mensaje</label>
                            <textarea class="form-control" id="modalMensaje" rows="3" required></textarea>
                        </div>
                    </form>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cerrar</button>
                    <button type="button" class="btn btn-primary">Enviar Mensaje</button>
                </div>
            </div>
        </div>
    </div>

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
</body>
</html>
