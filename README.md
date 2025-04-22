# Tablero-Mirtha
Tablero de Mirtha contra el mundo 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Tablero Mortal Kombat - Mirtha Legrand</title>
  <style>
    body {
      background-color: #111;
      color: white;
      font-family: Arial, sans-serif;
      text-align: center;
    }
    .board {
      position: relative;
      display: inline-block;
    }
    .character {
      position: absolute;
      border: 2px solid transparent;
    }
    .dead::after {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(255, 0, 0, 0.5);
      background-image: url('https://upload.wikimedia.org/wikipedia/commons/2/2f/Red_X.svg');
      background-repeat: no-repeat;
      background-position: center;
      background-size: 70%;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <h1>El Tablero de Mirtha Legrand</h1>
  <p>Haz clic sobre una persona para marcarla como fallecida.</p>

  <div class="board">
    <img src="A_character_selection_screen_in_the_retro,_pixelat.png" alt="Tablero Mirtha" width="768" height="1152">

    <!-- Posiciones aproximadas de cada personaje (ajustalas según sea necesario) -->
    <div class="character" style="top: 100px; left: 80px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    <div class="character" style="top: 100px; left: 320px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    <div class="character" style="top: 100px; left: 560px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    
    <div class="character" style="top: 250px; left: 80px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    <div class="character" style="top: 250px; left: 560px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    
    <div class="character" style="top: 400px; left: 80px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    <div class="character" style="top: 400px; left: 320px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    <div class="character" style="top: 400px; left: 560px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
    
    <div class="character" style="top: 550px; left: 320px; width: 120px; height: 120px;" onclick="toggleDeath(this)"></div>
  </div>

  <script>
    function toggleDeath(element) {
      element.classList.toggle('dead');
    }
  </script>
</body>
</html>
