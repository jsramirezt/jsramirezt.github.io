<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mexadecimal - Cyberpunk en México</title>
    <meta name="description" content="Descubre 'Mexadecimal', el libro de ciencia ficción cyberpunk que muestra a México en el año 2065 y su infernal sociedad. Autor: Jesús Sacramento Ramírez Tapia.">
    <meta name="keywords" content="cyberpunk, libro ciencia ficción, mexadecimal, Jesús Sacramento Ramírez Tapia, Jesús Ramírez, distopía, sociedad mexicana, México, futuro distópico, ciberpunk, 2065">
    <meta name="author" content="Kaito Nakamura">
    <style>
        /* Estilos generales */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Courier New', monospace;
        }
        
        body {
            background-color: #121212;
            color: #00ff00;
            line-height: 1.6;
            padding: 20px;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(0, 255, 0, 0.05) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(0, 255, 0, 0.05) 0%, transparent 20%);
            min-height: 100vh;
        }
        
        /* Efecto de escaneo */
        body::after {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: repeating-linear-gradient(
                0deg,
                rgba(0, 0, 0, 0.15),
                rgba(0, 0, 0, 0.15) 1px,
                transparent 1px,
                transparent 2px
            );
            pointer-events: none;
            z-index: 100;
            animation: scan 8s linear infinite;
        }
        
        @keyframes scan {
            0% { transform: translateY(-100%); }
            100% { transform: translateY(100%); }
        }
        
        /* Contenedor principal */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }
        
        /* Encabezado */
        header {
            text-align: center;
            padding: 20px 0;
            border-bottom: 2px solid #00ff00;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(0, 255, 0, 0.1), transparent);
            transform: translateX(-100%);
            /*animation: shine 5s infinite;*/
        }
        
        @keyframes shine {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        
        /* Logo */
        .logo {
            font-size: 3.5rem;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 4px;
            margin-bottom: 15px;
            text-shadow: 0 0 10px #00ff00, 0 0 20px #00ff00;
            animation: flicker 4s infinite alternate;
        }
        
        @keyframes flicker {
            0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% {
                opacity: 1;
            }
            20%, 24%, 55% {
                opacity: 0.7;
            }
        }
        
        .logo a {
            color: #00ff00;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .logo a:hover {
            text-shadow: 0 0 15px #00ff00, 0 0 30px #00ff00;
        }
        
        /* Botón */
        .cta-button {
            display: inline-block;
            padding: 12px 30px;
            background-color: transparent;
            color: #00ff00;
            border: 2px solid #00ff00;
            text-decoration: none;
            text-transform: uppercase;
            font-weight: bold;
            letter-spacing: 2px;
            margin-top: 10px;
            position: relative;
            overflow: hidden;
            transition: all 0.3s ease;
            box-shadow: 0 0 10px rgba(0, 255, 0, 0.5);
        }
        
        .cta-button::before {
            content: "";
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(0, 255, 0, 0.2), transparent);
            transition: all 0.5s ease;
        }
        
        .cta-button:hover {
            background-color: rgba(0, 255, 0, 0.1);
            box-shadow: 0 0 20px rgba(0, 255, 0, 0.8);
        }
        
        .cta-button:hover::before {
            left: 100%;
        }
        
        /* Contenido principal */
        .main-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .book-cover {
            text-align: center;
            position: relative;
        }
        
        .book-image {
            width: 100%;
            max-width: 400px;
            height: auto;
            border: 3px solid #00ff00;
            box-shadow: 0 0 20px rgba(0, 255, 0, 0.5);
            /*filter: grayscale(100%) contrast(120%);*/
            transition: all 0.5s ease;
        }
        
        .book-image:hover {
            filter: grayscale(0%) contrast(120%);
            box-shadow: 0 0 30px rgba(0, 255, 0, 0.8);
        }
        
        .book-info {
            padding: 20px;
            border: 1px solid #00ff00;
            background-color: rgba(0, 0, 0, 0.5);
            box-shadow: 0 0 15px rgba(0, 255, 0, 0.3);
        }
        
        .book-title {
            font-size: 2rem;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 2px;
            text-shadow: 0 0 5px #00ff00;
        }
        
        .book-description {
            margin-bottom: 20px;
            line-height: 1.8;
        }
        
        .book-details {
            margin-top: 20px;
        }
        
        .detail-item {
            margin-bottom: 10px;
            display: flex;
        }
        
        .detail-label {
            font-weight: bold;
            min-width: 120px;
        }
        
        /* Sección de capítulos */
        .chapters {
            margin-top: 40px;
        }
        
        .section-title {
            font-size: 1.8rem;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 2px;
            border-bottom: 1px solid #00ff00;
            padding-bottom: 10px;
            text-shadow: 0 0 5px #00ff00;
        }
        
        .chapter-list {
            list-style-type: none;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 15px;
        }
        
        .chapter-item {
            padding: 15px;
            border: 1px solid #00ff00;
            background-color: rgba(0, 0, 0, 0.5);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .chapter-item::before {
            content: ">";
            position: absolute;
            left: 10px;
            color: #00ff00;
            font-weight: bold;
        }
        
        .chapter-item:hover {
            background-color: rgba(0, 255, 0, 0.1);
            box-shadow: 0 0 10px rgba(0, 255, 0, 0.5);
            transform: translateX(5px);
        }
        
        .chapter-number {
            font-weight: bold;
            margin-bottom: 5px;
            margin-left: 20px;
        }
        
        .chapter-title {
            margin-left: 20px;
        }
        
        /* Pie de página */
        footer {
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
            border-top: 1px solid #00ff00;
            font-size: 0.9rem;
            color: rgba(0, 255, 0, 0.7);
        }
        
        /* Efectos de terminal */
        .terminal-line {
            position: relative;
            margin-bottom: 10px;
        }
        
        .terminal-line::before {
            content: ">";
            position: absolute;
            left: -20px;
            color: #00ff00;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .main-content {
                grid-template-columns: 1fr;
            }
            
            .logo {
                font-size: 2.5rem;
            }
            
            .book-title {
                font-size: 1.5rem;
            }

        /* CLASE PARA SUPERSCRIPT */
        .sup {
            vertical-align: super;
            font-size: 0.3em;
            color: #00cc00;
        }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1 class="logo">
                <a href="https://www.ejemplo-libro-cyberpunk.com" target="_self">MEXADECIMAL<span class="sup">©</span></a>
            </h1>
            <a href="https://www.amazon.com.mx/Mexadecimal-Jes%C3%BAs-Sacramento-Ram%C3%ADrez-Tapia-ebook/dp/B08Q7D4DR7/ref=sr_1_1" class="cta-button" target="_blank">COMPRAR AHORA</a>
            <!--<a href="https://www.ejemplo-comprar-libro.com" class="cta-button" target="_blank">ENGLISH</a> -->
            <a href="https://mx-z.mx" class="cta-button" target="_blank">Saga MX-Z<span class="sup">©</span></a>
        </header>
        
        <main>
            <section class="main-content">
                <div class="book-cover">
                    <img src="./imgs/logo.jpg" alt="Portada del libro Mexadecimal" class="book-image">
                </div>
                
                <div class="book-info">
                    <h2 class="book-title">Mexadecimal<sup>©</sup></h2>
                    
                    <div class="terminal-line">
                        <p class="book-description">
                            ¡Oh vosotros los que entráis, adandonan toda esperanza! México, 2065.
                        <br>
                            "Desde cualquiera de las estaciones orbitales, la zona central de México semejaba un descomunal núcleo computacional cuántico." 
                        <br>
                            El avance de la tecnología ha dejado atrás a cualquier ley que ha intentado regularla. El calentamiento global ha provocado migraciones masivas hacia los interiores de los países. La verdad ha dejado de ser válida. La sociedad se ha reajustado para adoptar nuevas formas de exitencia. La tecnología está en nuestros cuerpos. La supervivencia, en nuestras almas. 
                        <br>    
                            Mexadecimal© es la primera novela de Jesús Ramírez, autor de la revolucionaria Saga MX-Z© que trata sobre una epidemia zombie en México.
                        </p>
                    </div>
                    
                    <div class="book-details">
                        <div class="detail-item">
                            <span class="detail-label">Autor:</span>
                            <span class="detail-value">Jesús Sacramento Ramírez Tapia.</span>
                        </div>
                        <div class="detail-item">
                            <span class="detail-label">Género:</span>
                            <span class="detail-value">Cyberpunk, Ciencia Ficción Mexicana.</span>
                        </div>
                    </div>
                </div>
            </section>

        </main>
        
        <footer>
            <p>© 2020 Jesús Sacramento Ramírez Tapia. Todos los derechos reservados.</p>
            <!--
           <p>.</p> 
        --> 
        </footer>
    </div>
</body>
</html>
