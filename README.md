<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Rxzwell-VII • Genre Fluid • Broward, FL • Matrix Reloaded</title>
  <style>
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      background:#000;
      color:#0f0;
      font-family: 'Courier New', Courier, monospace;
      overflow-x:hidden;
      cursor: none;
    }
    canvas {
      position:fixed;
      top:0; left:0;
      z-index:1;
    }
    .content {
      position:relative;
      z-index:10;
      min-height:100vh;
      padding:2rem 1rem;
      text-align:center;
    }
    h1 {
      font-size:5rem;
      text-shadow:0 0 20px #0f0, 0 0 40px #0f0, 0 0 80px #0f0;
      margin:1rem 0;
      letter-spacing:0.15em;
      animation:glitch 5s infinite;
    }
    .main-hero {
      max-width:90%;
      max-height:60vh;
      margin:2rem auto;
      display:block;
      border:3px solid #0f0;
      border-radius:16px;
      box-shadow:0 0 40px #0f0, 0 0 80px #0f0, inset 0 0 20px #0f0;
      animation: pulse 4s infinite alternate, glitch 6s infinite;
      filter: brightness(1.15) contrast(1.3) drop-shadow(0 0 15px #0f0);
    }
    p.tagline {
      font-size:2rem;
      margin:1.5rem 0;
    }
    p.bio {
      font-size:1.5rem;
      max-width:900px;
      margin:0 auto 3rem;
      line-height:1.5;
    }
    .links {
      display:flex;
      flex-wrap:wrap;
      justify-content:center;
      gap:1.2rem;
      margin:2.5rem 0;
    }
    a {
      color:#0f0;
      text-decoration:none;
      font-size:1.4rem;
      padding:1rem 1.8rem;
      border:2px solid #0f0;
      border-radius:10px;
      transition:all 0.4s ease;
      text-shadow:0 0 8px #0f0;
    }
    a:hover {
      background:rgba(0,255,0,0.15);
      box-shadow:0 0 30px #0f0;
      transform:scale(1.08);
    }
    h2 {
      font-size:3rem;
      margin:3rem 0 1.5rem;
      text-shadow:0 0 25px #0f0;
    }
    .spotify {
      margin:3rem auto;
      max-width:600px;
    }
    .tour {
      font-size:2.2rem;
      margin:4rem 0 2rem;
      animation: pulse 3s infinite alternate;
    }
    .cursor {
      position:fixed;
      width:50px;
      height:50px;
      pointer-events:none;
      transform:translate(-50%, -50%);
      z-index:9999;
      background:url('https://thumbs.dreamstime.com/b/cat-digital-background-digitally-generated-image-neon-green-glow-set-against-backdrop-binary-code-reminiscent-matrix-428414002.jpg') center/cover;
      border-radius:50%;
      box-shadow:0 0 25px #0f0, 0 0 50px #0f0, inset 0 0 15px #0f0;
      mix-blend-mode:screen;
      animation:pulse 2.5s infinite alternate, glitch-cursor 4s infinite;
    }
    @keyframes pulse {
      from { transform:translate(-50%, -50%) scale(1); box-shadow:0 0 15px #0f0, 0 0 30px #0f0; }
      to   { transform:translate(-50%, -50%) scale(1.15); box-shadow:0 0 40px #0f0, 0 0 80px #0f0; }
    }
    @keyframes glitch {
      0%,100% { transform:translate(0); }
      20% { transform:translate(-3px, 3px); }
      40% { transform:translate(3px, -3px); }
      60% { transform:translate(-3px, -3px); }
      80% { transform:translate(3px, 3px); }
    }
    @keyframes glitch-cursor {
      0%,100% { filter:brightness(1) hue-rotate(0deg); }
      15% { filter:brightness(1.6) hue-rotate(120deg); }
      35% { filter:brightness(0.7) hue-rotate(-90deg); }
    }
    footer {
      margin-top:5rem;
      padding:2rem;
      font-size:1.3rem;
      opacity:0.7;
    }
  </style>
</head>
<body>

  <canvas id="matrix"></canvas>
  <div class="cursor"></div>

  <div class="content">
    <h1>Rxzwell-VII</h1>

    <!-- MAIN HERO IMAGE: Replace src with your direct Pinterest image URL -->
    <img 
      class="main-hero" 
      src="YOUR_DIRECT_PIN_IMAGE_URL_HERE" 
      alt="Rxzwell-VII Main Art – Neon Glitch Cat Laser Eyes Matrix Vibe"
      loading="eager"
    />

    <p class="tagline">Broward, Florida • Genre Fluid Creator of ARt</p>
    <p class="bio">Underground producer • Visual alchemist • Musician breaking the code • One glitch at a time in the simulation</p>

    <div class="links">
      <a href="https://on.soundcloud.com/fKI5mvsiiI3ReV02WA" target="_blank">SoundCloud</a>
      <a href="https://youtube.com/@rxzwell" target="_blank">YouTube</a>
      <a href="https://open.spotify.com/artist/6qmhxNUynVviDvxQRggtFA" target="_blank">Spotify</a>
      <a href="https://music.apple.com/us/artist/rxzwell/1720338869" target="_blank">Apple Music</a>
      <a href="https://bandlab.com/post/eee5a961-26a3-4086-be4b-ea691554e8c9" target="_blank">BandLab</a>
    </div>

    <div class="links">
      <a href="https://instagram.com/rxzwell" target="_blank">Instagram</a>
      <a href="https://www.linkedin.com/in/rxzwell-vii-b935922bb/" target="_blank">LinkedIn</a>
      <a href="https://pin.it/1pgh7Sbk8" target="_blank">Pinterest Gallery</a>
      <a href="https://www.tiktok.com/@rxzwell007" target="_blank">TikTok</a>
      <a href="https://twitch.tv/rxzwell" target="_blank">Twitch</a>
    </div>

    <h2>Enter the Stream</h2>
    <div class="spotify">
      <iframe style="border-radius:12px" src="https://open.spotify.com/embed/artist/6qmhxNUynVviDvxQRggtFA?utm_source=generator" width="100%" height="400" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"></iframe>
    </div>

    <div class="tour">TOUR COMING SOON • Simulation Reset Imminent 🔥</div>

    <footer>
      Wake up, Rxzwell-VII... The Matrix has you. • © 2026 Genre Fluid ARt
    </footer>
  </div>

  <script>
    // Matrix digital rain
    const canvas = document.getElementById('matrix');
    const ctx = canvas.getContext('2d');

    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    const chars = '01アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲンabcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*()_+-=[]{}|;:,.<>?/'.split('');
    const fontSize = 16;
    const columns = canvas.width / fontSize;
    const drops = Array(Math.floor(columns)).fill(1);

    function draw() {
      ctx.fillStyle = 'rgba(0, 0, 0, 0.04)';
      ctx.fillRect(0, 0, canvas.width, canvas.height);

      ctx.fillStyle = '#0f0';
      ctx.font = fontSize + 'px monospace';

      drops.forEach((y, i) => {
        const text = chars[Math.floor(Math.random() * chars.length)];
        const x = i * fontSize;
        ctx.fillText(text, x, y * fontSize);

        if (y * fontSize > canvas.height && Math.random() > 0.975) drops[i] = 0;
        drops[i]++;
      });
    }

    setInterval(draw, 40);

    window.addEventListener('resize', () => {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    });

    // Custom laser eyes cat cursor
    const cursor = document.querySelector('.cursor');
    document.addEventListener('mousemove', e => {
      cursor.style.left = e.clientX + 'px';
      cursor.style.top = e.clientY + 'px';
    });
  </script>
</body>
</html>
