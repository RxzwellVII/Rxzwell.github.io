<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rxzwell | Official</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Rajdhani:wght@400;600&display=swap" rel="stylesheet">

<style>
* {margin:0;padding:0;box-sizing:border-box;}

body{
background:#050507;
color:white;
font-family:'Rajdhani',sans-serif;
overflow-x:hidden;
cursor: crosshair;
}

/* Optional custom cursor */
/* body { cursor: url('cursor.png'), auto; } */

.neon-green{
color:#00ff99;
text-shadow:0 0 8px #00ff99,0 0 25px #00ff99;
}

.neon-pink{
color:#ff00cc;
text-shadow:0 0 8px #ff00cc,0 0 25px #ff00cc;
}

/* HERO */
.hero{
height:100vh;
background:
linear-gradient(rgba(0,0,0,.75),rgba(0,0,0,.85)),
url('rxzwell-hero.jpg') center/cover no-repeat;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
position:relative;
}

.hero h1{
font-family:'Orbitron',sans-serif;
font-size:5rem;
letter-spacing:10px;
animation:glitch 1.5s infinite;
}

@keyframes glitch{
0%{text-shadow:2px 2px #ff00cc,-2px -2px #00ff99;}
50%{text-shadow:-2px -2px #ff00cc,2px 2px #00ff99;}
100%{text-shadow:2px -2px #ff00cc,-2px 2px #00ff99;}
}

.pulse7{
font-size:3rem;
margin-top:15px;
animation:pulse 2s infinite;
}

@keyframes pulse{
0%{opacity:1;text-shadow:0 0 10px #00ff99;}
50%{opacity:.5;text-shadow:0 0 40px #00ff99;}
100%{opacity:1;text-shadow:0 0 10px #00ff99;}
}

/* Scroll distortion */
.section{
padding:100px 20px;
max-width:1100px;
margin:auto;
text-align:center;
transition:all .6s ease;
}

.section:hover{
transform:scale(1.02);
filter:contrast(120%);
}

.section h2{
font-family:'Orbitron';
font-size:2.5rem;
margin-bottom:30px;
}

/* Buttons */
.links a{
display:inline-block;
margin:10px;
padding:14px 30px;
border:2px solid #00ff99;
color:#00ff99;
text-decoration:none;
font-weight:600;
transition:.3s;
}

.links a:hover{
background:#00ff99;
color:black;
box-shadow:0 0 20px #00ff99;
transform:scale(1.05);
}

/* Tour cards */
.tour{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:20px;
}

.tour div{
border:1px solid #222;
padding:20px;
width:250px;
background:#0f0f14;
}

/* Merch */
.merch img{
width:200px;
border:1px solid #222;
margin:15px;
transition:.3s;
}

.merch img:hover{
transform:scale(1.1);
box-shadow:0 0 20px #ff00cc;
}

/* Email form */
input[type=email]{
padding:12px;
width:250px;
background:#111;
border:1px solid #00ff99;
color:white;
}

button{
padding:12px 20px;
background:#00ff99;
border:none;
cursor:pointer;
font-weight:bold;
}

/* Scanlines */
body::after{
content:"";
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:repeating-linear-gradient(
to bottom,
rgba(255,255,255,0.02),
rgba(255,255,255,0.02) 1px,
transparent 1px,
transparent 3px);
pointer-events:none;
}

footer{
padding:40px;
opacity:.6;
border-top:1px solid #222;
text-align:center;
}

</style>
</head>
<body>

<!-- Optional Intro Audio -->
<audio autoplay loop muted>
<source src="intro.mp3" type="audio/mpeg">
</audio>

<section class="section">
  <h2 class="neon-pink">STREAM</h2>
  <div class="links">
    <a href="https://open.spotify.com/artist/6qmhxNUynVviDvxQRggtFA" target="_blank">Spotify</a>
    <a href="https://music.apple.com/us/artist/rxzwell/1720338869" target="_blank">Apple Music</a>
    <a href="https://on.soundcloud.com/fKI5mvsiiI3ReV02WA" target="_blank">SoundCloud</a>
    <a href="https://bandlab.com/post/eee5a961-26a3-4086-be4b-ea691554e8c9" target="_blank">BandLab</a>
  </div>

  <br><br>

  <iframe style="border-radius:12px"
    src="https://open.spotify.com/embed/artist/6qmhxNUynVviDvxQRggtFA"
    width="100%" height="352" frameborder="0"
    allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture">
  </iframe>
</section>

<section class="section">
  <h2 class="neon-green">CONNECT</h2>
  <div class="links">
    <a href="https://youtube.com/@rxzwell" target="_blank">YouTube</a>
    <a href="https://instagram.com/rxzwell" target="_blank">Instagram</a>
    <a href="https://twitch.tv/rxzwell" target="_blank">Twitch</a>
    <a href="https://www.linkedin.com/in/rxzwell-vii-b935922bb/" target="_blank">LinkedIn</a>
    <a href="https://pin.it/1pgh7Sbk8" target="_blank">Pinterest</a>
  </div>
</section></div>

<br><br>

<iframe style="border-radius:12px"
src="https://open.spotify.com/embed/artist/6qmhxNUynVviDvxQRggtFA"
width="100%" height="352" frameBorder="0"
allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture">
</iframe>
</section>

<section class="section">
<h2 class="neon-pink">TOUR</h2>
<div class="tour">
<div>
<h3>Miami, FL</h3>
<p>March 12, 2026</p>
</div>
<div>
<h3>Orlando, FL</h3>
<p>April 2, 2026</p>
</div>
<div>
<h3>Tampa, FL</h3>
<p>April 18, 2026</p>
</div>
</div>
</section>

<section class="section">
<h2 class="neon-green">MERCH</h2>
<div class="merch">
<img src="https://via.placeholder.com/200x250" alt="Merch1">
<img src="https://via.placeholder.com/200x250" alt="Merch2">
</div>
</section>

<section class="section">
<h2 class="neon-pink">JOIN THE UNDERGROUND</h2>
<form>
<input type="email" placeholder="Enter your email">
<button>SUBMIT</button>
</form>
</section>

<section class="section">
<h2 class="neon-green">EPK</h2>
<p>
Rxzwell is a Broward, Florida-based genre-fluid punk artist blending distortion,
emotion, and futuristic rebellion. Available for booking, collaborations, and press.
</p>
<br>
<a class="links" href="mailto:yourbookingemail@email.com">BOOKING INQUIRIES</a>
</section>

<footer>
© 2026 Rxzwell — All Rights Reserved
</footer>

</body>
</html>
