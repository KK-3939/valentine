<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Cutie 💖</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: 'Comic Sans MS', cursive, sans-serif;
      overflow: hidden;
    }

    .card {
      background: white;
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }

    h1 {
      color: #ff4d6d;
      margin-bottom: 30px;
    }

    button {
      padding: 12px 30px;
      font-size: 18px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      margin: 10px;
      transition: all 0.3s ease;
    }

    #yes {
      background: #ff4d6d;
      color: white;
    }

    #no {
      background: #adb5bd;
      color: white;
      position: absolute;
    }

    #message {
      font-size: 22px;
      color: #ff4d6d;
      margin-top: 20px;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Cutie 💕<br>Will you be my Valentine?</h1>
    <button id="yes" onclick="sayYes()">Yes 💖</button>
    <button id="no">No 🙄</button>
    <div id="message"></div>
  </div>

  <script>
    const noBtn = document.getElementById("no");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });
