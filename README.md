<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Realm Defense Clone</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet" />
  <style>
    body {
      font-family: 'Roboto', sans-serif;
    }
    #gameContainer {
      position: relative;
      width: 800px;
      margin: 0 auto;
    }
    #gameCanvas {
      background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80') no-repeat center center;
      background-size: cover;
      border-radius: 0.5rem;
      box-shadow: 0 10px 15px rgba(0,0,0,0.5);
    }
    #uiPanel {
      position: absolute;
      top: 10px;
      left: 10px;
      background: rgba(0,0,0,0.6);
      padding: 10px 15px;
      border-radius: 0.5rem;
      font-size: 16px;
      color: white;
      font-weight: 700;
      user-select: none;
      width: 180px;
    }
    #uiPanel div {
      margin-bottom: 8px;
    }
  </style>
</head>
<body class="bg-gray-900 text-white min-h-screen flex flex-col">
  <header class="p-4 bg-gray-800 shadow-md text-center text-2xl font-bold">
    Realm Defense Clone
  </header>
  <main class="flex-grow flex justify-center items-center p-4">
    <div id="gameContainer">
      <canvas id="gameCanvas" width="800" height="600"></canvas>
      <div id="uiPanel">
        <div id="healthDisplay">Health: 10</div>
        <div id="moneyDisplay">Money: $100</div>
        <div id="waveDisplay">Wave: 1</div>
        <div>Click canvas to place tower ($50)</div>
      </div>
    </div>
  </main>
  <footer class="p-4 bg-gray-800 text-center text-sm text-gray-400">
    &copy; 2024 Realm Defense Clone
  </footer>
  <script src="main.js"></script>
</body>
</html>
