<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>スターくんRPG公式サイト</title>
  <style>
    body {
      margin: 0;
      font-family: "Noto Sans JP", sans-serif;
      background: radial-gradient(ellipse at bottom, #0b0d26 0%, #000 100%);
      color: white;
      overflow-x: hidden;
    }

    header {
      text-align: center;
      padding: 2rem;
      background: rgba(255,255,255,0.05);
      box-shadow: 0 0 10px rgba(255,255,255,0.2);
    }

    h1 {
      font-size: 2.5rem;
      letter-spacing: 2px;
      color: #ffd700;
      text-shadow: 0 0 15px #ffd700, 0 0 25px #ff9;
    }

    .stars {
      position: fixed;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      background: transparent url('https://www.transparenttextures.com/patterns/stardust.png') repeat;
      z-index: -1;
      animation: moveStars 100s linear infinite;
    }

    @keyframes moveStars {
      from { background-position: 0 0; }
      to { background-position: -10000px 5000px; }
    }

    section {
      padding: 3rem 1.5rem;
      max-width: 800px;
      margin: auto;
      text-align: center;
    }

    h2 {
      color: #ffd700;
      text-shadow: 0 0 10px #ffd700;
    }

    button {
      background: #ffd700;
      border: none;
      border-radius: 10px;
      padding: 1rem 2rem;
      margin-top: 1rem;
      cursor: pointer;
      font-size: 1.2rem;
      box-shadow: 0 0 20px #ff0;
      transition: all 0.2s;
    }

    button:hover {
      background: #fff066;
      transform: scale(1.05);
    }

    footer {
      text-align: center;
      padding: 2rem;
      font-size: 0.9rem;
      color: #ccc;
    }

    audio {
      margin-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="stars"></div>
  <header>
    <h1>⭐スターくんRPG公式サイト⭐</h1>
    <p>〜 光と闇の戦いが、今はじまる 〜</p>
  </header>

  <section>
    <h2>🎮 ゲームをプレイ</h2>
    <p>ブラウザで遊べるRPG！スターくんの冒険へ出発！</p>
    <button onclick="location.href='game/index.html'">ゲームスタート！</button>
  </section>

  <section>
    <h2>💫 スターくんとは？</h2>
    <p>
      星の力を持つ少年。優しいが、仲間と世界を守るために戦う。<br>
      最大の敵は、かつての自分の心「ダークスター」…。
    </p>
  </section>

  <section>
    <h2>🎵 BGMを再生</h2>
    <audio controls loop>
      <source src="assets/bgm/star_theme.mp3" type="audio/mpeg">
      お使いのブラウザはオーディオをサポートしていません。
    </audio>
  </section>

  <footer>
    © 2025 スターくん制作チーム | fan project
  </footer>
</body>
</html>
