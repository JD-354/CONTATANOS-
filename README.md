# CONTATANOS-
BB
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tienda con Sección de Contactos</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" rel="stylesheet">
    <style>
        html {
            scroll-behavior: smooth; /* Para scroll suave */
        }
        .contact-section {
            padding: 80px 0;
            background-color: #f8f9fa;
        }
        .contact-info {
            padding: 20px;
            border-radius: 8px;
            background-color: white;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body>

    <!-- Sección Inicio -->
    <section id="inicio" class="mt-5 pt-5">
        <div class="container">
            <h2>Bienvenidos a nuestra tienda</h2>
            <!-- Contenido de inicio aquí -->
        </div>
    </section>

    <!-- Sección Productos -->
    <section id="productos" class="py-5">
        <div class="container">
            <h2>Nuestros Productos</h2>
            <!-- Contenido de productos aquí -->
        </div>
    </section>

    <!-- Sección de Contacto -->
    <section id="contacto" class="contact-section">
        <div class="container">
            <h2 class="text-center mb-5">Contáctanos</h2>
            <div class="row">
                <!-- Información de Contacto -->
                <div class="col-md-6 mb-4">
                    <div class="contact-info">
                        <h3>Información de Contacto</h3>
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
                        <h3>Envíanos un mensaje</h3>
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
    <footer class="bg-dark text-white py-4">
        <div class="container text-center">
            <p class="mb-0">© 2024 Mi Tienda. Todos los derechos reservados.</p>
        </div>
    </footer>

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

   
