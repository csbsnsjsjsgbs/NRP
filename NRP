index.html<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>MyGameTwin</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Segoe UI', sans-serif; background: #0f0f0f; color: #ccc; line-height: 1.6; transition: background 0.3s, color 0.3s; }
    header { background: #111; padding: 1rem 2rem; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; z-index: 1000; }
    header h1 { color: #00ffd5; }
    nav a { color: #ccc; margin-left: 20px; text-decoration: none; transition: color 0.2s; }
    nav a:hover { color: #00ffd5; }
    .container { padding: 2rem; max-width: 1000px; margin: auto; }
    section { margin: 3rem 0; }
    .upload-box, .simulation-box, .leaderboard-box { background: #1a1a1a; padding: 2rem; border-radius: 10px; box-shadow: 0 0 10px #00ffd533; }
    input[type="file"] { background: #222; color: #ccc; border: 1px solid #444; padding: 0.5rem; border-radius: 5px; }
    button { background: #00ffd5; color: #000; border: none; padding: 0.7rem 1.5rem; border-radius: 5px; cursor: pointer; margin-top: 1rem; }
    .dark-mode-toggle { cursor: pointer; background: none; border: none; color: #00ffd5; font-size: 1rem; }
    table { width: 100%; border-collapse: collapse; margin-top: 1rem; }
    th, td { padding: 1rem; border-bottom: 1px solid #333; text-align: left; }
    th { color: #00ffd5; }
    footer { text-align: center; padding: 2rem; color: #555; font-size: 0.9rem; }
    .dark body { background: #fff; color: #111; }
    .dark header, .dark .upload-box, .dark .simulation-box, .dark .leaderboard-box { background: #f0f0f0; color: #111; }
    .dark nav a { color: #111; }
  </style>
</head>
<body>
  <header>
    <h1>MyGameTwin</h1>
    <nav>
      <a href="#upload">Upload</a>
      <a href="#simulate">Simulate</a>
      <a href="#leaderboard">Leaderboard</a>
      <button class="dark-mode-toggle" onclick="toggleDarkMode()">🌓</button>
    </nav>
  </header>

  <div class="container">
    <section id="upload" class="upload-box">
      <h2>🎥 Upload Your Gameplay</h2>
      <p>Upload FC 25, Fortnite, or Valorant footage to train your AI clone.</p>
      <input type="file" accept="video/*" />
      <button>Start Clone Training</button>
    </section>

    <section id="simulate" class="simulation-box">
      <h2>🤖 Simulate Your Clone</h2>
      <p>Preview a 1v1 simulation of your AI twin vs another player’s clone.</p>
      <video controls width="100%" style="margin-top: 1rem;" src="https://www.w3schools.com/html/mov_bbb.mp4"></video>
    </section>

    <section id="leaderboard" class="leaderboard-box">
      <h2>🏆 Top GameTwins</h2>
      <table>
        <thead>
          <tr><th>Rank</th><th>Gamer</th><th>Game</th><th>Clone Rating</th></tr>
        </thead>
        <tbody>
          <tr><td>1</td><td>ShadowX</td><td>FC 25</td><td>98</td></tr>
          <tr><td>2</td><td>NovaAim</td><td>Valorant</td><td>95</td></tr>
          <tr><td>3</td><td>TurboBuildz</td><td>Fortnite</td><td>93</td></tr>
        </tbody>
      </table>
    </section>
  </div>

  <footer>© 2025 MyGameTwin — Built with game love 💙</footer>

  <script>
    function toggleDarkMode() {
      document.body.classList.toggle('dark');
    }
  </script>
</body>
</html>
