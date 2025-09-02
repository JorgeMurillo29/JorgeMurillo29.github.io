<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para El Amor de Mi Vida, Alison Luna aajajaja</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Montserrat:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        :root{--p-c:#ff69b4;--s-c:#ffc0cb;--t-d-c:#4b0082;--t-l-c:#fff;--a-c:#d81b60;--bg-g-s:#ffebee;--bg-g-e:#fce4ec}
        body{background:linear-gradient(135deg,var(--bg-g-s) 0%,var(--bg-g-e) 100%);font-family:Montserrat,sans-serif;color:var(--t-d-c);display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:100vh;margin:0;text-align:center;overflow:hidden;position:relative}
        body::before{content:'';position:absolute;top:0;left:0;width:100%;height:100%;background-image:url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="30" height="30"><path d="M15 5c2.2 0 4 1.8 4 4 0 2.2-2 3.5-4 5-2-1.5-4-2.8-4-5 0-2.2 1.8-4 4-4z" fill="%23ffc0cb" opacity="0.4"/></svg>');background-repeat:repeat;background-size:30px 30px;animation:backgroundMove 60s linear infinite;opacity:.6;z-index:0}
        @keyframes backgroundMove{from{background-position:0 0}to{background-position:300px 300px}}
        .container{background-color:rgba(255,255,255,.95);padding:40px 30px;border-radius:25px;box-shadow:0 8px 30px rgba(0,0,0,.2);max-width:650px;width:90%;border:3px solid var(--p-c);z-index:10;position:relative;animation:fadeInScale 1s ease-out forwards}
        @keyframes fadeInScale{from{opacity:0;transform:scale(.9)}to{opacity:1;transform:scale(1)}}
        .intro-message{font-family:'Dancing Script',cursive;font-size:1.8em;color:var(--a-c);margin-bottom:10px;animation:fadeIn 1.5s ease-in forwards}
        @keyframes fadeIn{from{opacity:0}to{opacity:1}}
        h1{font-family:'Dancing Script',cursive;font-size:3.5em;color:var(--a-c);margin-bottom:25px;animation:pulse 2s infinite,glow 1.5s ease-in-out infinite alternate;text-shadow:2px 2px 4px rgba(0,0,0,.1)}
        @keyframes pulse{0%{transform:scale(1)}50%{transform:scale(1.03)}100%{transform:scale(1)}}
        @keyframes glow{from{text-shadow:0 0 5px var(--a-c),0 0 10px var(--p-c)}to{text-shadow:0 0 10px var(--a-c),0 0 20px var(--p-c)}}
        p{font-family:Montserrat,sans-serif;font-size:1.3em;line-height:1.7;margin-bottom:35px;color:var(--t-d-c);font-weight:500}
        .question-box{background-color:var(--s-c);padding:25px;border-radius:18px;border:1px solid var(--p-c);margin-top:30px;animation:slideUp .8s ease-out forwards}
        @keyframes slideUp{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}
        .question-box p{font-weight:700;color:var(--a-c);margin-bottom:20px;font-size:1.4em}
        .buttons-container{display:flex;justify-content:center;gap:25px;flex-wrap:wrap}
        .button{background-color:var(--p-c);color:var(--t-l-c);padding:14px 30px;border:none;border-radius:10px;cursor:pointer;font-size:1.1em;font-weight:700;transition:transform .3s ease,background-color .3s ease,box-shadow .3s ease;box-shadow:0 4px 10px rgba(0,0,0,.1)}
        .button:hover{background-color:var(--a-c);transform:translateY(-5px) scale(1.05);box-shadow:0 6px 15px rgba(0,0,0,.2)}
        .heart{position:absolute;background-color:var(--p-c);transform:rotate(-45deg);animation:floatUp 5s forwards;opacity:0;pointer-events:none;z-index:5;box-shadow:0 0 8px var(--p-c)}
        .heart:before,.heart:after{content:'';position:absolute;background-color:var(--p-c);border-radius:50%;width:100%;height:100%}
        .heart:before{top:-50%;left:0}
        .heart:after{left:50%;top:0}
        @keyframes floatUp{0%{transform:translateY(0) rotate(-45deg) scale(0);opacity:0}20%{opacity:.8;transform:translateY(-50px) rotate(-45deg) scale(1)}100%{transform:translateY(-500px) rotate(-45deg) scale(1.5);opacity:0}}
        .marriage-question{display:none;background-color:rgba(255,240,245,.98);padding:40px;border-radius:25px;box-shadow:0 8px 30px rgba(0,0,0,.2);max-width:600px;width:90%;border:3px solid var(--a-c);margin-top:40px;z-index:10;animation:fadeInScale 1s ease-out forwards}
        .marriage-question p{font-family:'Dancing Script',cursive;font-size:2.8em;color:var(--a-c);margin-bottom:30px;text-shadow:1px 1px 3px rgba(0,0,0,.1)}
        .marriage-buttons-container{display:flex;justify-content:center;gap:30px;flex-wrap:wrap}
        .marriage-button{background-color:var(--p-c);color:var(--t-l-c);padding:18px 40px;border:none;border-radius:12px;cursor:pointer;font-size:1.3em;font-weight:700;transition:transform .3s ease,background-color .3s ease,box-shadow .3s ease;box-shadow:0 4px 10px rgba(0,0,0,.1)}
        .marriage-button.no{background-color:#8b0000}
        .marriage-button:hover{background-color:var(--a-c);transform:translateY(-7px) scale(1.08);box-shadow:0 8px 20px rgba(0,0,0,.25)}
        .marriage-button.no:hover{background-color:#690000;transform:translateY(-7px) scale(1.08);box-shadow:0 8px 20px rgba(0,0,0,.25)}
        @media (max-width:768px){h1{font-size:2.8em}p{font-size:1.1em}.button,.marriage-button{padding:12px 25px;font-size:1em}.marriage-question p{font-size:2.2em}}
        @media (max-width:480px){h1{font-size:2.2em}p{font-size:1em}.container,.marriage-question{padding:25px 15px}.buttons-container,.marriage-buttons-container{flex-direction:column;gap:15px}.button,.marriage-button{width:80%;margin:0 auto}.marriage-question p{font-size:1.8em}}
    </style>
</head>
<body>
    <div class="container" id="mainContent">
        <p class="intro-message">Esta página la hice en corto tiempo y con amor para ti, lo que mas me costo fue hacerlo pagina web.</p>
        <h1>El amor que mi corazon anhela, esa eres tu, Alison</h1>
        <p>
            Eres la mujer más bella que he conocido y el amor que siempre he querido tener. Quiero cuidarte, tenerte y amarte toda la vida. Y jamas abandonarte 
        </p>
        <div class="question-box">
            <p>¿Me amas mucho sisi o nono 😔?</p>
            <div class="buttons-container">
                <button class="button" onclick="showMarriageQuestion()">¡Sí, con todo mi corazón!</button>
                <button class="button" onclick="showMarriageQuestion()">¡Claro que sí!</button>
            </div>
        </div>
    </div>

    <div class="marriage-question" id="marriageQuestion">
        <p>Alison, ¿en un futuro sí te casarías conmigo?</p>
        <div class="marriage-buttons-container">
            <button class="marriage-button yes" onclick="alert('Yo se que dirias que si jajaj, quiero que sepas que yo tmb quiero, y ue soy el chico mas feliz, y mi corazoncito se alegra')">¡SÍ, SÍ, SÍ!</button>
            <button class="marriage-button no" onclick="alert('¡No! Esa no es una opción válida, Alison. Dale al otro boton ve, mala, no me amas 😔')">¡NO, NO, NO!</button>
        </div>
    </div>

    <script>
        function createHeart(){const heart=document.createElement('div');heart.classList.add('heart');const size=Math.random()*25+15;heart.style.width=size+'px';heart.style.height=size+'px';heart.style.left=Math.random()*100+'vw';heart.style.bottom='-20px';heart.style.animationDuration=Math.random()*3+4+'s';heart.style.animationDelay=Math.random()*2+'s';document.body.appendChild(heart);setTimeout(()=>heart.remove(),parseFloat(heart.style.animationDuration)*1000+parseFloat(heart.style.animationDelay)*1000)}
        function showMarriageQuestion(){for(let i=0;i<70;i++){setTimeout(createHeart,i*80)}setTimeout(()=>{document.getElementById('mainContent').style.display='none';document.getElementById('marriageQuestion').style.display='block'},1000)}
    </script>
</body>
</html>
