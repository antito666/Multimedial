# Multimedial
#### Exploración creativa de arte, tecnologia y medios digitales interactivos.
#### Cultura web y arte digital.

### Index

### Unidad I. Hipervínculo
1. [Mi pagina web.](#ejercicio-1-mi-pagina-web) 

### Unidad II. Programación visual creativa basada en nodos

1. [Intro Touch Designer.](#intro-touchdesigner)


## Unidad I. Hipervínculo

#### Ejercicio 1, Mi pagina web 
[Index:](https://antito666.github.io/Multimedial/w/index.html)

```
<!DOCTYPE html>
<!-- Indica al navegador que este documento usa HTML5 -->

<html lang="es">  
<!-- Inicio del documento HTML -->

<head>
<!-- Sección donde van metadatos, título y estilos -->

<meta charset="UTF-8">
<!-- Define la codificación de caracteres para que se vean bien tildes y símbolos -->

<title>santo.art | Galería</title>
<!-- Título de la página que aparece en la pestaña del navegador -->

<style>
/* Aquí comienza la sección de estilos CSS que define la apariencia visual */      
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

/* Estilo general del cuerpo */

        body {
            font-family: 'times new roman';
            background-color: #ffffff;
            color: #1a1a1a;
            line-height: 3.6;
            display: flex;
            flex-direction: column;
            align-items: center;
        }


       /* Contenedor principal */
        .contenedor {
            width: 100%;
            padding: 60px 40px;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: 200;
            letter-spacing: 8px;
            text-transform: uppercase;
            margin-bottom: 1%;
            text-align: center;
        }

        /* Navegación Minimalista */
        nav {
            margin-bottom: 50px;
        }

        nav a {
            text-decoration: none;
            color: #888;
            font-size: 0.85rem;
            margin: 0 15px;
            text-transform: uppercase;
            letter-spacing: 2px;
            transition: color 0.4s ease;
        }

        nav a:hover {
            color: #000;
        }

        /* Contenedor de Obra Principal */
        .hero-art {
            width: 90%;
            max-width: 600px;
            margin-bottom: 80px;
            overflow: hidden;
        }

        .hero-art img {
            width: 100%;
            height: auto;
            display: block;
            filter: grayscale(20%); /* Toque artístico */
            transition: filter 0.5s ease;
        }

        .hero-art img:hover {
            filter: grayscale(0%);
        }

        /* Pie de página sutil */
        footer {
            padding: 40px;
            font-size: 0.7rem;
            letter-spacing: 1px;
            color: #bbb;
            text-transform: uppercase;
        }

        /* Ajuste para móviles */
        @media (max-width: 600px) {
            header h1 { font-size: 1.8rem; }
            nav a { display: block; margin: 10px 0; }
        }
    </style>
</head>
<body>

    <header>
        <h1>SANTO</h1>
    </header>

    <nav>
        <a href="index.html">Inicio</a>
        <a href="obras.html">Obras</a>
        <a href="contacto.html">Contacto</a>
    </nav>

    <main class="hero-art">
        <img src="img/5.jpg" alt="Obra de Santo">
    </main>

    <footer>
        &copy; 2026 SANTO ART.
    </footer>

</body>
</html>
```
[Obras:](https://antito666.github.io/Multimedial/w/obras.html)
```
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>santo.art | Obra</title>
    <style>
        /* 1. RESET TOTAL */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'times new roman', serif;
            background-color: #ffffff;
            color: #1a1a1a;
            display:block;
            
        }

      
      /* --- MENÚ LATERAL DEFINITIVO --- */
nav {
    width: 200px;
    height: 100vh;
    position: fixed;
    top: 0;
    left: 0;
    padding: 40px;
    display: flex;
    flex-direction: column;
    background: #fff;
    z-index: 100;
}

nav h1 {
    font-weight: 200;
    font-size: 1.2rem;
    letter-spacing: 4px;
    text-transform: uppercase;
    margin-bottom: 40px;
    cursor: pointer;
    color: #000;
    line-height: 1; /* Altura de línea fija para el título */
}

.links {
    display: flex;
    flex-direction: column;
    /* Eliminamos el gap y usamos margin manual para control absoluto */
}

.links a {
    text-decoration: none;
    color: #999;
    text-transform: uppercase;
    font-size: 0.7rem;
    letter-spacing: 2px;
    transition: color 0.3s;
    display: block;      /* Importante para que el margen funcione igual siempre */
    line-height: 1.5;   /* Interlineado fijo en todas las páginas */
    margin-bottom: 12px; /* Espacio fijo entre botones */
}

.links a:hover, .links a.active {
    color: #000;
}

/* Ajuste del contenido principal para que coincida exactamente */
.contenido-principal {
    margin-left: 200px;
    width: calc(100% - 200px);
    padding: 60px 40px;
}

        .serie-titulo {
            font-weight: 200;
            text-transform: uppercase;
            letter-spacing: 6px;
            margin-bottom: 60px;
            font-size: 1rem;
            text-align: center;
        }

        /* 4. GALERÍA (COLOR ORIGINAL) */
        .galeria-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr); 
            gap: 40px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .bloque-obra {
            margin-bottom: 30px;
        }

        .bloque-obra img {
            width: 100%;
            height: auto;
            display: block;
            margin-bottom: 15px;
            transition: transform 0.4s ease;
        }

        .bloque-obra img:hover {
            transform: scale(1.02);
        }

        .info-tecnica {
            text-align: left;
            padding: 0 5px;
        }

        .info-tecnica h2 {
            font-weight: 400;
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 5px;
        }

        .info-tecnica p {
            font-weight: 300;
            font-size: 0.7rem;
            color: #888;
        }

        /* RESPONSIVO */
        @media (max-width: 900px) {
            .galeria-grid { grid-template-columns: 1fr 1fr; }
        }

        @media (max-width: 600px) {
            body { flex-direction: column; }
            nav { width: 100%; height: auto; position: relative; padding: 20px; text-align: center; }
            .links { flex-direction: row; justify-content: center; gap: 20px; }
            .contenido-principal { margin-left: 0; width: 100%; padding: 20px; }
            .galeria-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <nav>
        <h1 onclick="location.href='index.html'">SANTO</h1>
        <div class="links">
            <a href="index.html">Inicio</a>
            <a href="obras.html" class="active">Obras</a>
            <a href="contacto.html">Contacto</a>
        </div>
    </nav>

    <main class="contenido-principal">
        <h2 class="serie-titulo">(re)encarnaciones</h2>

        <div class="galeria-grid">
            <div class="bloque-obra">
                <img src="img/foto.jpg" alt="Obra 1">
                <div class="info-tecnica">
                    <h2>(re)encarnación n 1°</h2>
                    <p>Cartón reciclado y carboncillo</p> 
                    <p>65 x 45 cm. | 2025</p>
                </div>
            </div>

            <div class="bloque-obra">
                <img src="img/2.jpg" alt="Obra 2">
                <div class="info-tecnica">
                    <h2>(re)encarnación n 2°</h2>
                    <p>Cartón reciclado y carboncillo</p> 
                    <p>58 x 44 cm. | 2025</p>
                </div>
            </div>

            <div class="bloque-obra">
                <img src="img/3.jpg" alt="Obra 3">
                <div class="info-tecnica">
                    <h2>(re)encarnación n 3°</h2>
                    <p>Cartón reciclado y carboncillo</p> 
                    <p>47 x 35 cm. | 2025</p>
                </div>
            </div>

            <div class="bloque-obra">
                <img src="img/4.jpg" alt="Obra 4">
                <div class="info-tecnica">
                    <h2>(re)encarnación n 4°</h2>
                    <p>Cartón reciclado y carboncillo</p> 
                    <p>57 x 77 cm. | 2025</p>
                </div>
            </div>
        </div>
    </main>

</body>
</html>
```
[Contacto:](https://antito666.github.io/Multimedial/w/contacto.html)
```
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>santo.art | Contacto</title>
    <style>

        * { 
            margin: 0;
            padding: 0;
            box-sizing: border-box; 
        }

        body { 
            font-family: 'times new roman';
            background-color: #ffffff;
            color: #000;
            display: flex;
            min-height: 100vh; 
        }
    
     /* Menú Lateral */
  
nav {
    width: 200px;
    height: 100vh;
    position: fixed;
    top: 0;
    left: 0;
    padding: 40px;
    display: flex;
    flex-direction: column;
    background: #fff;
    z-index: 100;
}

nav h1 {
    font-weight: 200;
    font-size: 1.2rem;
    letter-spacing: 4px;
    text-transform: uppercase;
    margin-bottom: 40px;
    cursor: pointer;
    color: #000;
}

.links {
    display: flex;
    flex-direction: column;
    gap: 15px; /* Espacio uniforme entre los enlaces */
}

.links a {
    text-decoration: none;
    color: #999;
    text-transform: uppercase;
    font-size: 0.7rem;
    letter-spacing: 2px;
    transition: color 0.3s;
    line-height: 1.2; /* Reset para que no herede el line-height del body */
}

.links a:hover, .links a.active {
    color: #000;
}

/* Ajuste del contenido para que no lo tape el menú */
main, .contenido-principal {
    margin-left: 200px; 
    width: calc(100% - 200px);
    min-height: 100vh;
}

/* Ajuste para móviles */
@media (max-width: 600px) {
    nav { 
        width: 100%; 
        height: auto; 
        position: relative; 
        padding: 20px; 
        text-align: center; 
    }
    .links { 
        flex-direction: row; 
        justify-content: center; 
        gap: 20px; 
    }
    main, .contenido-principal { 
        margin-left: 0; 
        width: 100%; 
    }
}

        /* SECCIÓN DE CONTACTO ÚNICA */
        main {
            margin-left: 220px;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 40px;
        }

        .contacto-container {
            max-width: 500px;
            width: 100%;
        }

        .contacto-container h2 {
            font-weight: 100;
            font-size: 2.5rem;
            letter-spacing: 5px;
            text-transform: uppercase;
            margin-bottom: 40px;
            color: #000;
        }

        .dato-contacto {
            margin-bottom: 40px;
        }

        /* Etiqueta pequeña (Email, Tel, etc) */
        .dato-contacto span {
            display: block;
            font-size: 0.6rem;
            text-transform: uppercase;
            letter-spacing: 3px;
            color: #999;
            margin-bottom: 10px;
        }

        .dato-contacto a {
            text-decoration: none;
            color: #000;
            font-size: 1.2rem;
            font-weight: 300;
            transition: opacity 0.3s;
            border-bottom: 1px solid transparent;
        }

        .dato-contacto a:hover {

            opacity: 0.5;
            border-bottom: 1px solid #000;
        }
    

    </style>
</head>
<body>

    <nav>
        <h1 onclick="location.href='index.html'">SANTO</h1>
        <div class="links">
            <a href="index.html">Inicio</a>
            <a href="obras.html">Obras</a>
            <a href="contacto.html">Contacto</a>
        </div>
    </nav>

    <main>
        <div class="contacto-container">
            <h2>Contacto</h2>

            <div class="dato-contacto">
                <span>Email</span>
                <a href="https://mail.google.com/mail/?view=cm&fs=1&to=s4nto4rt@gmail.com" target="_blank">santo4rt@gmail.com</a>
    </div>

            <div class="dato-contacto">
                <span>Instagram</span>
                <a href="https://www.instagram.com/art__santo/" target="_blank">@art__santo</a>
            </div>
        </div>
    </main>

</body>
</html>
```

## Intro TouchDesigner:

#### [lsystem:](https://drive.google.com/drive/folders/1YOWy3f60O9f4HLP63a-3TfSWbuuSmHxN)
<img src="https://antito666.github.io/Multimedial/w/img/giphytd2.gif" width="auto" height="auto" />

#### [point:](https://drive.google.com/drive/folders/1R6pyLGTVwhnx3ZhugPtKKkZf-Esu_7fe)
<img src="https://antito666.github.io/Multimedial/w/img/giphy.gif" width="auto" height="auto" />
