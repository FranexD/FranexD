# 
![banner](snopy.webp)
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Perfil Profesional</title>
    <style>
        /* Estilos generales */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #fff;
            background-color: #1a1a1a;
            background-size: cover;
            transition: background 0.5s ease-in-out;
        }

        .container {
            width: 90%;
            margin: auto;
            overflow: hidden;
        }

        /* Encabezado personalizado */
        .header {
            background: #333;
            color: #f2a3c3;
            text-align: center;
            padding: 80px 0;
            font-size: 2.5em;
            font-weight: bold;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
            position: relative;
            transition: background-color 0.5s ease;
        }

        .header h1 {
            margin: 0;
            font-size: 3em;
            color: #f5a3e0;
        }

        /* Sección "Sobre Mí" */
        .about {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 40px;
            margin-top: 20px;
            border-radius: 10px;
            background: rgba(255, 102, 204, 0.2);
            text-align: center;
            transition: transform 0.3s ease;
            box-shadow: 0px 5px 15px rgba(255, 102, 204, 0.3);
            color: #f5a3e0;
        }

        .about:hover {
            transform: scale(1.02);
            box-shadow: 0px 8px 20px rgba(255, 102, 204, 0.4);
        }

        .about img {
            width: 150px;
            border-radius: 50%;
            transition: transform 0.3s ease;
            margin-bottom: 20px;
        }

        .about img:hover {
            transform: scale(1.1);
        }

        .about h2 {
            color: #ff66cc;
        }

        /* Botón de descarga */
        .cv-button {
            display: inline-block;
            margin-top: 20px;
            padding: 12px 24px;
            background-color: #f5a3e0;
            color: #1a1a1a;
            text-decoration: none;
            font-weight: bold;
            border-radius: 8px;
            transition: background-color 0.3s ease;
        }

        .cv-button:hover {
            background-color: #ff66cc;
            color: #fff;
        }

        /* Sección de habilidades */
        .skills {
            background: rgba(255, 102, 204, 0.1);
            color: #fff;
            padding: 30px 0;
            text-align: center;
            margin-top: 20px;
            border-radius: 10px;
            box-shadow: 0px 5px 15px rgba(255, 102, 204, 0.2);
        }

        .skills h2 {
            text-transform: uppercase;
            margin-bottom: 20px;
            color: #ff66cc;
        }

        .skills-list {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            list-style: none;
            padding: 0;
        }

        .skills-list li {
            margin: 10px;
            padding: 10px 20px;
            background: #333;
            border-radius: 4px;
            color: #f5a3e0;
            font-weight: bold;
            transition: transform 0.3s ease, background-color 0.3s ease;
        }

        .skills-list li:hover {
            transform: translateY(-5px);
            background-color: #ff66cc;
        }

        /* Pie de página */
        footer {
            background: #333;
            color: #fff;
            text-align: center;
            padding: 20px;
            margin-top: 20px;
            border-top-left-radius: 10px;
            border-top-right-radius: 10px;
        }

        footer a {
            color: #ff66cc;
            text-decoration: underline;
        }

        footer a:hover {
            color: #f5a3e0;
        }
    </style>
</head>

<body>
    <!-- Incluye jQuery -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

    <!-- Encabezado -->
    <header class="header">
        <h1>Francesca Castillo</h1>
    </header>

    <div class="container">
        <!-- "Sobre Mí" -->
        <section id="about" class="about">
            <img src="image/congafas.jpg" alt="Foto de perfil">
            <h2>Sobre Mí</h2>
            <p>¡Hola! 👋 Soy una estudiante de Ingeniería en Informática de Chile. Apasionada por el desarrollo de<br/>
                software, bases de datos y el desarrollo web. Disfruto de enfrentar nuevos retos y aprender algo<br/>
                nuevo cada día.</p><br/>
            <!-- Botón para descargar mi curriculum--->
            <a href="image/curricul actual fran.pdf" class="cv-button" download="Mi_Curriculum">Descargar CV</a>
        </section>

        <!-- Habilidades -->
        <section id="skills" class="skills">
            <h2>Habilidades Técnicas</h2>
            <ul class="skills-list">
                <li>HTML5</li>
                <li>CSS3</li>
                <li>JavaScript</li>
                <li>Python</li>
                <li>MySQL</li>
                <li>React</li>
                <li>Git</li>
                <li>Google Cloud</li>
                <li>Oracle</li>
            </ul>
        </section>
    </div>

    <!-- Pie de página -->
    <footer>
        <p>Contacto: <a href="francesca.castillo25@gmail.com">francesca.castillo25@gmail.com</a></p>
    </footer>

    <script>
        $(document).ready(function () {
            // Efecto de hover para el fondo del encabezado
            $(".header").hover(function () {
                $(this).css("background-color", "#1a1a1a");
            }, function () {
                $(this).css("background-color", "#333");
            });

            // Efecto de desplazamiento para "Sobre Mí"
            $(".about").hover(function () {
                $(this).css("background-color", "rgba(255, 102, 204, 0.3)");
            }, function () {
                $(this).css("background-color", "rgba(255, 102, 204, 0.2)");
            });

            // Animación de rebote en habilidades
            $(".skills-list li").hover(function () {
                $(this).animate({ top: "-10px" }, 200);
            }, function () {
                $(this).animate({ top: "0px" }, 200);
            });
        });
    </script>
</body>

</html>
