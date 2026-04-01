<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For You ❤️</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: pink;
      font-family: Arial, sans-serif;
      text-align: center;
    }

    h1 {
      font-size: 2.5rem;
    }

    .buttons {
      margin-top: 20px;
    }

    button {
      padding: 10px 20px;
      font-size: 18px;
      border: none;
      border-radius: 10px;
      margin: 10px;
      cursor: pointer;
    }

    #yes {
      background: #ff4d6d;
      color: white;
    }

    #no {
      background: white;
    }
  </style>
</head>
<body>

  <div>
    <h1>Will you be mine? ❤️</h1>
    <div class="buttons">
      <button id="yes">Yes 😍</button>
      <button id="no">No 😢</button>
    </div>
  </div>

  <script>
    const noBtn = document.getElementById("no");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * window.innerWidth - 100;
      const y = Math.random() * window.innerHeight - 50;
      noBtn.style.position = "absolute";
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    document.getElementById("yes").onclick = () => {
      document.body.innerHTML = "<h1>Yayyy ❤️ I knew it 😍</h1>";
    };
  </script>

</body>
</html>
