# Presente-Yasmin0407
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>🎈 Feliz Aniversário, Yasmin!</title>
  <style>
    body {
      font-family: "Segoe UI", sans-serif;
      background: #fff5f5;
      color: #333;
      margin: 0; padding: 0;
      display: flex; align-items: center; justify-content: center;
      min-height: 100vh; text-align: center;
    }
    #locked { max-width: 300px; padding: 30px; background: #fff;
      border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); }
    input { padding: 10px; width: 100px; font-size: 18px;
      margin-top: 10px; text-align: center; }
    #content { display: none; max-width: 500px; padding: 20px;
      background: #fff; border-radius: 10px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1); }
    img { max-width: 100%; margin: 10px 0; border-radius: 8px; }
    .btn { margin: 10px; padding: 12px 20px; border: none;
      border-radius: 50%; font-size: 24px; cursor: pointer; }
    .btn-sim:hover { background: #cceaff; }
    .btn-nao:hover { background: #ffcccc; }
    h1, h2 { color: #a6327c; }
  </style>
</head>
<body>

  <div id="locked">
    <h1>🔐 Acesso Especial</h1>
    <p>Digite o código secreto:</p>
    <input type="password" id="senha" placeholder="0000">
    <button onclick="checkSenha()">Entrar</button>
    <p id="msg" style="color:red;"></p>
  </div>

  <div id="content">
    <h1>🎉 Feliz Aniversário, Yasmin!</h1>
    <p>
      Ela tem um encanto que hipnotiza sem esforço, uma beleza que vai muito além do que se vê...
      O sorriso dela é poesia em forma de luz... e cada gesto carrega doçura e força.
      Ela não precisa tentar ser linda — ela simplesmente é. Linda de um jeito que s&oacute; se sente.
    </p>

    <img src="yasmin1.jpg" alt="Yasmin foto 1">
    <img src="yasmin2.jpg" alt="Yasmin foto 2">

    <h2>🎶 Playlist Daniel Caesar</h2>
    <p>
      <a href="https://open.spotify.com/playlist/37i9dQZF1DX8Tmlu6cSoZ3?si=d62533b5e56648e7"
         target="_blank">
         Toquei essa playlist pensando em você
      </a>
    </p>

    <h2>💖 Me dá uma chance?</h2>
    <button class="btn btn-sim" onclick="resposta('sim')">🧸</button>
    <button class="btn btn-nao" onclick="resposta('não')">❌</button>
    <p id="resp" style="font-size:18px; margin-top:20px;"></p>
  </div>

  <script>
    function checkSenha() {
      const pass = document.getElementById('senha').value;
      if (pass === '0407') {
        document.getElementById('locked').style.display = 'none';
        document.getElementById('content').style.display = 'block';
      } else {
        document.getElementById('msg').innerText = 'Código incorreto. Tente novamente.';
      }
    }
    function resposta(ans) {
      const el = document.getElementById('resp');
      if (ans === 'sim') {
        el.innerText = '🌟 Que alegria, Yasmin!';
      } else {
        el.innerText = '😢 Entendo… mas agradeço por você ter vindo até aqui!';
      }
    }
  </script>
</body>
</html>
