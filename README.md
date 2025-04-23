# mobil-joget
gabut aja
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mobil Joget</title>
  <style>
    body {
      background-color: #1e1e2f;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
      margin: 0;
    }
    .car {
      width: 200px;
      height: 100px;
      background: red;
      border-radius: 20px;
      position: relative;
      animation: dance 1s infinite ease-in-out;
    }
    .car::before, .car::after {
      content: "";
      width: 40px;
      height: 40px;
      background: black;
      border-radius: 50%;
      position: absolute;
      bottom: -20px;
    }
    .car::before {
      left: 20px;
    }
    .car::after {
      right: 20px;
    }
    @keyframes dance {
      0% { transform: translateY(0) rotate(-3deg); }
      25% { transform: translateY(-10px) rotate(3deg); }
      50% { transform: translateY(0) rotate(-3deg); }
      75% { transform: translateY(10px) rotate(3deg); }
      100% { transform: translateY(0) rotate(-3deg); }
    }
  </style>
</head>
<body>
  <div class="car"></div>
  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-buddy.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</body>
</html>
