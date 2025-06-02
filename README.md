<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kelompok 4</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #e6f0ff;
      margin: 0;
      padding: 0;
      text-align: center;
    }
    h1 {
      background-color: #0073e6;
      color: white;
      padding: 20px;
    }
    .container {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
      margin: 30px;
    }
    .card {
      background-color: white;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      padding: 20px;
      width: 200px;
      cursor: pointer;
      transition: 0.3s;
    }
    .card:hover {
      transform: scale(1.05);
      background-color: #f0f8ff;
    }
    .info {
      display: none;
      margin-top: 10px;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <h1>Kelompok 4</h1>
  <div class="container">
    <div class="card" onclick="showInfo(this)">
      <strong>Nama 1</strong>
      <div class="info">NBI: 123456789</div>
    </div>
    <div class="card" onclick="showInfo(this)">
      <strong>Nama 2</strong>
      <div class="info">NBI: 987654321</div>
    </div>
    <div class="card" onclick="showInfo(this)">
      <strong>Nama 3</strong>
      <div class="info">NBI: 112233445</div>
    </div>
    <div class="card" onclick="showInfo(this)">
      <strong>Nama 4</strong>
      <div class="info">NBI: 556677889</div>
    </div>
  </div>

  <script>
    function showInfo(card) {
      const infos = document.querySelectorAll(".info");
      infos.forEach(i => i.style.display = "none");
      card.querySelector(".info").style.display = "block";
    }
  </script>
</body>
</html>
