<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rxzwell — Creat0r 0F ARt</title>
  <meta name="description" content="Rxzwell · Broward, Florida · Genre FLuid · Creat0r 0F ARt" />

  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;800&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#05060a;
      --fg:#e6e6ff;
      --neon:#6b7cff;
      --pink:#ff4fd8;
      --cyan:#00f0ff;
      --muted:#9aa0ff;
      --card:rgba(255,255,255,.05);
      --glass:rgba(20,20,40,.55);
      --online:#00ff9c;
      --offline:#444;
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      min-height:100vh;
      font-family:Inter, system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
      color:var(--fg);
      background:
        radial-gradient(1200px 600px at 10% 10%, rgba(0,240,255,.08), transparent 40%),
        radial-gradient(800px 600px at 90% 20%, rgba(255,79,216,.08), transparent 40%),
        linear-gradient(180deg, #04050a, #07081a 60%, #04050a);
      overflow-x:hidden;
    }

    /* Scanlines */
    body::after{
      content:"";
      position:fixed; inset:0;
      pointer-events:none;
      background:repeating-linear-gradient(
        to bottom,
        rgba(255,255,255,.03) 0px,
        rgba(255,255,255,.02) 1px,
        rgba(0,0,0,0) 3px
      );
      mix-blend-mode:overlay;
      opacity:.15;
    }

    .wrap{max-width:1100px;margin:0 auto;padding:28px 20px 80px}

    /* HERO */
    header{text-align:center;padding:24px 0}
    .hero{
      max-width:360px;
      width:100%;
      margin:0 auto 16px;
      border-radius:20px;
      box-shadow:
        0 0 40px rgba(255,79,216,.35),
        0 0 90px rgba(0,240,255,.25);
      animation:float 6s ease-in-out infinite;
    }
    @keyframes float{
      0%,100%{transform:translateY(0)}
      50%{transform:translateY(-6px)}
    }

    .tag{
      font-family:Orbitron;
      letter-spacing:.18em;
      text-transform:uppercase;
      font-size:12px;
      color:var(--muted);
    }

    h1{
      font-family:Orbitron;
      font-weight:800;
      letter-spacing:.1em;
      margin:8px 0 4px;
      text-shadow:0 0 18px rgba(107,124,255,.45);
    }

    .sub{opacity:.9}

    /* Twitch status */
    .twitch-status{
      margin-top:10px;
      display:flex;
      justify-content:center;
      align-items:center;
      gap:10px;
      font-family:Orbitron;
      font-size:12px;
      letter-spacing:.14em;
    }
    .dot{
      width:12px;height:12px;border-radius:50%;background:var(--offline);
    }
    .online{
      background:var(--online);
      box-shadow:0 0 10px rgba(0,255,156,.8),0 0 30px rgba(0,255,156,1);
      animation:pulse 1.8s infinite;
    }
    @keyframes pulse{
      0%{box-shadow:0 0 10px rgba(0,255,156,.6)}
      50%{box-shadow:0 0 30px rgba(0,255,156,1)}
      100%{box-shadow:0 0 10px rgba(0,255,156,.6)}
    }

    /* Cards */
    .cards{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:16px;
      margin:32px 0;
    }
    .card{
      background:var(--glass);
      border:1px solid rgba(255,255,255,.08);
      border-radius:18px;
      padding:16px;
      backdrop-filter:blur(12px);
      box-shadow:0 20px 40px rgba(0,0,0,.4);
    }
    .card h3{font-family:Orbitron;margin:4px 0 10px}

    .links a{
      display:flex;justify-content:space-between;align-items:center;
      padding:10px 12px;margin:8px 0;
      background:rgba(255,255,255,.06);
      border-radius:12px;
      text-decoration:none;color:var(--fg);
      transition:.25s;
    }
    .links a:hover{filter:brightness(1.25);transform:translateX(2px)}

    /* Merch */
    .merch img{
      width:100%;
      border-radius:16px;
      box-shadow:0 0 30px rgba(255,79,216,.25);
    }

    footer{text-align:center;margin-top:40px;opacity:.8}
  </style>
</head>
<body>

<div class="wrap">

  <header>
    <img class="hero" src="https://i.pinimg.com/originals/5R/7V/rv/5R7VrvJ4D.jpg" alt="Rxzwell main artwork" />
    <div class="tag">Broward, Florida · Genre FLuid</div>
    <h1>RXZWELL</h1>
    <div class="sub">Creat0r 0F ARt</div>

    <div class="twitch-status">
      <div class="dot online"></div>
      <div>LIVE ON TWITCH</div>
    </div>
  </header>

  <section class="cards">
    <div class="card">
      <h3>Music</h3>
      <div class="links">
        <a href="https://open.spotify.com/artist/6qmhxNUynVviDvxQRggtFA" target="_blank">Spotify ↗</a>
        <a href="https://on.soundcloud.com/fKI5mvsiiI3ReV02WA" target="_blank">SoundCloud ↗</a>
        <a href="https://youtube.com/@rxzwell" target="_blank">YouTube ↗</a>
        <a href="https://music.apple.com/us/artist/rxzwell/1720338869" target="_blank">Apple Music ↗</a>
      </div>
    </div>

    <div class="card">
      <h3>Social / Streaming</h3>
      <div class="links">
        <a href="https://instagram.com/rxzwell" target="_blank">Instagram ↗</a>
        <a href="https://www.tiktok.com/@rxzwell007" target="_blank">TikTok ↗</a>
        <a href="https://twitch.tv/rxzwell" target="_blank">Twitch ↗</a>
        <a href="https://www.linkedin.com/in/rxzwell-vii-b935922bb/" target="_blank">LinkedIn ↗</a>
      </div>
    </div>

    <div class="card">
      <h3>Album Merch</h3>
      <div class="merch">
        <img src="https://i.pinimg.com/originals/3E/L8/dG/3EL8dGO9n.jpg" alt="Rxzwell merch" />
      </div>
    </div>
  </section>

  <footer>
    <h2>TOUR COMING SOON</h2>
    <small>© Rxzwell</small>
  </footer>

</div>

</body>
</html>
