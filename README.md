# Visne-meus-Valentinus-ess(⁠ ⁠◜⁠‿⁠◝⁠ ⁠)⁠♡
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para Jimena 🌌💘</title>

  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      background: radial-gradient(circle at top, #1b2735, #090a0f);
      font-family: "Georgia", serif;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
    }

    .container {
      max-width: 90%;
      padding: 35px;
      border-radius: 20px;
      background: rgba(255, 255, 255, 0.08);
      box-shadow: 0 0 25px rgba(255, 182, 193, 0.4);
      backdrop-filter: blur(8px);
    }

    h1 {
      font-size: 2em;
      margin-bottom: 20px;
      color: #ffb6c1;
    }

    button {
      padding: 15px 35px;
      font-size: 1.3em;
      border: none;
      border-radius: 40px;
      cursor: pointer;
      background: #ff69b4;
      color: white;
      transition: 0.3s;
      box-shadow: 0 0 15px rgba(255, 105, 180, 0.6);
    }

    button:hover {
      transform: scale(1.1);
    }

    #mensajeFinal {
      margin-top: 25px;
      font-size: 1.2em;
      line-height: 1.6;
      color: white;
      display: none;
    }

    #amor {
      font-size: 1.6em;
      color: #ffb6c1;
      margin-bottom: 10px;
    }

    .stars {
      position: absolute;
      width: 2px;
      height: 2px;
      background: white;
      animation: twinkle 2s infinite alternate;
    }

    @keyframes twinkle {
      from { opacity: 0.3; }
      to { opacity: 1; }
    }
  </style>
</head>

<body>

  <div class="container">
    <h1>Visne meus Valentinus esse? 💘</h1>

    <button onclick="clicSi()">Sí</button>

    <div id="mensajeFinal">
      <div id="amor">Te amo mucho Jimena 🌌💖</div>
      <div>
        “En este pequeño universo infinito…  
        siempre termino encontrándote a ti.”
      </div>
    </div>
  </div>

  <script>
    // Estrellitas decorativas
    for (let i = 0; i < 70; i++) {
      let star = document.createElement("div");
      star.className = "stars";
      star.style.top = Math.random() * 100 + "vh";
      star.style.left = Math.random() * 100 + "vw";
      star.style.animationDuration = (Math.random() * 2 + 1) + "s";
      document.body.appendChild(star);
    }

    // Contador de clics
    let intentos = 0;

    function clicSi() {
      intentos++;

      if (intentos < 4) {
        alert("💘 Tocaste 'Sí' (" + intentos + "/4)");
      }

      if (intentos === 4) {
        document.getElementById("mensajeFinal").style.display = "block";
      }
    }
  </script>

</body>
</html>
