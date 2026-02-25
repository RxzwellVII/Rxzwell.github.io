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

  <!-- Base Styles -->
  <style>
    :root{
      --bg:#05060a;
      --fg:#e6e6ff;
      --neon:#6b7cff;
      --pink:#ff4fd8;
      --cyan:#00f0ff;
      --muted:#9aa0ff;
      --card:rgba(255,255,255,.04);
      --glass:rgba(20,20,40,.55);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      color:var(--fg);
      background:
        radial-gradient(1200px 600px at 10% 10%, rgba(0,240,255,.08), transparent 40%),
        radial-gradient(800px 600px at 90% 20%, rgba(255,79,216,.08), transparent 40%),
        linear-gradient(180deg, #04050a, #07081a 60%, #04050a);
      font-family:Inter, system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
      overflow-x:hidden;
    }

    /* Scanlines + subtle distortion */
    body::after{
      content:"";
      position:fixed; inset:0;
      pointer-events:none;
      background:
        repeating-linear-gradient(
          to bottom,
          rgba(255,255,255,.03) 0px,
          rgba(255,255,255,.02) 1px,
          rgba(0,0,0,0) 3px
        );
      mix-blend-mode:overlay;
      animation:scan 6s linear infinite;
    }
    @keyframes scan{0%{opacity:.12}50%{opacity:.2}100%{opacity:.12}}

    /* Cursor: cat with laser eyes */
    .cursor{
      position:fixed; left:0; top:0; width:36px; height:36px; pointer-events:none; z-index:9999;
      transform:translate(-50%,-50%);
      filter:drop-shadow(0 0 10px rgba(0,240,255,.8));
    }
    .cursor svg{width:100%; height:100%}
    .laser{
      animation:laser 1.2s linear infinite;
      transform-origin:0 50%;
    }
    @keyframes laser{
      0%{opacity:.2}50%{opacity:1}100%{opacity:.2}
    }

    /* Layout */
    .wrap{max-width:1100px; margin:0 auto; padding:28px 20px 80px}
    header{
      display:grid; gap:18px; align-items:center; text-align:center; padding:28px 0 10px;
    }
    .tag{
      font-family:Orbitron; letter-spacing:.18em; text-transform:uppercase;
      color:var(--muted); font-size:12px
    }
    h1{
      font-family:Orbitron; font-weight:800; letter-spacing:.08em; margin:6px 0 4px;
      text-shadow:0 0 18px rgba(107,124,255,.45);
    }
    .glitch{
      position:relative; display:inline-block;
    }
    .glitch::before,.glitch::after{
      content:attr(data-text); position:absolute; inset:0;
      mix-blend-mode:screen; opacity:.7
    }
    .glitch::before{transform:translate(2px, -1px); color:var(--cyan)}
    .glitch::after{transform:translate(-2px, 1px); color:var(--pink)}
    .sub{color:#cfd2ff; opacity:.9}

    .cards{display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:16px; margin:28px 0}
    .card{
      background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02));
      border:1px solid rgba(255,255,255,.08);
      border-radius:18px; padding:16px 16px 18px; backdrop-filter: blur(10px);
      box-shadow:0 20px 40px rgba(0,0,0,.35);
      transition:transform .25s ease, box-shadow .25s ease;
    }
    .card:hover{transform:translateY(-4px); box-shadow:0 30px 70px rgba(0,0,0,.5)}
    .card h3{font-family:Orbitron; margin:4px 0 10px}
    .links a{
      display:flex; align-items:center; justify-content:space-between; gap:10px;
      padding:10px 12px; margin:8px 0; border-radius:12px; text-decoration:none; color:var(--fg);
      background:var(--glass); border:1px solid rgba(255,255,255,.08);
      transition:filter .2s ease, transform .2s ease;
    }
    .links a:hover{filter:brightness(1.2); transform:translateX(2px)}

    .embed{
      margin:24px 0 10px; padding:14px; border-radius:16px; background:var(--card);
      border:1px solid rgba(255,255,255,.08)
    }

    /* Merch */
    .merch{
      display:grid; grid-template-columns:repeat(auto-fit,minmax(160px,1fr)); gap:14px; margin-top:10px
    }
    .ph{
      aspect-ratio:1/1; border-radius:14px; background:
        linear-gradient(135deg, rgba(107,124,255,.25), rgba(255,79,216,.25));
      border:1px dashed rgba(255,255,255,.25);
      display:grid; place-items:center; color:#fff; opacity:.8
    }

    footer{
      margin-top:40px; text-align:center; color:#b9bcff; opacity:.8
    }

    /* Flicker */
    .flicker{animation:flicker 3s infinite}
    @keyframes flicker{
      0%,19%,22%,62%,64%,70%,100%{opacity:1}
      20%,21%,63%,69%{opacity:.6}
    }
  </style>
</head>
<body>
  <!-- Custom Cursor -->
  <div class="cursor" id="cursor">
    <svg viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
      <circle cx="32" cy="32" r="16" fill="#111" stroke="#6b7cff"/>
      <path d="M20 24 L16 16 M44 24 L48 16" stroke="#6b7cff" stroke-width="3" stroke-linecap="round"/>
      <circle cx="26" cy="32" r="2" fill="#00f0ff"/>
      <circle cx="38" cy="32" r="2" fill="#ff4fd8"/>
      <rect class="laser" x="40" y="31" width="24" height="2" fill="#ff4fd8"/>
      <rect class="laser" x="0" y="31" width="24" height="2" fill="#00f0ff"/>
    </svg>
  </div>

  <div class="wrap">
    <header>
      <img src="/mnt/data/openart-image_apCxoAPn_1768320325579_raw.jpg" alt="Rxzwell main artwork" style="max-width:320px;width:100%;border-radius:18px;box-shadow:0 0 40px rgba(255,79,216,.35),0 0 80px rgba(0,240,255,.25);margin:0 auto 12px;display:block" />
      <div class="tag">Broward, Florida · Genre FLuid</div>
      <h1 class="glitch flicker" data-text="RXZWELL">RXZWELL</h1>
      <div class="sub">Creat0r 0F ARt</div>
    </header>

    <section class="cards">
      <div class="card">
        <h3>Music · Listen Here</h3>
        <div class="links">
          <a href="https://on.soundcloud.com/fKI5mvsiiI3ReV02WA" target="_blank">SoundCloud <span>↗</span></a>
          <a href="https://youtube.com/@rxzwell" target="_blank">YouTube <span>↗</span></a>
          <a href="https://open.spotify.com/artist/6qmhxNUynVviDvxQRggtFA" target="_blank">Spotify <span>↗</span></a>
          <a href="https://bandlab.com/post/eee5a961-26a3-4086-be4b-ea691554e8c9" target="_blank">BandLab <span>↗</span></a>
          <a href="https://music.apple.com/us/artist/rxzwell/1720338869" target="_blank">Apple Music <span>↗</span></a>
        </div>
      </div>

      <div class="card">
        <h3>Contact · Social</h3>
        <div class="links">
          <a href="https://instagram.com/rxzwell" target="_blank">Instagram <span>↗</span></a>
          <a href="https://www.linkedin.com/in/rxzwell-vii-b935922bb/" target="_blank">LinkedIn <span>↗</span></a>
          <a href="https://pin.it/1pgh7Sbk8" target="_blank">Pinterest <span>↗</span></a>
          <a href="https://www.tiktok.com/@rxzwell007" target="_blank">TikTok <span>↗</span></a>
          <a href="https://twitch.tv/rxzwell" target="_blank">Twitch <span>↗</span></a>
        </div>
      </div>

      <div class="card">
        <h3>Spotify · Preview</h3>
        <div class="embed">
          <!-- Autoplay may be blocked by browsers; kept muted-safe by default -->
          <iframe style="border-radius:12px" src="https://open.spotify.com/embed/artist/6qmhxNUynVviDvxQRggtFA?utm_source=generator&theme=0" width="100%" height="152" frameBorder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
        </div>
      </div>
    </section>

    <section class="card">
      <h3>Album Merch</h3>
      <div class="merch">
        <img src="/mnt/data/IMG_6522.jpeg" alt="Rxzwell merch package" style="width:100%;border-radius:14px;border:1px solid rgba(255,255,255,.15);box-shadow:0 10px 30px rgba(0,0,0,.5)" />
        <img src="/mnt/data/IMG_6523.jpeg" alt="Rxzwell merch USB" style="width:100%;border-radius:14px;border:1px solid rgba(255,255,255,.15);box-shadow:0 10px 30px rgba(0,0,0,.5)" />
      </div>
        <div class="ph">Image 2</div>
        <div class="ph">Image 3</div>
        <div class="ph">Image 4</div>
      </div>
    </section>

    <footer>
      <h2 class="flicker">TOUR COMING SOON</h2>
      <small>© Rxzwell</small>
    </footer>
  </div>

  <!-- Interactions -->
  <script>
    const c = document.getElementById('cursor');
    window.addEventListener('mousemove', e => {
      c.style.left = e.clientX + 'px';
      c.style.top  = e.clientY + 'px';
    });
  </script>
</body>
</html>


