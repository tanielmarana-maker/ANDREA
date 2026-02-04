# ANDREA
Pls say yes
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Andrea 💖</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      font-family: Arial, sans-serif;
      text-align: center;
      background-image: url('https://i.imgur.com/2yaf2wb.jpg');
      background-size: cover;
      background-position: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: white;
      text-shadow: 2px 2px 5px black;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 20px;
    }

    .buttons {
      display: flex;
      gap: 20px;
    }

    button {
      font-size: 20px;
      padding: 15px 30px;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    #yesBtn {
      background: #ff4d6d;
      color: white;
      font-size: 22px;
    }

    #noBtn {
      background: #555;
      color: white;
    }

    .minions {
      margin-top: 30px;
    }

    .minions img {
      width: 200px;
    }
  </style>
</head>
<body>

  <h1>Andrea, will you be my Valentine? 💖</h1>

  <div class="buttons">
    <button id="yesBtn">YES 💘</button>
    <button id="noBtn">NO 😢</button>
  </div>

  <div class="minions">
    <img src="https://media.giphy.com/media/3o6Zt481isNVuQI1l6/giphy.gif" alt="Minions with flowers">
  </div>

  <script>
    const yesBtn = document.getElementById("yesBtn");
    const noBtn = document.getElementById("noBtn");

    let yesSize = 22;
    let noClicks = 0;

    noBtn.addEventListener("click", () => {
      noClicks++;
      yesSize += 15;
      yesBtn.style.fontSize = yesSize + "px";
      yesBtn.style.padding = (yesSize / 2) + "px " + (yesSize) + "px";

      if (noClicks >= 3) {
        yesBtn.style.fontSize = "80px";
        yesBtn.style.padding = "40px 80px";
      }
    });

    yesBtn.addEventListener("click", () => {
      document.body.innerHTML = `
        <h1>YAY ANDREA!!! 💕🥰</h1>
        <h2>Happy Valentine's Day! 🌹</h2>
        <img src="https://media.giphy.com/media/l0MYC0LajbaPoEADu/giphy.gif" width="300">
      `;
    });
  </script>

</body>
</html>
