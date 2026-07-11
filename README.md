<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistemas de Información</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- base.html: Encabezado y menú principal reutilizables -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">Soluciones TI</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#menu">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="menu">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#inicio">Inicio</a></li>
                    <li class="nav-item"><a class="nav-link" href="#quienes-somos">Quiénes Somos</a></li>
                    <li class="nav-item"><a class="nav-link" href="#servicios">Servicios</a></li>
                    <li class="nav-item"><a class="nav-link" href="#registro-desarrolladores">Registro</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contacto">Contacto</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- base.html: Hero principal con título y descripción -->
    <header>
        <h1 class="display-5 fw-bold">Soluciones Tecnológicas Integrales</h1>
        <p class="lead">Diseñamos experiencias digitales eficientes, modernas y accesibles para cada proyecto.</p>
    </header>

    <!-- base.html: Contenido principal dinámico renderizado con JavaScript -->
    <main class="container py-4">
        <section id="inicio" class="section-card">
            <div class="row align-items-center">
                <div class="col-lg-7">
                    <h2 class="text-center text-lg-start">Inicio</h2>
                    <p>Bienvenido a nuestro catálogo digital para la gestión de servicios y soporte técnico. Este proyecto reúne soluciones tecnológicas adaptadas a las necesidades de los usuarios, con un enfoque práctico y visualmente moderno.</p>
                    <div class="d-flex flex-wrap gap-2 justify-content-center justify-content-lg-start">
                        <a href="#servicios" class="btn btn-success">Ver Servicios</a>
                        <a href="#contacto" class="btn btn-outline-success">Contáctanos</a>
                    </div>
                </div>
                <aside class="col-lg-5 mt-3 mt-lg-0">
                    <div class="hero-card">
                        <h5 class="text-success">Atención integral</h5>
                        <p>Gestionamos soporte, organización de información y acompañamiento tecnológico con enfoque en resultados.</p>
                    </div>
                </aside>
            </div>
        </section>

        <section id="quienes-somos" class="section-card">
            <h2 class="text-center mb-4">Quiénes Somos</h2>
            <div class="row align-items-center">
                <article class="col-md-6">
                    <p>Somos un equipo dedicado al desarrollo de sistemas de información que facilitan la gestión de servicios tecnológicos. Nuestro trabajo está enfocado en ofrecer herramientas digitales claras, seguras y fáciles de usar para empresas y usuarios.</p>
                    <p>Destacamos la innovación, la accesibilidad y la calidad en cada solución que implementamos.</p>
                </article>
                <aside class="col-md-6">
                    <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=900&q=80" class="img-fluid rounded shadow img-cover" alt="Equipo trabajando en tecnología">
                </aside>
            </div>
        </section>

        <section id="servicios" class="section-card">
            <h2 class="text-center mb-4">Servicios</h2>
            <div id="serviciosLista" class="row"></div>
            <div id="mensajeServicios" class="mt-4"></div>
            <div class="mt-4 text-center">
                <iframe class="img-fluid rounded shadow" width="100%" height="315" src="https://www.youtube-nocookie.com/embed/NLvcamk5yiM?si=d64RqSq4BVRaFy1-" title="Video explicativo" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            </div>
        </section>

        <section id="proyectos" class="section-card">
            <h2 class="text-center mb-4">Proyectos en Desarrollo</h2>
            <div id="proyectosDinamicos" class="row"></div>
            <div id="mensajeProyectos" class="mt-3"></div>
        </section>

        <section id="registro-desarrolladores" class="section-card">
            <h2 class="text-center mb-4">Base de Registro de Desarrolladores</h2>
            <div class="row">
                <div class="col-lg-5 mb-4">
                    <div class="card p-4 shadow-sm">
                        <h4 class="mb-3 text-success">Ingresar Datos</h4>
                        <p class="text-muted small">Completa los campos para agregar un nuevo registro al sistema.</p>
                        <form id="formRegistro" novalidate>
                            <div class="mb-3">
                                <label class="form-label" for="inputNombre">Nombre</label>
                                <input type="text" class="form-control" id="inputNombre" placeholder="Escribe el nombre completo">
                                <div class="invalid-feedback" id="errorNombre"></div>
                            </div>
                            <div class="mb-3">
                                <label class="form-label" for="selectCategoria">Categoría</label>
                                <select class="form-select" id="selectCategoria">
                                    <option value="" selected>Elige una opción...</option>
                                    <option value="Frontend">Frontend</option>
                                    <option value="Backend">Backend</option>
                                    <option value="Fullstack">Fullstack</option>
                                </select>
                                <div class="invalid-feedback" id="errorCategoria"></div>
                            </div>
                            <div class="mb-3">
                                <label class="form-label" for="txtDescripcion">Descripción</label>
                                <textarea class="form-control" id="txtDescripcion" rows="3" placeholder="Agrega una descripción detallada..."></textarea>
                                <div class="invalid-feedback" id="errorDescripcion"></div>
                            </div>
                            <button type="submit" class="btn btn-success w-100">Guardar Registro</button>
                        </form>
                    </div>
                </div>

                <div class="col-lg-7">
                    <div class="card p-4 shadow-sm h-100">
                        <div class="d-flex justify-content-between align-items-center mb-3">
                            <h4 class="text-success m-0">Registros en Base de Datos</h4>
                            <button class="btn btn-outline-danger btn-sm" id="btnBorrarTodo">Borrar Todo</button>
                        </div>
                        <div class="d-flex justify-content-between align-items-center mb-2">
                            <span class="text-muted">Total de registros: <strong id="totalRegistros">0</strong></span>
                        </div>
                        <div id="mensajeValidacion"></div>
                        <div class="table-responsive mt-3">
                            <table class="table table-striped table-hover align-middle">
                                <thead class="table-dark">
                                    <tr>
                                        <th>Nombre</th>
                                        <th>Categoría</th>
                                        <th>Descripción</th>
                                        <th>Acción</th>
                                    </tr>
                                </thead>
                                <tbody id="tablaRegistros"></tbody>
                            </table>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="contacto" class="section-card">
            <h2 class="text-center mb-4">Contacto</h2>
            <div class="row">
                <div class="col-lg-7">
                    <form>
                        <div class="mb-3">
                            <input type="text" class="form-control" placeholder="Nombre">
                        </div>
                        <div class="mb-3">
                            <input type="email" class="form-control" placeholder="Correo electrónico">
                        </div>
                        <div class="mb-3">
                            <input type="text" class="form-control" placeholder="Asunto">
                        </div>
                        <div class="mb-3">
                            <textarea class="form-control" rows="4" placeholder="Mensaje"></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary">Enviar</button>
                    </form>
                </div>
                <aside class="col-lg-5 mt-4 mt-lg-0">
                    <div class="card p-4 shadow-sm h-100">
                        <h5 class="text-success">Canales de contacto</h5>
                        <p>Estamos disponibles para atender tus consultas y recibir tus comentarios.</p>
                        <div class="d-grid gap-2">
                            <a href="mailto:jair18042007@gmail.com" class="btn btn-outline-primary">Correo</a>
                            <a href="https://www.facebook.com/share/14dKGgcFMSz/" target="_blank" class="btn btn-outline-info">Facebook</a>
                            <a href="https://www.instagram.com/cristopher_xrv18?igsh=MTBlMWRhaDFuM2doNg==" target="_blank" class="btn btn-outline-danger">Instagram</a>
                        </div>
            </div>
        </section>
    <!-- base.html: Pie de página global del sitio -->
    <footer>
        <p><strong>Nombre:</strong> Cristopher Jair Robalino Montes</p>
        <p><strong>Asignatura:</strong> DESARROLLO DE APLICACIONES WEB</p>
        <p><strong>Año:</strong> 2026</p>
    </footer>

    <img src="https://eva.pregrado.uea.edu.ec/eva2626/web/pluginfile.php/1/theme_moove/logo/1780768848/logo_eva_pregrado_2626.png" alt="Logo EVA" class="bottom-left">

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
    <script src="script.js"></script>
</body>
</html>
