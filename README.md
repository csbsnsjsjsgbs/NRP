<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>GameTwin Arena</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    :root {
      --bg: #0e0e0e;
      --text: #00ffee;
      --accent: #ffee00;
      --card: #1a1a1a;
    }

  [data-theme="light"] {
      --bg: #f5f5f5;
      --text: #003344;
      --accent: #0055ff;
      --card: #ffffff;
    }

   body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      transition: all 0.4s ease;
    }

  header {
      background: var(--card);
      padding: 20px;
      text-align: center;
      font-size: 28px;
      font-weight: bold;
      box-shadow: 0 0 12px var(--text);
      position: sticky;
      top: 0;
      z-index: 100;
    }

   #toggleTheme {
      position: absolute;
      right: 20px;
      top: 20px;
      background: var(--accent);
      color: #000;
      border: none;
      padding: 8px 16px;
      font-weight: bold;
      cursor: pointer;
      border-radius: 6px;
    }

  main {
      padding: 30px;
      max-width: 900px;
      margin: auto;
    }

  h2 {
      color: var(--accent);
    }

   .upload-box {
      border: 2px dashed var(--text);
      padding: 30px;
      border-radius: 12px;
      background-color: var(--card);
      text-align: center;
      transition: 0.3s;
    }

  input[type="file"] {
      margin-top: 15px;
    }

   button.action {
      background: var(--accent);
      color: #000;
      padding: 10px 20px;
      font-weight: bold;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 15px;
    }

   button.action:hover {
      background-color: #ff0;
    }

   .results {
      margin-top: 40px;
      background: var(--card);
      padding: 20px;
      border-radius: 10px;
      display: none;
      box-shadow: 0 0 15px var(--text);
    }

  .results div {
      margin: 8px 0;
    }

   footer {
      text-align: center;
      padding: 40px 0 20px;
      font-size: 14px;
      color: #888;
    }

   /* Optional animated background glow */
    body::before {
      content: "";
      position: fixed;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle at center, var(--accent), transparent 70%);
      animation: glow 8s infinite alternate ease-in-out;
      z-index: -1;
      opacity: 0.03;
    }

   @keyframes glow {
      0% { transform: scale(1); }
      100% { transform: scale(1.2); }
    }
  </style>
</head>
<body>

  <header>
    🎮 GameTwin Arena
    <button id="toggleTheme">Toggle Mode</button>
  </header>

  <main>
    <h2>Upload Your Gameplay</h2>
    <p>Create your AI-powered game twin and simulate battles against other players.</p>
  </main>

  <footer>© 2025 GameTwin Arena — Powered by AI & You</footer>

  <script>
    function showResults() {
      const fileInput = document.getElementById('upload');
      if (!fileInput.files.length) {
        alert("Please upload a gameplay file first.");
        return;
      }
      document.getElementById('results').style.display = 'block';
    }

    // Theme toggle
    const btn = document.getElementById('toggleTheme');
    btn.addEventListener('click', () => {
      const current = document.body.getAttribute("data-theme");
      if (current === "light") {
        document.body.removeAttribute("data-theme");
      } else {
        document.body.setAttribute("data-theme", "light");
      }
    });
  </script>

</body>
</html>
