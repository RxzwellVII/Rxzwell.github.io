<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Rxzwell-VII • Genre Fluid Creator • Broward, FL</title>
  <style>
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      background:#000;
      color:#0f0;
      font-family: 'Courier New', Courier, monospace;
      overflow-x:hidden;
      cursor: none; /* Hide default cursor */
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
      padding:2rem;
      text-align:center;
    }
    h1 {
      font-size:4rem;
      text-shadow:0 0 10px #0f0, 0 0 20px #0f0, 0 0 40px #0f0;
      margin:1rem 0;
      letter-spacing:0.1em;
      animation:glitch 4s infinite;
    }
    h2 {
      font-size:2.5rem;
      margin:2rem 0 1rem;
      text-shadow:0 0 15px #0f0;
    }
    .cursor {
      position:fixed;
      width:40px;
      height:40px;
      pointer-events:none;
      transform:translate(-50%, -50%);
      z-index:9999;
      background:url('https://thumbs.dreamstime.com/b/cat-digital-background-digitally-generated-image-neon-green-glow-set-against-backdrop-binary-code-reminiscent-matrix-428414002.jpg') center/cover no-repeat;
      border-radius:50%;
      box-shadow:0 0 20px #0f0, 0 0 40px #0f0, inset 0 0 10px #0f0;
      mix-blend-mode:screen;
      animation:pulse 2s infinite alternate, glitch-cursor 3s infinite;
    }
    @keyframes pulse {
      from { box-shadow:0 0 10px #0f0, 0 0 20px #0f0; }
      to   { box-shadow:0 0 30px #0f0, 0 0 60px #0f0; }
    }
    @keyframes glitch {
      0%,100% { transform:translate(0); }
      20% { transform:translate(-2px, 2px); }
      40% { transform:translate(2px, -2px); }
      60% { transform:translate(-2px, -2px); }
      80% { transform:translate(2px, 2px); }
    }
    @keyframes glitch-cursor {
      0%,100% { filter:brightness(1); }
      10% { filter:brightness(1.5) hue-rotate(90deg); }
      30% { filter:brightness(0.8) hue-rotate(-60deg); }
    }
    .links {
      display:flex;
      flex-wrap:wrap;
      justify-content:center;
      gap:1.5rem;
      margin:2rem 0;
    }
    a {
      color:#0f0;
      text-decoration:none;
      font-size:1.3rem;
      padding:0.8rem 1.5rem;
      border:1px solid #0f0;
      border-radius:8px;
      transition:all 0.3s;
      text-shadow:0 0 5px #0f0;
    }
    a:hover {
      background:#0f03;
      box-shadow:0 0 20px #0f0;
      transform:scale(1.05);
    }
    .spotify-embed {
      margin:3rem auto;
      max-width:500px;
    }
    .merch-tease {
      margin:3rem 0;
      font-size:1.5rem;
    }
    footer {
      margin-top:4rem;
      padding:2rem;
      font-size:1.1rem;
      opacity:0.8;
    }
  </style>
</head>
<body>

  <canvas id="matrix"></canvas>

  <div class="cursor"></div>

  <div class="content">
    <h1>Rxzwell-VII</h1>
    <p style="font-size:1.8rem; margin:1rem 0;">Broward, Florida • Genre Fluid Creator of ARt</p>
    <p style="font-size:1.4rem; max-width:800px; margin:0 auto 2rem;">Underground producer • Musician • Visual alchemist • Breaking the simulation one beat at a time</p>

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
      <a href="https://pin.it/1pgh7Sbk8" target="_blank">Pinterest</a>
      <a href="https://www.tiktok.com/@rxzwell007" target="_blank">TikTok</a>
      <a href="https://twitch.tv/rxzwell" target="_blank">Twitch</a>
    </div>

    <h2>Stream & Vibe</h2>
    <div class="spotify-embed">
      <iframe style="border-radius:12px" src="https://open.spotify.com/embed/artist/6qmhxNUynVviDvxQRggtFA?utm_source=generator" width="100%" height="380" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"></iframe>
    </div>

    <h2>TOUR COMING SOON</h2>
    <p class="merch-tease">Album merch dropping with the simulation reset • Stay plugged in 🔥</p>

    <footer>
      Wake up, Rxzwell... The Matrix has you. • © 2026 Genre Fluid ARt
    </footer>
  </div>

  <script>
    // Matrix digital rain
    const canvas = document.getElementById('matrix');
    const ctx = canvas.getContext('2d');

    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    const chars = '01アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲンabcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*()_+-=[]{}|;:,.<>?/'.split('');
    const fontSize = 14;
    const columns = canvas.width / fontSize;
    const drops = Array(Math.floor(columns)).fill(1);

    function draw() {
      ctx.fillStyle = 'rgba(0, 0, 0, 0.05)';
      ctx.fillRect(0, 0, canvas.width, canvas.height);

      ctx.fillStyle = '#0f0';
      ctx.font = fontSize + 'px monospace';

      drops.forEach((y, i) => {
        const text = chars[Math.floor(Math.random() * chars.length)];
        const x = i * fontSize;

        ctx.fillText(text, x, y * fontSize);

        if (y * fontSize > canvas.height && Math.random() > 0.975) {
          drops[i] = 0;
        }
        drops[i]++;
      });
    }

    setInterval(draw, 35);

    window.addEventListener('resize', () => {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    });

    // Custom cursor follow
    const cursor = document.querySelector('.cursor');
    document.addEventListener('mousemove', e => {
      cursor.style.left = e.clientX + 'px';
      cursor.style.top = e.clientY + 'px';
    });
  </script>
</body>
</html> 
