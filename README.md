<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SuaRra Negus — Digital Power</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
<style>
* {box-sizing:border-box;margin:0;padding:0;font-family:'Poppins',sans-serif;scroll-behavior:smooth;}
body{background:#0D1117;color:#F5F5F5;line-height:1.6;}
header{position:relative;text-align:center;padding:40px 20px;background:linear-gradient(135deg,#0B0F1A,#1E293B);box-shadow:0 4px 15px rgba(0,0,0,0.5);}
header h1{font-size:32px;color:#FFD700;margin-bottom:5px;display:inline-block;vertical-align:middle;}
header p{opacity:0.9;}
header .logo{width:60px;height:60px;vertical-align:middle;margin-right:15px;transition:0.3s;}
header .logo:hover{transform:scale(1.2) rotate(10deg);}

/* NAV */
nav{background:#0B0F1A;position:sticky;top:0;z-index:10;}
nav ul{list-style:none;display:flex;justify-content:center;flex-wrap:wrap;}
nav ul li{margin:10px 15px;}
nav ul li a{text-decoration:none;color:#F5F5F5;font-weight:600;transition:0.3s;}
nav ul li a:hover{color:#FFAA00;transform:scale(1.05);}

/* MAIN */
main{max-width:900px;margin:auto;padding:20px;}
section{background:#111827;padding:25px;margin-bottom:25px;border-radius:12px;box-shadow:0 10px 25px rgba(0,0,0,0.4);transition:0.5s;opacity:0; transform:translateY(30px);}
section.visible{opacity:1; transform:translateY(0);}
h2{color:#FFD700;margin-bottom:15px;}
ul li{margin:8px 0;}

/* BUTTONS */
.btn,.btn-pay{display:block;padding:15px;margin-top:15px;border-radius:10px;font-weight:600;text-align:center;text-decoration:none;transition:0.3s;}
.btn{background:#FFAA00;color:#0D1117;}
.btn:hover{background:#FFD633;transform:scale(1.05);}
.btn-pay{background:#16a34a;color:white;}
.btn-pay:hover{background:#22c55e;transform:scale(1.05);}

/* FORM */
form input,form textarea{width:100%;padding:12px;margin-top:10px;border-radius:8px;border:none;}
form button{width:100%;padding:14px;margin-top:15px;background:#FFAA00;color:#0D1117;border:none;border-radius:8px;font-weight:600;transition:0.3s;}
form button:hover{background:#FFD633;transform:scale(1.05);}

/* FOOTER */
footer{text-align:center;padding:20px;background:#0B0F1A;font-size:14px;}

/* SOCIAL LINKS */
.social{display:flex;justify-content:center;margin-top:10px;}
.social a{margin:0 10px;color:#F5F5F5;font-size:24px;transition:0.3s;}
.social a:hover{color:#FFAA00;transform:scale(1.2);}

/* STATISTICS */
.stats{display:flex;justify-content:space-around;margin-top:15px;}
.stat{background:#1F2937;padding:15px 25px;border-radius:10px;box-shadow:0 5px 15px rgba(0,0,0,0.3);transition:0.3s;}
.stat:hover{transform:scale(1.05);}
.stat h3{color:#FFAA00;margin-bottom:5px;font-size:20px;}
.stat p{font-size:16px;}

/* MEDIA */
@media(max-width:600px){
    header h1{font-size:24px;}
    header .logo{width:50px;height:50px;}
    .stats{flex-direction:column;align-items:center;}
    .stat{margin-bottom:15px;width:80%;}
}
</style>
</head>
<body>

<header>
<img src="https://i.ibb.co/yXH4qP1/logo-suarra.png" alt="Logo SuaRra Negus" class="logo">
<h1>SuaRra Negus</h1>
<p>Digital Power • Royal Vision</p>
</header>

<nav>
<ul>
<li><a href="#accueil">Accueil</a></li>
<li><a href="#services">Services</a></li>
<li><a href="#boutique">Boutique</a></li>
<li><a href="#contact">Contact</a></li>
</ul>
</nav>

<main>
<section id="accueil" class="animate">
<h2>Bienvenue</h2>
<p>Bienvenue sur le site officiel de SuaRra Negus. Découvrez nos services digitaux modernes et rentables.</p>
</section>

<section id="services" class="animate">
<h2>Nos Services</h2>
<ul>
<li>Création de sites web professionnels</li>
<li>Design moderne et responsive</li>
<li>Intégration WhatsApp</li>
<li>Paiement Mobile Money</li>
</ul>
</section>

<section id="boutique" class="animate">
<h2>Offres & Paiement</h2>
<p><strong>Site Business</strong> - 75 000 FCFA</p>
<a class="btn" href="https://wa.me/22607690322?text=Bonjour%20je%20veux%20commander%20un%20site%20business" target="_blank">💬 Commander via WhatsApp</a>
<a class="btn btn-pay" href="https://wa.me/22607690322?text=Bonjour%20je%20veux%20payer%20par%20Mobile%20Money" target="_blank">💳 Payer par Mobile Money</a>

<div class="stats">
<div class="stat"><h3 id="visites">0</h3><p>Visites</p></div>
<div class="stat"><h3 id="commandes">0</h3><p>Commandes</p></div>
</div>
</section>

<section id="contact" class="animate">
<h2>Contact</h2>
<form onsubmit="envoyerMessage(); return false;">
<input type="text" placeholder="Votre nom" required>
<input type="email" placeholder="Votre email" required>
<textarea rows="5" placeholder="Votre message" required></textarea>
<button type="submit">Envoyer</button>
</form>

<div class="social">
<a href="https://wa.me/22607690322" target="_blank">📱</a>
<a href="https://www.facebook.com/" target="_blank">📘</a>
<a href="https://www.tiktok.com/" target="_blank">🎵</a>
<a href="https://www.instagram.com/" target="_blank">📸</a>
</div>
</section>
</main>

<footer>
© 2026 SuaRra Negus
</footer>

<script>
// Animation au scroll
const sections = document.querySelectorAll('.animate');
const observer = new IntersectionObserver(entries => {
entries.forEach(entry => {
    if(entry.isIntersecting){
        entry.target.classList.add('visible');
    }
});
},{threshold:0.2});
sections.forEach(sec => observer.observe(sec));

// Statistiques dynamiques
let visites = 0;
let commandes = 0;
function updateStats() {
    visites += Math.floor(Math.random()*3);
    commandes += Math.floor(Math.random()*1);
    document.getElementById('visites').innerText = visites;
    document.getElementById('commandes').innerText = commandes;
}
setInterval(updateStats,3000);

// Formulaire
function envoyerMessage() {
    alert("Merci ! Votre message a été envoyé 🚀");
}
</script>

</body>
</html>
