# Visne-meus-Valentinus-esse
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para Jimena 💖</title>

  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #ffdde1, #ee9ca7);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
      text-align: center;
    }

    .card {
      background: white;
      padding: 30px;
      border-radius: 25px;
      box-shadow: 0 0 20px rgba(0,0,0,0.2);
      max-width: 350px;
      position: relative;
      z-index: 2;
    }

    h1 {
      font-size: 2em;
      color: #e6005c;
      margin-bottom: 10px;
    }

    p {
      font-size: 1.2em;
      color: #333;
    }

    .love-text {
      font-size: 1.3em;
      font-weight: bold;
      color: #ff2e75;
      margin-top: 15px;
    }

    button {
      margin: 15px;
      padding: 12px 25px;
      border: none;
      border-radius: 20px;
      font-size: 1.1em;
      cursor: pointer;
      transition: 0.3s;
    }

    #yesBtn {
      background: #ff4d88;
      color: white;
    }

    #yesBtn:hover {
      background: #e6005c;
    }

    #noBtn {
      background: #555;
      color: white;
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
      bottom: -65px;
    }

    .heart {
      position: absolute;
      font-size: 3em;
      transition: 0.3s;
      z-index: 1;
    }

    a.song-btn {
      display: inline-block;
      background: #ff4d88;
      color: white;
      padding: 12px 20px;
      border-radius: 20px;
      text-decoration: none;
      font-size: 1.1em;
      font-weight: bold;
      margin-top: 15px;
    }

    a.song-btn:hover {
      background: #e6005c;
    }
  </style>
</head>

<body>

  <div class="card">
    <h1>Jimena 💖</h1>

    <p>¿Quieres ser mi San Valentín? 🌹</p>

    <p class="love-text">Te amo mucho Jimena ❤️</p>

    <!-- Botón para abrir canción -->
    <p>🎶 Nuestra canción:</p>

    <a class="song-btn"
      href="https://youtu.be/GfCqMv--ncA?si=QCObzg-9hcDQMke3"
      target="_blank">
      ▶ Escuchar All The Stars 💖
    </a>

    <br><br>

    <button id="yesBtn">Sí 💘</button>
    <button id="noBtn">No 💔</button>
  </div>

  <!-- Corazón que se mueve -->
  <div class="heart" id="heart">❤️</div>

  <script>
    const noBtn = document.getElementById("noBtn");
    const heart = document.getElementById("heart");
    const yesBtn = document.getElementById("yesBtn");

    // Cuando presione NO → el corazón se mueve por la pantalla
    noBtn.addEventListener("click", () => {
      const x = Math.random() * (window.innerWidth - 60);
      const y = Math.random() * (window.innerHeight - 60);

      heart.style.left = x + "px";
      heart.style.top = y + "px";
    });

    // Cuando presione SÍ → mensaje final romántico
    yesBtn.addEventListener("click", () => {
      document.body.innerHTML = `
        <div style="
          color:white;
          font-size:2.5em;
          text-align:center;
          padding:30px;
        ">
          🌹 Sabía que dirías que sí 😭💖<br><br>
          Te amo muchísimo Jimena ❤️✨
        </div>
      `;
    });
  </script>

</body>
</html>
