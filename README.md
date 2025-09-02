<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Mi Amor Eterno</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Montserrat:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #ff69b4; /* Rosa Corazón */
            --secondary-color: #ffc0cb; /* Rosa Claro */
            --text-dark-color: #4b0082; /* Morado Oscuro */
            --text-light-color: #ffffff; /* Blanco */
            --accent-color: #d81b60; /* Rojo Rosado */
            --bg-gradient-start: #ffebee; /* Rosado muy claro */
            --bg-gradient-end: #fce4ec; /* Otro rosado claro */
        }

        body {
            background: linear-gradient(135deg, var(--bg-gradient-start) 0%, var(--bg-gradient-end) 100%);
            font-family: 'Montserrat', sans-serif;
            color: var(--text-dark-color);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            text-align: center;
            overflow: hidden;
            position: relative;
        }

        /* Animación de fondo de corazones */
        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="30" height="30"><path d="M15 5c2.2 0 4 1.8 4 4 0 2.2-2 3.5-4 5-2-1.5-4-2.8-4-5 0-2.2 1.8-4 4-4z" fill="%23ffc0cb" opacity="0.4"/></svg>');
            background-repeat: repeat;
            background-size: 30px 30px;
            animation: backgroundMove 60s linear infinite;
            opacity: 0.6;
            z-index: 0;
        }

        @keyframes backgroundMove {
            from { background-position: 0 0; }
            to { background-position: 300px 300px; }
        }

        .container {
            background-color: rgba(255, 255, 255, 0.95);
            padding: 40px 30px;
            border-radius: 25px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
            max-width: 650px;
            width: 90%;
            border: 3px solid var(--primary-color);
            z-index: 10;
            position: relative;
            animation: fadeInScale 1s ease-out forwards;
        }

        @keyframes fadeInScale {
            from { opacity: 0; transform: scale(0.9); }
            to { opacity: 1; transform: scale(1); }
        }

        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 3.5em;
            color: var(--accent-color);
            margin-bottom: 25px;
            animation: pulse 2s infinite, glow 1.5s ease-in-out infinite alternate;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.03); }
            100% { transform: scale(1); }
        }

        @keyframes glow {
            from { text-shadow: 0 0 5px var(--accent-color), 0 0 10px var(--primary-color); }
            to { text-shadow: 0 0 10px var(--accent-color), 0 0 20px var(--primary-color); }
        }

        .snoopy-image {
            width: 160px;
            margin-bottom: 25px;
            animation: floatSnoopy 3s ease-in-out infinite alternate;
            filter: drop-shadow(4px 4px 8px rgba(0,0,0,0.2));
        }

        @keyframes floatSnoopy {
            0% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0); }
        }

        p {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.3em;
            line-height: 1.7;
            margin-bottom: 35px;
            color: var(--text-dark-color);
            font-weight: 500;
        }

        .question-box {
            background-color: var(--secondary-color);
            padding: 25px;
            border-radius: 18px;
            border: 1px solid var(--primary-color);
            margin-top: 30px;
            animation: slideUp 0.8s ease-out forwards;
        }

        @keyframes slideUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .question-box p {
            font-weight: bold;
            color: var(--accent-color);
            margin-bottom: 20px;
            font-size: 1.4em;
        }

        .buttons-container {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap; /* Para pantallas pequeñas */
        }

        .button {
            background-color: var(--primary-color);
            color: var(--text-light-color);
            padding: 14px 30px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            font-size: 1.1em;
            font-weight: bold;
            transition: transform 0.3s ease, background-color 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }
        .button:hover {
            background-color: var(--accent-color);
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 6px 15px rgba(0,0,0,0.2);
        }

        /* Estilos para los corazones animados */
        .heart {
            position: absolute;
            background-color: var(--primary-color);
            transform: rotate(-45deg);
            animation: floatUp 5s forwards;
            opacity: 0;
            pointer-events: none;
            z-index: 5;
            box-shadow: 0 0 8px var(--primary-color); /* Pequeño brillo a los corazones */
        }
        .heart:before,
        .heart:after {
            content: "";
            position: absolute;
            background-color: var(--primary-color);
            border-radius: 50%;
            width: 100%;
            height: 100%;
        }
        .heart:before {
            top: -50%;
            left: 0;
        }
        .heart:after {
            left: 50%;
            top: 0;
        }

        @keyframes floatUp {
            0% { transform: translateY(0) rotate(-45deg) scale(0); opacity: 0; }
            20% { opacity: 0.8; transform: translateY(-50px) rotate(-45deg) scale(1); }
            100% { transform: translateY(-500px) rotate(-45deg) scale(1.5); opacity: 0; }
        }

        /* Estilos para la pregunta de matrimonio */
        .marriage-question {
            display: none;
            background-color: rgba(255, 240, 245, 0.98);
            padding: 40px;
            border-radius: 25px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
            max-width: 600px;
            width: 90%;
            border: 3px solid var(--accent-color);
            margin-top: 40px;
            z-index: 10;
            animation: fadeInScale 1s ease-out forwards;
        }
        .marriage-question p {
            font-family: 'Dancing Script', cursive;
            font-size: 2.8em;
            color: var(--accent-color);
            margin-bottom: 30px;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.1);
        }
        .marriage-buttons-container {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
        }
        .marriage-button {
            background-color: var(--primary-color);
            color: var(--text-light-color);
            padding: 18px 40px;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            font-size: 1.3em;
            font-weight: bold;
            transition: transform 0.3s ease, background-color 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }
        .marriage-button.no {
            background-color: #8b0000; /* Rojo oscuro para 'No' */
        }
        .marriage-button:hover {
            background-color: var(--accent-color);
            transform: translateY(-7px) scale(1.08);
            box-shadow: 0 8px 20px rgba(0,0,0,0.25);
        }
        .marriage-button.no:hover {
            background-color: #690000;
            transform: translateY(-7px) scale(1.08);
            box-shadow: 0 8px 20px rgba(0,0,0,0.25);
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.8em;
            }
            p {
                font-size: 1.1em;
            }
            .snoopy-image {
                width: 120px;
            }
            .button, .marriage-button {
                padding: 12px 25px;
                font-size: 1em;
            }
            .marriage-question p {
                font-size: 2.2em;
            }
        }
        @media (max-width: 480px) {
            h1 {
                font-size: 2.2em;
            }
            p {
                font-size: 1em;
            }
            .container, .marriage-question {
                padding: 25px 15px;
            }
            .buttons-container, .marriage-buttons-container {
                flex-direction: column;
                gap: 15px;
            }
            .button, .marriage-button {
                width: 80%;
                margin: 0 auto;
            }
            .marriage-question p {
                font-size: 1.8em;
            }
        }
    </style>
</head>
<body>
    <div class="container" id="mainContent">
        <h1>Mi Amor Eterno</h1>
        <img src="https://www.snoopy.com/images/snoopy_heart.png" alt="Snoopy con corazón" class="snoopy-image">
        <p>
            Eres el amor más bello que tengo y la mujer que siempre he querido tener, mi cielo. Por eso, quiero cuidarte, tenerte cerca, y amarte con toda mi alma... ¡toda la vida!
        </p>
        <div class="question-box">
            <p>¿Me amas mucho?</p>
            <div class="buttons-container">
                <button class="button" onclick="showMarriageQuestion()">¡Sí, con todo mi corazón!</button>
                <button class="button" onclick="showMarriageQuestion()">¡Claro que sí, mi amor!</button>
            </div>
        </div>
    </div>

    <div class="marriage-question" id="marriageQuestion">
        <p>Mi vida... ¿Te casarías conmigo? ¡Sí o No!</p>
        <div class="marriage-buttons-container">
            <button class="marriage-button yes" onclick="alert('¡¡¡SABÍA QUE DIRÍAS QUE SÍ!!! ¡Me haces el hombre más feliz del mundo! ¡Te amo con locura, mi futura esposa!')">¡SÍ, SÍ, SÍ!</button>
            <button class="marriage-button no" onclick="alert('¡Ah, no! Esa no es una opción válida, mi amor. 😉 Por favor, dale al otro botón. ¡Sé que quieres! ❤️')">¡NO, NO, NO!</button>
        </div>
    </div>

    <script>
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            const size = Math.random() * 25 + 15; // Corazones de 15px a 40px
            heart.style.width = size + 'px';
            heart.style.height = size + 'px';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.bottom = '-20px'; // Empiezan un poco más abajo
            heart.style.animationDuration = Math.random() * 3 + 4 + 's'; // Duración de 4 a 7 segundos
            heart.style.animationDelay = Math.random() * 2 + 's'; // Retraso para que no salgan todos a la vez
            document.body.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, parseFloat(heart.style.animationDuration) * 1000 + parseFloat(heart.style.animationDelay) * 1000);
        }

        function showMarriageQuestion() {
            // Generar muchos corazones
            for (let i = 0; i < 70; i++) { // Más corazones
                setTimeout(createHeart, i * 80); // Corazones salen más rápido
            }

            // Ocultar el contenido principal y mostrar la pregunta de matrimonio
            setTimeout(() => { // Pequeño retraso para que se vean los corazones
                document.getElementById('mainContent').style.display = 'none';
                document.getElementById('marriageQuestion').style.display = 'block';
            }, 1000); // 1 segundo después de los primeros corazones
        }
    </script>
</body>
</html>
