<!DOCTYPE html>
<html lang="mn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday, Sweetie!</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #FFDEE9, #B5FFFC);
      font-family: 'Comic Sans MS', cursive, sans-serif;
      overflow: hidden;
      position: relative;
    }
    #container {
      text-align: center;
      z-index: 1;
    }
    #clickBtn {
      padding: 12px 24px;
      font-size: 20px;
      border: none;
      border-radius: 12px;
      background-color: #FFB6C1;
      color: white;
      cursor: pointer;
      transition: 0.3s;
    }
    #clickBtn:hover {
      background-color: #FF69B4;
    }
    #message {
      font-size: 28px;
      margin-top: 20px;
      display: none;
    }
    #bunny {
      font-size: 60px;
      margin-bottom: 10px;
      display: block;
    }
    .confetti {
      position: absolute;
      border-radius: 50%;
      top: -10px;
      animation-name: fall, swing;
      animation-duration: 3s, 2s;
      animation-iteration-count: 1, infinite;
      animation-timing-function: linear, ease-in-out;
    }
    @keyframes fall {
      0% { transform: translateY(0);}
      100% { transform: translateY(100vh);}
    }
    @keyframes swing {
      0% { transform: translateX(0);}
      50% { transform: translateX(20px);}
      100% { transform: translateX(0);}
    }
  </style>
</head>
<body>
  <div id="container">
    <span id="bunny">🐰</span>
    <button id="clickBtn">Энд дар 🐇👉</button>
    <div id="message">🎉 Happy Birthday, Sweetie! 🎂</div>
  </div>

  <script>
    const btn = document.getElementById("clickBtn");
    const msg = document.getElementById("message");

    btn.addEventListener("click", () => {
      msg.style.display = "block";

      for (let i = 0; i < 100; i++) {  // confetti-гийн тоог нэмсэн
        const conf = document.createElement("div");
        conf.classList.add("confetti");
        conf.style.left = Math.random() * window.innerWidth + "px";
        conf.style.backgroundColor = `hsl(${Math.random()*360}, 70%, 60%)`;
        conf.style.width = conf.style.height = Math.random() * 12 + 8 + "px";
        conf.style.animationDelay = Math.random() * 2 + "s";
        conf.style.animationDuration = 3 + Math.random() * 2 + "s, " + (2 + Math.random()*2) + "s";
        document.body.appendChild(conf);
        setTimeout(() => { conf.remove(); }, 5000);
      }
    });
  </script>
</body>
</html>
