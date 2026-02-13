# Valentines-for-Eunice
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Happy Valentine’s Day, Eunice ❤️</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      min-height: 100vh;
      overflow-x: hidden;
      color: #fff;
      text-align: center;
    }

    .container {
      padding: 80px 20px;
      max-width: 800px;
      margin: auto;
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 20px;
    }

    h2 {
      font-size: 1.8rem;
      margin-bottom: 30px;
      font-weight: 400;
    }

    .card {
      background: rgba(255, 255, 255, 0.15);
      backdrop-filter: blur(10px);
      border-radius: 20px;
      padding: 40px 30px;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
      margin-top: 40px;
    }

    p {
      font-size: 1.2rem;
      line-height: 1.8;
      margin-bottom: 20px;
    }

    .signature {
      margin-top: 30px;
      font-size: 1.3rem;
      font-style: italic;
    }

    button {
      margin-top: 30px;
      padding: 15px 35px;
      border: none;
      border-radius: 30px;
      background: #fff;
      color: #ff4f81;
      font-size: 1.1rem;
      cursor: pointer;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    button:hover {
      transform: translateY(-3px);
      box-shadow: 0 10px 20px rgba(0,0,0,0.2);
    }

    /* Floating hearts */
    .heart {
      position: fixed;
      bottom: -20px;
      font-size: 24px;
      animation: floatUp 6s linear infinite;
      opacity: 0.8;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) scale(1);
        opacity: 0;
      }
      10% {
        opacity: 0.8;
      }
      100% {
        transform: translateY(-120vh) scale(1.5);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>Happy Valentine’s Day ❤️</h1>
    <h2>Eunice, this is for you</h2>

    <div class="card">
      <p>
        Dear Eunice,
      </p>
      <p>
        From the moment you came into my life, everything felt brighter, warmer,
        and more meaningful. You have a way of making ordinary moments feel special
        just by being you.
      </p>
      <p>
        This little website is a small reminder of how loved, appreciated,
        and cherished you are — not just today, but every single day.
      </p>
      <p>
        Thank you for your kindness, your smile, and the happiness you bring into
        my world.
      </p>

      <div class="signature">
        With all my love ❤️
      </div>

      <button onclick="showMessage()">Click for a Surprise 💌</button>
    </div>
  </div>

  <script>
    function showMessage() {
      alert("Eunice, you are my favorite person in the world 💖");
    }

    // Floating hearts generator
    setInterval(() => {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.innerText = "❤️";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (4 + Math.random() * 3) + "s";
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 7000);
    }, 400);
  </script>

</body>
</html>
