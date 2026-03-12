<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>DG CONSULTORIA | Especialista em MikroTik, OLT e Infraestrutura</title>

<meta name="description" content="Consultoria especializada em MikroTik, OLT, Servidores, BGP, IPv6, Firewall e Infraestrutura para provedores de internet.">
<meta name="keywords" content="MikroTik, OLT, Consultoria ISP, BGP, IPv6, Firewall, Provedor de Internet">
<meta name="author" content="DG CONSULTORIA">

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;900&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box}
body{
font-family:'Poppins',sans-serif;
background:#000;
color:#fff;
overflow-x:hidden;
}

/* FUNDO TECNOLÓGICO */
body::before{
content:"";
position:fixed;
width:100%;
height:100%;
background:url('https://images.unsplash.com/photo-1558494949-ef010cbdcc31') center/cover no-repeat;
opacity:0.07;
z-index:-1;
}

/* HEADER */
header{
display:flex;
justify-content:space-between;
align-items:center;
padding:20px 8%;
position:fixed;
width:100%;
background:rgba(0,0,0,0.9);
border-bottom:1px solid #00ff88;
z-index:1000;
}

.logo{
font-family:'Orbitron',sans-serif;
font-size:24px;
color:#00ff88;
text-shadow:0 0 15px #00ff88;
}

nav a{
margin-left:25px;
text-decoration:none;
color:#fff;
cursor:pointer;
transition:.3s;
font-weight:500;
}

nav a:hover{color:#00ff88}

/* SEÇÕES */
section{
min-height:100vh;
padding:140px 8%;
display:none;
animation:fade .6s ease;
}

.active{display:block}

@keyframes fade{
from{opacity:0;transform:translateY(20px)}
to{opacity:1;transform:translateY(0)}
}

h1{
font-family:'Orbitron',sans-serif;
font-size:42px;
color:#00ff88;
margin-bottom:20px;
text-shadow:0 0 15px #00ff88;
}

h2{color:#00ff88;margin:20px 0}

p{color:#ccc;margin-bottom:20px;line-height:1.6}

.btn{
background:#00ff88;
padding:14px 35px;
color:#000;
font-weight:bold;
text-decoration:none;
border-radius:6px;
cursor:pointer;
transition:.3s;
display:inline-block;
}

.btn:hover{
background:#00cc66;
box-shadow:0 0 20px #00ff88;
}

/* CARDS */
.cards{
display:flex;
flex-wrap:wrap;
gap:30px;
justify-content:center;
}

.card{
background:rgba(20,20,20,.9);
padding:30px;
width:300px;
border-radius:10px;
border:1px solid #00ff8830;
transition:.4s;
text-align:center;
}

.card:hover{
transform:translateY(-10px);
box-shadow:0 0 25px #00ff88;
}

/* FORM */
form{max-width:500px;margin:auto}

input,select,textarea{
width:100%;
padding:12px;
margin-bottom:15px;
background:#111;
border:1px solid #00ff88;
color:#fff;
border-radius:5px;
}

button{
width:100%;
padding:14px;
background:#00ff88;
border:none;
font-weight:bold;
cursor:pointer;
border-radius:5px;
}

/* AREA CLIENTE */
.login-box{
max-width:400px;
margin:auto;
background:#111;
padding:30px;
border-radius:10px;
border:1px solid #00ff88;
}

/* WHATSAPP */
.whatsapp{
position:fixed;
bottom:25px;
right:25px;
background:#00ff88;
color:#000;
padding:18px;
border-radius:50%;
font-weight:bold;
box-shadow:0 0 20px #00ff88;
text-decoration:none;
animation:pulse 1.5s infinite;
}

@keyframes pulse{
0%{box-shadow:0 0 10px #00ff88}
50%{box-shadow:0 0 25px #00ff88}
100%{box-shadow:0 0 10px #00ff88}
}

footer{
text-align:center;
padding:20px;
border-top:1px solid #00ff88;
}
</style>
</head>

<body>

<header>
<div class="logo">DG CONSULTORIA</div>
<nav>
<a onclick="showPage('home')">Home</a>
<a onclick="showPage('sobre')">Sobre</a>
<a onclick="showPage('servicos')">Serviços</a>
<a onclick="showPage('cliente')">Área Cliente</a>
<a onclick="showPage('contato')">Contato</a>
</nav>
</header>

<!-- HOME -->
<section id="home" class="active">
<h1>Especialistas em Infraestrutura para ISPs</h1>
<p>MikroTik, OLT, BGP, IPv6, Firewall e soluções completas para provedores.</p>
<a class="btn" onclick="showPage('contato')">Solicitar Consultoria</a>
</section>

<!-- SOBRE -->
<section id="sobre">
<h1>Sobre a DG CONSULTORIA</h1>
<p>Somos especialistas em redes de alta performance, infraestrutura para provedores de internet e segurança avançada.</p>
<p>Atuamos com foco em estabilidade, escalabilidade e performance.</p>
</section>

<!-- SERVIÇOS -->
<section id="servicos">
<h1>Nossos Serviços</h1>
<div class="cards">

<div class="card">
<h2>MikroTik</h2>
<p>BGP, IPv6, Load Balance, Failover, Firewall.</p>
</div>

<div class="card">
<h2>OLT & Fibra</h2>
<p>Provisionamento ONU, VLAN, Integração PPPoE.</p>
</div>

<div class="card">
<h2>Servidores</h2>
<p>Linux, Windows, Virtualização e Cloud.</p>
</div>

</div>
</section>

<!-- AREA CLIENTE -->
<section id="cliente">
<h1>Área do Cliente</h1>
<div class="login-box">
<input type="text" placeholder="Usuário">
<input type="password" placeholder="Senha">
<button>Acessar</button>
</div>
</section>

<!-- CONTATO -->
<section id="contato">
<h1>Entre em Contato</h1>
<form id="whatsappForm">
<input type="text" id="nome" placeholder="Seu nome" required>
<select id="solucao" required>
<option value="">Qual solução deseja?</option>
<option>MikroTik</option>
<option>OLT</option>
<option>Servidor</option>
<option>Consultoria Completa</option>
</select>
<textarea id="mensagem" placeholder="Descreva seu projeto" required></textarea>
<button type="submit">Enviar pelo WhatsApp</button>
</form>
</section>

<footer>
© 2026 DG CONSULTORIA - Todos os direitos reservados
</footer>

<a href="https://api.whatsapp.com/send?phone=5521976487485" target="_blank" class="whatsapp">W</a>

<script>
function showPage(page){
document.querySelectorAll("section").forEach(sec=>sec.classList.remove("active"));
document.getElementById(page).classList.add("active");
}

document.getElementById('whatsappForm').addEventListener('submit',function(e){
e.preventDefault();
var nome=document.getElementById('nome').value;
var solucao=document.getElementById('solucao').value;
var mensagem=document.getElementById('mensagem').value;

var texto=`Olá, meu nome é ${nome}.
Solução: ${solucao}.
Detalhes: ${mensagem}`;

var numero='5521976487485';
var url=`https://api.whatsapp.com/send?phone=${numero}&text=${encodeURIComponent(texto)}`;
window.open(url,'_blank');
});
</script>

</body>
</html># dgmtconsultoria
