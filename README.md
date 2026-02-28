<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Virtual Flower Letter 🌸</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .container {
      background: white;
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      text-align: center;
      width: 320px;
    }

    .flower {
      font-size: 80px;
      animation: float 2s infinite ease-in-out;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    textarea {
      width: 100%;
      height: 80px;
      margin-top: 10px;
      border-radius: 10px;
      border: 1px solid #ccc;
      padding: 10px;
      font-size: 14px;
    }

    button {
      margin-top: 10px;
      padding: 10px 20px;
      border: none;
      border-radius: 10px;
      background: #ff4d6d;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background: #e63950;
    }

    .letter {
      margin-top: 15px;
      padding: 10px;
      border-radius: 10px;
      background: #fff0f3;
      min-height: 50px;
      white-space: pre-wrap;
    }

    .share {
      margin-top: 10px;
      font-size: 12px;
      color: gray;
    }
  </style>
</head>
<body>

<div class="container">
  <div class="flower">🌸</div>

  <h3>Write your letter 💌</h3>

  <textarea id="inputLetter" placeholder="Type your message..."></textarea>

  <button onclick="generateLetter()">Generate Flower Letter</button>

  <div class="letter" id="outputLetter"></div>

  <div class="share">Share this page link with someone special ❤️</div>
</div>

<script>
  function generateLetter() {
    const text = document.getElementById("inputLetter").value;
    document.getElementById("outputLetter").innerText = text;
  }
</script>

</body>
</html>
