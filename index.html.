
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KlarexxSMP — Minecraft Server</title>
<meta name="theme-color" content="#07111f">

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;600;700;800&family=Montserrat:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<style>
:root {
  --bg:#060d18;
  --panel:#0d1b2c;
  --cyan:#39f2df;
  --blue:#397cff;
  --text:#f2f8ff;
  --muted:#91a9c1;
}
*{margin:0;padding:0;box-sizing:border-box;scroll-behavior:smooth}
body{
  background:var(--bg);
  color:var(--text);
  font-family:Montserrat,sans-serif;
  overflow-x:hidden;
}
body:before{
  content:"";
  position:fixed;inset:0;z-index:-2;
  background:
  radial-gradient(circle at 15% 20%,#123c5b66,transparent 35%),
  radial-gradient(circle at 85% 65%,#075b6570,transparent 35%),
  linear-gradient(145deg,#060d18,#0a1728);
}
body:after{
  content:"";position:fixed;inset:0;z-index:-1;
  opacity:.13;pointer-events:none;
  background-image:linear-gradient(#ffffff10 1px,transparent 1px),
  linear-gradient(90deg,#ffffff10 1px,transparent 1px);
  background-size:45px 45px;
}
a{text-decoration:none;color:inherit}
button{font-family:inherit;cursor:pointer}
.container{width:min(1120px,92%);margin:auto}

/* NAV */
nav{
  position:sticky;top:0;z-index:50;
  background:#071321d9;
  backdrop-filter:blur(18px);
  border-bottom:1px solid #39f2df25;
}
.navinner{
  height:76px;display:flex;align-items:center;
  justify-content:space-between;gap:15px;
}
.logo{
  font-family:Orbitron,sans-serif;
  font-weight:800;font-size:20px;
  color:var(--cyan);
  text-shadow:0 0 20px #39f2df80;
}
.navlinks{display:flex;gap:25px;color:#b8c9da;font-size:13px}
.navlinks a:hover{color:var(--cyan)}
.navbtn{
  border:1px solid #39f2df80;
  background:#39f2df12;color:var(--cyan);
  padding:11px 17px;border-radius:10px;
  font-size:12px;font-weight:800;
}

/* HERO */
.hero{
  min-height:610px;display:flex;align-items:center;
  position:relative;padding:90px 0;
}
.hero-content{max-width:730px;animation:appear 1s ease}
.tag{
  display:inline-block;padding:9px 14px;
  border:1px solid #39f2df55;
  border-radius:30px;color:var(--cyan);
  background:#39f2df0d;font-size:11px;
  letter-spacing:2px;font-weight:800;
}
h1{
  font-family:Orbitron,sans-serif;
  font-size:clamp(42px,8vw,82px);
  line-height:1.08;margin:25px 0;
  letter-spacing:-3px;
}
h1 span{
  color:var(--cyan);
  text-shadow:0 0 35px #39f2df70;
}
.hero p{color:var(--muted);font-size:16px;line-height:1.8;max-width:560px}
.actions{display:flex;gap:14px;flex-wrap:wrap;margin-top:30px}
.btn{
  display:inline-flex;justify-content:center;align-items:center;
  padding:15px 23px;border-radius:11px;
  font-weight:800;font-size:13px;
  transition:.3s;
}
.btn-main{
  color:#04131b;background:linear-gradient(110deg,#39f2df,#48baff);
  box-shadow:0 0 25px #39f2df40;
}
.btn-main:hover{transform:translateY(-4px);box-shadow:0 0 35px #39f2df80}
.btn-outline{border:1px solid #39f2df60;color:var(--cyan)}
.btn-outline:hover{background:#39f2df16;transform:translateY(-3px)}
.serverbox{
  margin-top:45px;padding:17px 20px;
  display:flex;align-items:center;justify-content:space-between;
  gap:15px;max-width:480px;
  background:#102238b8;border:1px solid #39f2df35;
  border-radius:14px;
}
.serverbox small{color:var(--muted);display:block;margin-bottom:6px}
.serverbox strong{font-family:Orbitron,sans-serif;font-size:13px}
.copy{
  background:var(--cyan);color:#06151c;border:0;
  border-radius:9px;padding:12px 15px;font-weight:800;
}

/* SECTIONS */
section{padding:85px 0}
.section-title{text-align:center;margin-bottom:45px}
.section-title small{color:var(--cyan);letter-spacing:3px;font-weight:800}
.section-title h2{
  font-family:Orbitron,sans-serif;
  font-size:clamp(26px,5vw,39px);margin-top:13px
}
.section-title p{color:var(--muted);margin-top:12px;font-size:13px}

/* FEATURES */
.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
.feature,.rule,.donate-card{
  background:linear-gradient(145deg,#102238,#0b1727);
  border:1px solid #ffffff12;border-radius:18px;
  padding:25px;transition:.35s;position:relative;overflow:hidden;
}
.feature:before,.donate-card:before{
  content:"";position:absolute;top:0;left:0;width:100%;height:2px;
  background:linear-gradient(90deg,transparent,var(--cyan),transparent);
  opacity:.6;
}
.feature:hover,.rule:hover,.donate-card:hover{
  transform:translateY(-7px);
  border-color:#39f2df70;
  box-shadow:0 15px 40px #0007,0 0 20px #39f2df12;
}
.feature .emoji{font-size:31px;margin-bottom:18px}
.feature h3{font-size:16px;margin-bottom:10px}
.feature p{font-size:12px;line-height:1.7;color:var(--muted)}

/* STORE */
.store{background:#091525a8;border-top:1px solid #39f2df18;border-bottom:1px solid #39f2df18}
.donates{display:grid;grid-template-columns:repeat(4,1fr);gap:15px}
.donate-card{text-align:center;padding:25px 17px}
.donate-card .symbol{font-size:39px;margin-bottom:17px}
.donate-card h3{font-family:Orbitron,sans-serif;font-size:17px}
.donate-card .price{font-size:29px;font-weight:800;margin:17px 0 8px}
.donate-card p{color:var(--muted);font-size:11px;margin-bottom:20px}
.buy{
  display:block;padding:13px 8px;border-radius:9px;
  background:linear-gradient(100deg,#39f2df,#399dff);
  color:#06131d;font-size:11px;font-weight:900;
  transition:.3s;
}
.buy:hover{filter:brightness(1.2);transform:scale(1.04)}
.dizer{--accent:#5bdfff}
.santa{--accent:#ff7777}
.klarexx{--accent:#ffd76a}
.nivazu{--accent:#5fffc6}
.donate-card{border-color:color-mix(in srgb,var(--accent),transparent 65%)}
.donate-card h3,.donate-card .price{color:var(--accent)}
.donate-card:before{background:var(--accent)}

/* RULES */
.rules{display:grid;grid-template-columns:repeat(2,1fr);gap:15px}
.rule{display:flex;gap:15px;align-items:flex-start}
.rule b{color:var(--cyan);font-size:18px}
.rule p{font-size:13px;line-height:1.6;color:var(--muted)}

/* CTA */
.cta{
  text-align:center;padding:55px 25px;
  border:1px solid #39f2df45;border-radius:22px;
  background:radial-gradient(ellipse at top,#12405288,#0c1b2d 70%);
}
.cta h2{font-family:Orbitron,sans-serif;font-size:clamp(24px,5vw,37px)}
.cta p{color:var(--muted);margin:15px 0 25px;font-size:13px}
footer{
  padding:30px 0;border-top:1px solid #ffffff12;
  color:#7890a8;font-size:11px;text-align:center;
}
footer strong{color:var(--cyan)}
@keyframes appear{
  from{opacity:0;transform:translateY(25px)}
  to{opacity:1;transform:translateY(0)}
}
@media(max-width:800px){
  .grid{grid-template-columns:repeat(2,1fr)}
  .donates{grid-template-columns:repeat(2,1fr)}
  .navlinks{display:none}
  .hero{min-height:550px}
}
@media(max-width:480px){
  .grid,.rules{grid-template-columns:1fr}
  .donates{grid-template-columns:repeat(2,minmax(0,1fr));gap:10px}
  .donate-card{padding:20px 10px}
  .donate-card .price{font-size:24px}
  .logo{font-size:16px}
  .navbtn{padding:10px;font-size:10px}
}
</style>
</head>

<body>
<nav>
  <div class="container navinner">
    <a class="logo" href="#">KLAREXX<span>SMP</span></a>
    <div class="navlinks">
      <a href="#home">Главная</a>
      <a href="#features">Возможности</a>
      <a href="#donate">Донаты</a>
      <a href="#rules">Правила</a>
    </div>
    <a class="navbtn" href="https://t.me/klarexxSmp" target="_blank">TELEGRAM ↗</a>
  </div>
</nav>

<main>
<section class="hero" id="home">
  <div class="container">
    <div class="hero-content">
      <span class="tag">✦ MINECRAFT JAVA SERVER</span>
      <h1>ТВОЯ ИСТОРИЯ<br>НА <span>KLAREXX</span></h1>
      <p>Начни свой путь, создавай союзы, развивай экономику и стань легендой KlarexxSMP. Твой мир — твои правила!</p>
      <div class="actions">
        <a class="btn btn-main" href="#connect">НАЧАТЬ ИГРАТЬ</a>
        <a class="btn btn-outline" href="#donate">МАГАЗИН ДОНАТОВ</a>
      </div>
      <div class="serverbox" id="connect">
        <div>
          <small>IP СЕРВЕРА · JAVA</small>
          <strong>klarexxsmp.mcsh.gg</strong>
        </div>
        <button class="copy" onclick="copyIP()">КОПИРОВАТЬ</button>
      </div>
    </div>
  </div>
</section>

<section id="features">
  <div class="container">
    <div class="section-title">
      <small>ВОЗМОЖНОСТИ</small>
      <h2>ПОЧЕМУ KLAREXX?</h2>
      <p>Всё необходимое для интересной игры</p>
    </div>
    <div class="grid">
      <div class="feature"><div class="emoji">🛡️</div><h3>Приваты</h3><p>Защищай свои территории и строй собственную базу.</p></div>
      <div class="feature"><div class="emoji">💰</div><h3>Экономика</h3><p>Торгуй, зарабатывай и развивайся вместе с игроками.</p></div>
      <div class="feature"><div class="emoji">⚔️</div><h3>Кланы</h3><p>Собирай команду и соревнуйся с другими игроками.</p></div>
      <div class="feature"><div class="emoji">🏪</div><h3>Аукцион</h3><p>Выставляй предметы и находи выгодные предложения.</p></div>
      <div class="feature"><div class="emoji">🎁</div><h3>Награды</h3><p>Заходи в игру и получай ежедневные бонусы.</p></div>
      <div class="feature"><div class="emoji">🏆</div><h3>Ивенты</h3><p>Участвуй в событиях и докажи, на что способен.</p></div>
    </div>
  </div>
</section>

<section class="store" id="donate">
  <div class="container">
    <div class="section-title">
      <small>PREMIUM SHOP</small>
      <h2>МАГАЗИН ПРИВИЛЕГИЙ</h2>
      <p>Выбери свой статус на KlarexxSMP</p>
    </div>
    <div class="donates">
      <div class="donate-card dizer">
        <div class="symbol">💎</div>
        <h3>DIZER</h3>
        <div class="price">20 ₽</div>
        <p>Привилегия сервера</p>
        <a class="buy" href="https://t.me/klarexxSmp" target="_blank">КУПИТЬ ↗</a>
      </div>
      <div class="donate-card santa">
        <div class="symbol">🎅</div>
        <h3>SANTA</h3>
        <div class="price">39 ₽</div>
        <p>Привилегия сервера</p>
        <a class="buy" href="https://t.me/klarexxSmp" target="_blank">КУПИТЬ ↗</a>
      </div>
      <div class="donate-card klarexx">
        <div class="symbol">👑</div>
        <h3>KLAREXX</h3>
        <div class="price">54 ₽</div>
        <p>Привилегия сервера</p>
        <a class="buy" href="https://t.me/klarexxSmp" target="_blank">КУПИТЬ ↗</a>
      </div>
      <div class="donate-card nivazu">
        <div class="symbol">⚡</div>
        <h3>NIVAZU</h3>
        <div class="price">69 ₽</div>
        <p>Привилегия сервера</p>
        <a class="buy" href="https://t.me/klarexxSmp" target="_blank">КУПИТЬ ↗</a>
      </div>
    </div>
  </div>
</section>

<section id="rules">
  <div class="container">
    <div class="section-title">
      <small>FAIR PLAY</small>
      <h2>ПРАВИЛА СЕРВЕРА</h2>
      <p>Уважай игроков и поддерживай порядок</p>
    </div>
    <div class="rules">
      <div class="rule"><b>01</b><p>Уважай игроков и администрацию сервера.</p></div>
      <div class="rule"><b>02</b><p>Не используй читы и сторонние программы для преимущества.</p></div>
      <div class="rule"><b>03</b><p>Не спамь и не рекламируй посторонние проекты.</p></div>
      <div class="rule"><b>04</b><p>Соблюдай правила общения в игровом чате.</p></div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="cta">
      <h2>ГОТОВ К ПРИКЛЮЧЕНИЮ?</h2>
      <p>Присоединяйся к сообществу KlarexxSMP!</p>
      <a class="btn btn-main" href="https://t.me/klarexxSmp" target="_blank">НАШ TELEGRAM ↗</a>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="container">
    <strong>KLAREXXSMP</strong> · Minecraft Java Server<br><br>
    IP: klarexxsmp.mcsh.gg · Версия: 1.21.11<br><br>
    © 2026 KlarexxSMP
  </div>
</footer>

<script>
function copyIP(){
  navigator.clipboard.writeText("klarexxsmp.mcsh.gg")
  .then(()=>alert("IP сервера скопирован!"))
  .catch(()=>alert("IP: klarexxsmp.mcsh.gg"));
}
</script>
</body>
</html>
