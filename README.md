<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Noxora - Empowering Innovation</title>
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
font-family: 'Segoe UI', sans-serif;
background: #0f0f0f;
color: white;
}

/* === LOADER SCREEN === */
#loader {
position: fixed;
top: 0; left: 0;
width: 100vw;
height: 100vh;
background: black;
z-index: 1000;
overflow: hidden;
display: flex;
justify-content: flex-start;
align-items: center;
}

#loader img {
width: 220px;
height: auto;
animation: flyLeftToRight 4s ease-in-out forwards;
filter: drop-shadow(0 0 40px #00f2ff);
}

@keyframes flyLeftToRight {
0% {
transform: translateX(-300%);
opacity: 0.2;
}
25% {
opacity: 1;
}
50% {
transform: translateX(10%);
opacity: 1;
}
100% {
transform: translateX(200%);
opacity: 0;
}
}

@keyframes hideLoader {
to {
opacity: 0;
visibility: hidden;
}
}

#loader.fade-out {
animation: hideLoader 1s ease forwards;
}

/* === MAIN CONTENT === */
#main {
display: none;
animation: fadeIn 1s ease forwards;
animation-delay: 4.1s;
}

@keyframes fadeIn {
from { opacity: 0; }
to { opacity: 1; }
}

header {
background: #111;
padding: 30px;
text-align: center;
box-shadow: 0 0 15px #000;
}

header img {
height: 160px;
filter: drop-shadow(0 0 20px #00f2ff);
}

nav {
margin-top: 20px;
display: flex;
justify-content: center;
gap: 40px;
}

nav a {
color: white;
font-size: 18px;
text-decoration: none;
transition: 0.3s;
}

nav a:hover {
color: #00f2ff;
}

.hero {
padding: 100px 30px;
text-align: center;
background: linear-gradient(to right, #1c1c1c, #0c0c0c);
}

.hero h1 {
font-size: 3em;
color: #00f2ff;
margin-bottom: 10px;
}

.hero p {
font-size: 1.2em;
color: #ccc;
}

.section {
padding: 60px 30px;
}

.section h2 {
color: #00f2ff;
margin-bottom: 15px;
}

.section p {
line-height: 1.8em;
}

footer {
background: #111;
text-align: center;
padding: 20px;
color: #aaa;
}
</style>
</head>
<body>
<!-- Logo Loader Animation -->
<div id="loader"> <img src="noxora-logo.png" alt="Noxora Logo"> </div>
<!-- Main Website -->
<div id="main"> <header> <img src="noxora-logo.png" alt="Noxora Logo">
<nav> <a href="#home">Home</a> <a href="#about">About</a> <a
href="#services">Services</a> <a href="#contact">Contact</a> </nav> </header>
<section class="hero" id="home"> </section>
<h1>Welcome to Noxora</h1>
<p>Empowering your digital future with technology &amp; design</p>
<section class="section" id="about"> </section>
<h2>About Us</h2>
<p>Noxora is a creative tech company focusing on innovation, futuristic
designs, and powerful digital experiences.</p>
<section class="section" id="services"> </section>
<h2>Our Services</h2>
<p>We provide web development, mobile apps, UI/UX design,
cybersecurity, and software consulting for next-gen businesses.</p>
<section class="section" id="contact"> </section>
<h2>Contact</h2>
<p>Email: hello@noxora.com<br>
Phone: +91-90000-00000</p>
<footer> © 2025 Noxora. All rights reserved. </footer> </div>
<script>
// Auto-hide loader after 4s
setTimeout(() => {
document.getElementById("loader").classList.add("fade-out");
document.getElementById("main").style.display = "block";
}, 4000);
</script>
</body>
</html
