<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rxzwell — Official</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;800&family=Inter:wght@300;500&display=swap" rel="stylesheet">

<style>
:root{
--bg:#050505;
--neon1:#00f0ff;
--neon2:#00ff9c;
--text:#e5e5e5;
--gray:#1a1a1a;
--border:#2a2a2a;
}

*{margin:0;padding:0;box-sizing:border-box}
body{
background:var(--bg);
color:var(--text);
font-family:'Inter',sans-serif;
overflow-x:hidden;
}

/* Y2K grid background */
body::before{
content:"";
position:fixed;
top:0;left:0;
width:100%;height:100%;
background:
linear-gradient(to right, #111 1px, transparent 1px),
linear-gradient(to bottom, #111 1px, transparent 1px);
background-size:40px 40px;
opacity:.25;
z-index:-1;
}

/* Header */
header{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
border-bottom:1px solid var(--border);
}

h1{
font-family:'Orbitron',sans-serif;
font-size:4rem;
letter-spacing:4px;
background:linear-gradient(90deg,var(--neon1),var(--neon2));
-webkit-background-clip:text;
color:transparent;
text-shadow:0 0 15px var(--neon1);
animation:flicker 3s infinite alternate;
}

@keyframes flicker{
0%{opacity:1}
48%{opacity:.85}
50%{opacity:.4}
52%{opacity:.9}
100%{opacity:1}
}

.tag{
margin-top:15px;
color:#777;
font-size:14px;
letter-spacing:2px;
}

.btn{
margin-top:40px;
padding:12px 30px;
border:1px solid var(--neon1);
color:var(--neon1);
text-decoration:none;
font-family:'Orbitron';
transition:.3s;
}

.btn:hover{
background:var(--neon1);
color:black;
box-shadow:0 0 20px var(--neon1);
}

/* Sections */
section{
padding:80px 10%;
border-bottom:1px solid var(--border);
}

h2{
font-family:'Orbitron';
margin-bottom:30px;
color:var(--neon2);
letter-spacing:3px;
}

.card{
background:var(--gray);
padding:30px;
border:1px solid var(--border);
box-shadow:0 0 15px rgba(0,255,200,.05);
}

/* Social links */
.socials a{
display:inline-block;
margin:10px 20px 0 0;
color:var(--neon1);
text-decoration:none;
font-weight:500;
transition:.3s;
}

.socials a:hover{
color:var(--neon2);
text-shadow:0 0 10px var(--neon2);
}

/* Email */
input[type=email]{
padding:12px;
background:black;
border:1px solid var(--border);
color:white;
width:250px;
}

button{
padding:12px 25px;
border:none;
background:var(--neon2);
color:black;
font-weight:bold;
cursor:pointer;
}

button:hover{
box-shadow:0 0 15px var(--neon2);
}

/* Footer */
footer{
text-align:center;
padding:30px;
font-size:12px;
color:#666;
}
</style>
</head>

<body>

<header>
<h1>RXZWELL</h1>
<div class="tag">DIGITAL CHAOS • NEON FUTURE • 2000s CORE</div>
<a href="#music" class="btn">ENTER</a>
</header>

<section id="music">
<h2>LATEST DROP</h2>
<div class="card">
<iframe style="width:100%;height:315px;border:none;"
src="https://open.spotify.com/embed/track/YOURTRACKID">
</iframe>
</div>
</section>

<section>
<h2>CONNECT</h2>
<div class="socials">
<a href="#">Instagram</a>
<a href="#">YouTube</a>
<a href="#">TikTok</a>
<a href="#">X</a>
</div>
</section>

<section>
<h2>JOIN THE LIST</h2>
<div class="card">
<form action="YOURMAILCHIMPLINK" method="post" target="_blank">
<input type="email" name="EMAIL" placeholder="Enter email" required>
<button type="submit">SUBSCRIBE</button>
</form>
</div>
</section>

<section>
<h2>ABOUT</h2>
<div class="card">
<p>
Rxzwell is a dark neon digital entity blending early internet aesthetics
with futuristic sound design.
</p>
</div>
</section>

<footer>
© 2026 RXZWELL — ALL RIGHTS RESERVED
</footer>

</body>
</html>
