<!DOCTYPE html>
<html lang="no">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Maten i bryllupet</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Open+Sans:wght@400;600&display=swap');

    body {
      margin: 0;
      font-family: 'Open Sans', sans-serif;
      background: linear-gradient(135deg, #fff0f5, #f0fff0);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .container {
      background: rgba(255, 255, 255, 0.9);
      padding: 2rem 3rem;
      border-radius: 20px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.15);
      text-align: center;
      max-width: 500px;
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      color: #b22222;
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    ul {
      list-style: none;
      padding: 0;
      font-size: 1.2rem;
      color: #333;
    }

    li {
      margin: 0.5rem 0;
      position: relative;
    }

    li::before {
      content: "💖";
      position: absolute;
      left: -2rem;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Maten i bryllupet</h1>
    <ul id="meny"></ul>
  </div>

  <script>
    // Her kan du enkelt endre menyen:
    const meny = [
      "Forrett: Bruschetta med tomat og basilikum",
      "Hovedrett: Lammeskank med rotgrønnsaker",
      "Dessert: Sjokolademousse med bringebær"
    ];

    const ul = document.getElementById("meny");
    meny.forEach(ret => {
      const li = document.createElement("li");
      li.textContent = ret;
      ul.appendChild(li);
    });
  </script>
</body>
</html>
