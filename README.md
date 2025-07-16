<!DOCTYPE html>
<html lang="hu">
<head>
  <meta charset="UTF-8">
  <title>Ki az Imposztor?</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div id="game">
    <h1>🎭 Ki az Imposztor?</h1>
    <div id="setup">
      <label>Játékosok nevei (vesszővel elválasztva):</label><br>
      <input type="text" id="playersInput" placeholder="Anna, Bence, Csaba"><br><br>

      <label>Imposztorok száma:</label>
      <input type="number" id="imposterCount" min="1" max="3" value="1"><br><br>

      <label>Nehézség:</label>
      <select id="difficulty">
        <option value="easy">Könnyű</option>
        <option value="hard">Nehéz</option>
      </select><br><br>

      <label>Időkorlát (másodperc, 0 = kikapcsolva):</label>
      <input type="number" id="timeLimit" min="0" value="0"><br><br>

      <button onclick="startGame()">Játék indítása</button>
    </div>

    <div id="round" style="display:none;">
      <h2 id="playerName"></h2>
      <p id="roleInfo"></p>
      <button onclick="nextPlayer()">Tovább</button>
    </div>

    <div id="gameEnd" style="display:none;">
      <h2>🎉 Játék vége!</h2>
      <p>Szavazzatok, ki volt az Imposztor!</p>
      <button onclick="location.reload()">Új játék</button>
    </div>
  </div>
  <script src="script.js"></script>
</body>
</html># Ki-az-Imposztor-
