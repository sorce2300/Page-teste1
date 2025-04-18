<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Poker Table</title>
  <style>
    body {
      background: #1e1e1e;
      margin: 0;
      padding: 0;
      font-family: sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .table-container {
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .glow-border {
      position: absolute;
      width: 200px;
      height: 350px;
      border: 30px solid white;
      border-radius: 50% / 25%;
      z-index: 0;
      filter: blur(9px);
      opacity: 0.8;
    }
    .table {
      background: #006400;
      width: 200px;
      height: 350px;
      border: 25px solid #111;
      border-radius: 50% / 25%;
      position: relative;
      z-index: 1;
    }

    .seat {
      position: absolute;
      background: orange;
      border-radius: 50%;
      width: 40px;
      height: 40px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-weight: bold;
      color: #000;
      cursor: pointer;
      z-index: 2;
    }

    .seat:nth-child(1) { top: -80px; left: 50%; transform: translateX(-50%); }
    .seat:nth-child(2) { top: 15%; right: -80px; transform: translateY(-50%); }
    .seat:nth-child(3) { top: 50%; right: -80px; transform: translateY(-50%); }
    .seat:nth-child(4) { bottom: 15%; right: -80px; transform: translateY(50%); }
    .seat:nth-child(5) { bottom: -80px; left: 50%; transform: translateX(-50%); }
    .seat:nth-child(6) { bottom: 15%; left: -80px; transform: translateY(50%); }
    .seat:nth-child(7) { top: 50%; left: -80px; transform: translateY(-50%); }
    .seat:nth-child(8) { top: 15%; left: -80px; transform: translateY(-50%); }

  </style>
</head>
<body>
  <div class="table-container">
    <div class="glow-border"></div>
    <div class="table">
      <div class="seat">SIT1</div>
      <div class="seat">SIT2</div>
      <div class="seat">SIT3</div>
      <div class="seat">SIT4</div>
      <div class="seat">SIT5</div>
      <div class="seat">SIT6</div>
      <div class="seat">SIT7</div>
      <div class="seat">SIT8</div>
    </div>
  </div>
</body>
</html>
