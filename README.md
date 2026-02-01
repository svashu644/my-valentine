<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Will You Be My Valentine?</title>
  <style>
    body {
      background: #ffd6e7;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: Arial, sans-serif;
    }

    .card {
      background: #fff;
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      width: 320px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.1);
    }

    .emoji {
      font-size: 60px;
      margin-bottom: 15px;
    }

    h2 {
      margin-bottom: 30px;
    }

    button {
      padding: 10px 22px;
      border: none;
      border-radius: 20px;
      font-size: 16px;
      cursor: pointer;
      margin: 10px;
    }

    #yes {
      background: #ff4d88;
      color: white;
    }

    #no {
      background: #ddd;
      position: absolute;
    }

    .container {
      position: relative;
      height: 200px;
    }
  </style>
</head>
<body>

  <div class="card">
    <div class="emoji">🐣💗</div>
    <h2>Khushi, will you be my Valentine?</h2>

    <div class="container">
      <button id="yes" onclick="yesClicked()">Yes</button>
      <button id="no" onmouseover="moveNo()">No</button>
    </div>
  </div>

  <script>
    function moveNo() {
      const noBtn = document.getElementById("no");
      const x = Math.random() * 200;
      const y = Math.random() * 100;

      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    }

    function yesClicked() {
      alert("Yayyy 💖 See you on Valentine’s Day 😘");
    }
  </script>

</body>
</html>
