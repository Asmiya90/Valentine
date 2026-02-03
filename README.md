# Valentine<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Be My Valentine 💖</title>
  <style>
    body {
      background: linear-gradient(135deg, #ffd6e8, #ff9ecb);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      overflow: hidden;
    }
    .card {
      background: white;
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
      position: relative;
    }
    h1 {
      color: #ff4d88;
    }
    .buttons {
      margin-top: 25px;
      position: relative;
      height: 80px;
    }
    button {
      padding: 12px 30px;
      font-size: 18px;
      border-radius: 30px;
      border: none;
      cursor: pointer;
      margin: 10px;
      position: absolute;
    }
    .yes {
      background: #ff4d88;
      color: white;
      left: 20px;
    }
    .no {
      background: #ccc;
      color: #666;
      right: 20px;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Will you be my Valentine? 💕</h1>
    <p>You make my heart smile 🥺💖</p>

    <div class="buttons">
      <button class="yes" onclick="alert('YAY!!! 💖🌸 I knew it 😍')">
        Yes 💘
      </button>

      <button class="no" id="noBtn">
        No 🙃
      </button>
    </div>
  </div>

  <script>
    const noBtn = document.getElementById("noBtn");
    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 60 - 30;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    });
  </script>

</body>
</html>
