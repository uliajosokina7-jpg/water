<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ключ живой воды — доставка воды в Уральске</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=PT+Serif:wght@400;700&family=PT+Sans:wght@400;700&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#0B1F24;
    --deep:#123B44;
    --deep2:#0E2F37;
    --aqua:#2FB6D9;
    --aqua-dark:#1E8FAD;
    --ice:#EAF7FA;
    --ice2:#F6FBFC;
    --gold:#C9A227;
    --white:#FFFFFF;
    --shadow: 0 20px 50px -20px rgba(11,31,36,0.35);
  }
  *{box-sizing:border-box;margin:0;padding:0;}
  html{scroll-behavior:smooth;}
  body{
    font-family:'PT Sans', sans-serif;
    color:var(--ink);
    background:var(--ice2);
    line-height:1.6;
    overflow-x:hidden;
  }
  h1,h2,h3,.display{
    font-family:'PT Serif', serif;
    font-weight:700;
    line-height:1.15;
  }
  a{color:inherit; text-decoration:none;}
  img,svg{display:block; max-width:100%;}
  .container{
    max-width:1160px;
    margin:0 auto;
    padding:0 24px;
  }
  .eyebrow{
    display:inline-flex;
    align-items:center;
    gap:8px;
    font-size:13px;
    letter-spacing:.14em;
    text-transform:uppercase;
    color:var(--aqua-dark);
    font-weight:700;
    margin-bottom:14px;
  }
  .eyebrow::before{
    content:"";
    width:22px; height:2px;
    background:var(--gold);
    display:inline-block;
  }
  .btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:10px;
    padding:15px 30px;
    border-radius:999px;
    font-family:'PT Sans', sans-serif;
    font-weight:700;
    font-size:16px;
    cursor:pointer;
    border:2px solid transparent;
    transition:transform .25s ease, box-shadow .25s ease, background .25s ease;
    white-space:nowrap;
  }
  .btn-primary{
    background:var(--gold);
    color:var(--ink);
    box-shadow:0 10px 30px -8px rgba(201,162,39,.6);
  }
  .btn-primary:hover{ transform:translateY(-2px); box-shadow:0 16px 34px -8px rgba(201,162,39,.7); }
  .btn-ghost{
    border-color:rgba(255,255,255,.5);
    color:var(--white);
  }
  .btn-ghost:hover{ border-color:var(--white); background:rgba(255,255,255,.08); }
  .btn-dark{
    background:var(--deep);
    color:var(--white);
  }
  .btn-dark:hover{ transform:translateY(-2px); box-shadow:0 14px 28px -10px rgba(18,59,68,.6); }

  /* ---------- HEADER ---------- */
  header{
    position:fixed; top:0; left:0; right:0; z-index:100;
    padding:20px 0;
    transition:all .35s ease;
  }
  header.scrolled{
    background:rgba(11,31,36,.92);
    backdrop-filter: blur(10px);
    padding:12px 0;
    box-shadow:0 4px 20px rgba(0,0,0,.15);
  }
  .nav{
    display:flex; align-items:center; justify-content:space-between;
  }
  .logo{
    display:flex; align-items:center; gap:10px;
    color:var(--white);
    font-family:'PT Serif', serif;
    font-weight:700;
    font-size:19px;
    letter-spacing:.01em;
  }
  .logo svg{ width:34px; height:34px; flex-shrink:0; }
  .nav-links{
    display:flex; gap:32px; align-items:center;
    color:rgba(255,255,255,.85);
    font-size:15px;
  }
  .nav-links a:hover{ color:var(--gold); }
  .nav-cta{ display:flex; align-items:center; gap:16px; }
  .nav-phone{ color:var(--white); font-weight:700; font-size:15px; display:none; }
  .burger{ display:none; width:26px; height:20px; position:relative; cursor:pointer; }
  .burger span{ position:absolute; left:0; width:100%; height:2px; background:var(--white); transition:.3s; }
  .burger span:nth-child(1){top:0;} .burger span:nth-child(2){top:9px;} .burger span:nth-child(3){top:18px;}

  /* ---------- HERO ---------- */
  .hero{
    position:relative;
    min-height:100vh;
    display:flex; align-items:center;
    background:radial-gradient(120% 100% at 15% 0%, var(--deep) 0%, var(--ink) 65%);
    color:var(--white);
    padding:140px 0 100px;
    overflow:hidden;
  }
  .hero-grid{
    display:grid;
    grid-template-columns:1.1fr .9fr;
    gap:40px;
    align-items:center;
    position:relative; z-index:2;
  }
  .hero h1{
    font-size:clamp(38px, 5.2vw, 64px);
    letter-spacing:-.01em;
  }
  .hero h1 em{
    font-style:normal;
    color:var(--gold);
  }
  .hero p.lead{
    margin-top:22px;
    font-size:18px;
    color:rgba(255,255,255,.78);
    max-width:480px;
  }
  .hero-actions{
    margin-top:38px;
    display:flex; gap:16px; flex-wrap:wrap;
  }
  .hero-trust{
    margin-top:44px;
    display:flex; gap:34px; flex-wrap:wrap;
  }
  .hero-trust div{ font-size:13px; color:rgba(255,255,255,.6); }
  .hero-trust strong{
    display:block; font-family:'PT Serif',serif; font-size:26px; color:var(--white); font-weight:700;
  }
  .hero-visual{ position:relative; }
  .ripple-bg{
    position:absolute; inset:0;
    z-index:1;
    opacity:.5;
  }
  .ripple-bg circle{
    fill:none; stroke:var(--aqua); stroke-width:1;
    animation:rippleOut 6s ease-out infinite;
  }
  .ripple-bg circle:nth-child(2){ animation-delay:2s; }
  .ripple-bg circle:nth-child(3){ animation-delay:4s; }
  @keyframes rippleOut{
    0%{ transform:scale(.3); opacity:.9; }
    100%{ transform:scale(1.4); opacity:0; }
  }
  .key-draw{
    stroke-dasharray:900;
    stroke-dashoffset:900;
    animation:drawKey 2.6s ease forwards .4s;
  }
  @keyframes drawKey{ to{ stroke-dashoffset:0; } }

  /* ---------- SECTION SHARED ---------- */
  section{ padding:100px 0; }
  .section-head{ max-width:640px; margin-bottom:56px; }
  .section-head h2{ font-size:clamp(28px,3.6vw,42px); }
  .section-head p{ margin-top:16px; font-size:17px; color:#3d5a61; }
  .light{ background:var(--ice2); }
  .deep{ background:var(--deep); color:var(--white); }
  .deep .section-head p{ color:rgba(255,255,255,.72); }

  .reveal{ opacity:0; transform:translateY(28px); transition:opacity .7s ease, transform .7s ease; }
  .reveal.in{ opacity:1; transform:translateY(0); }

  /* ---------- ABOUT ---------- */
  .about-grid{
    display:grid;
    grid-template-columns:.95fr 1.05fr;
    gap:60px;
    align-items:center;
  }
  .about-graphic{
    background:var(--ice);
    border-radius:24px;
    padding:40px;
    position:relative;
    aspect-ratio:1/1;
    display:flex; align-items:center; justify-content:center;
  }
  .about-text p{ margin-bottom:16px; color:#2c454b; font-size:16.5px; }
  .stat-row{
    display:flex; gap:40px; margin-top:32px; flex-wrap:wrap;
  }
  .stat-row div strong{
    display:block; font-family:'PT Serif',serif; font-size:32px; color:var(--aqua-dark);
  }
  .stat-row div span{ font-size:13.5px; color:#5b7378; }

  /* ---------- PRODUCTS ---------- */
  .product-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:28px;
  }
  .product-card{
    background:var(--white);
    border-radius:20px;
    padding:34px 28px;
    box-shadow:var(--shadow);
    display:flex; flex-direction:column; gap:16px;
    border:1px solid rgba(18,59,68,.06);
    transition:transform .3s ease;
  }
  .product-card:hover{ transform:translateY(-6px); }
  .product-card .badge{
    align-self:flex-start;
    background:var(--ice);
    color:var(--aqua-dark);
    font-size:12.5px; font-weight:700;
    padding:5px 12px; border-radius:999px;
  }
  .product-card h3{ font-size:22px; }
  .product-card p{ color:#4a6167; font-size:15px; flex-grow:1; }
  .product-price{ font-family:'PT Serif',serif; font-size:22px; color:var(--ink); }
  .product-price span{ font-size:13px; color:#7c9297; font-family:'PT Sans',sans-serif; }

  /* ---------- BENEFITS ---------- */
  .benefit-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:24px;
  }
  .benefit-card{
    padding:30px 24px;
    border-radius:18px;
    background:rgba(255,255,255,.04);
    border:1px solid rgba(255,255,255,.1);
  }
  .benefit-card svg{ width:36px; height:36px; margin-bottom:18px; }
  .benefit-card h3{ font-size:18px; margin-bottom:8px; color:var(--white); }
  .benefit-card p{ font-size:14.5px; color:rgba(255,255,255,.65); }

  /* ---------- REVIEWS ---------- */
  .review-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:24px;
    margin-bottom:48px;
  }
  .review-card{
    background:var(--white);
    border-radius:18px;
    padding:28px;
    border:1px solid rgba(18,59,68,.08);
  }
  .stars{ color:var(--gold); font-size:16px; letter-spacing:2px; margin-bottom:12px; }
  .review-card p{ font-size:15px; color:#3d5a61; margin-bottom:16px; }
  .review-name{ font-weight:700; font-size:14.5px; }
  .review-note{ font-size:12.5px; color:#8ba0a4; }
  .review-cta{
    background:var(--ice);
    border-radius:20px;
    padding:40px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:24px;
    flex-wrap:wrap;
  }
  .review-cta h3{ font-size:22px; margin-bottom:6px; }
  .review-cta p{ color:#4a6167; font-size:15px; }
  .review-links{ display:flex; gap:12px; flex-wrap:wrap; }

  /* ---------- CONTACT ---------- */
  .contact-grid{
    display:grid;
    grid-template-columns:.85fr 1.15fr;
    gap:50px;
  }
  .contact-info-item{
    display:flex; gap:16px; margin-bottom:28px;
  }
  .contact-info-item svg{ width:26px; height:26px; flex-shrink:0; color:var(--gold); }
  .contact-info-item h4{ font-size:15.5px; margin-bottom:4px; }
  .contact-info-item p{ font-size:14.5px; color:rgba(255,255,255,.65); }
  .contact-form{
    background:var(--white);
    border-radius:22px;
    padding:40px;
    color:var(--ink);
  }
  .contact-form h3{ font-size:22px; margin-bottom:6px; }
  .contact-form > p{ font-size:14.5px; color:#5b7378; margin-bottom:26px; }
  .form-row{ display:flex; gap:16px; margin-bottom:16px; }
  .form-row > *{ flex:1; }
  label{ display:block; font-size:13px; font-weight:700; margin-bottom:6px; color:#2c454b; }
  input, textarea{
    width:100%;
    padding:13px 15px;
    border-radius:12px;
    border:1.5px solid #dce8ea;
    font-family:'PT Sans',sans-serif;
    font-size:15px;
    background:var(--ice2);
    transition:border-color .2s ease;
  }
  input:focus, textarea:focus{ outline:none; border-color:var(--aqua); }
  textarea{ min-height:90px; resize:vertical; }
  .form-note{ font-size:13px; color:#8ba0a4; margin-top:14px; }
  #formMsg{ display:none; margin-top:16px; padding:14px 16px; background:var(--ice); border-radius:10px; font-size:14.5px; color:var(--aqua-dark); font-weight:700; }

  /* ---------- FOOTER ---------- */
  footer{ background:var(--ink); color:rgba(255,255,255,.55); padding:36px 0; font-size:13.5px; }
  .footer-row{ display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap; gap:12px; }

  @media (max-width: 880px){
    .nav-links, .nav-phone{ display:none; }
    .burger{ display:block; }
    .hero-grid{ grid-template-columns:1fr; }
    .hero-visual{ order:-1; max-width:280px; margin:0 auto; }
    .about-grid, .contact-grid{ grid-template-columns:1fr; }
    .product-grid{ grid-template-columns:1fr; }
    .benefit-grid{ grid-template-columns:1fr 1fr; }
    .review-grid{ grid-template-columns:1fr; }
    .form-row{ flex-direction:column; }
    .review-cta{ flex-direction:column; align-items:flex-start; }
  }
</style>
</head>
<body>

<header id="siteHeader">
  <div class="container nav">
    <a href="#top" class="logo">
      <svg viewBox="0 0 40 40" fill="none"><circle cx="20" cy="20" r="19" stroke="#C9A227" stroke-width="1.5"/><path d="M14 20c0-4 2.5-7 6-9 3.5 2 6 5 6 9s-2.5 7-6 9c-3.5-2-6-5-6-9z" fill="#2FB6D9" opacity=".85"/><circle cx="20" cy="20" r="2" fill="#0B1F24"/></svg>
      Ключ живой воды
    </a>
    <nav class="nav-links">
      <a href="#about">О нас</a>
      <a href="#products">Продукция</a>
      <a href="#benefits">Почему мы</a>
      <a href="#reviews">Отзывы</a>
      <a href="#contact">Контакты</a>
    </nav>
    <div class="nav-cta">
      <a href="tel:+77000000000" class="nav-phone">+7 700 000-00-00</a>
      <a href="#contact" class="btn btn-primary" style="padding:11px 22px; font-size:14px;">Заказать воду</a>
      <div class="burger" id="burger"><span></span><span></span><span></span></div>
    </div>
  </div>
</header>

<section class="hero" id="top">
  <svg class="ripple-bg" viewBox="0 0 800 800" preserveAspectRatio="xMidYMid slice">
    <circle cx="650" cy="200" r="60"/>
    <circle cx="650" cy="200" r="60"/>
    <circle cx="650" cy="200" r="60"/>
  </svg>
  <div class="container hero-grid">
    <div>
      <div class="eyebrow">ИП Эврика · Уральск</div>
      <h1>Вода, которая помнит<br><em>вкус источника.</em></h1>
      <p class="lead">«Ключ живой воды» — доставка чистой питьевой воды в Уральске. От скважины до вашего порога, без посредников и без компромиссов в качестве.</p>
      <div class="hero-actions">
        <a href="#contact" class="btn btn-primary">Заказать воду</a>
        <a href="tel:+77000000000" class="btn btn-ghost">Позвонить: +7 700 000-00-00</a>
      </div>
      <div class="hero-trust">
        <div><strong>24 ч</strong>доставка по Уральску</div>
        <div><strong>19 / 5 / 1.5 л</strong>любой объём тары</div>
        <div><strong>100%</strong>контроль качества</div>
      </div>
    </div>
    <div class="hero-visual">
      <svg viewBox="0 0 320 320" fill="none">
        <path class="key-draw" d="M110 210c0 33 27 60 60 60s60-27 60-60-27-60-60-60c-6 0-12 1-17 2M170 150l70-70M215 105l25 25M235 85l25 25" stroke="#2FB6D9" stroke-width="4" stroke-linecap="round" stroke-linejoin="round"/>
        <circle cx="170" cy="210" r="14" fill="#C9A227"/>
        <path d="M40 60c30 0 30 20 60 20s30-20 60-20" stroke="#ffffff" stroke-opacity=".25" stroke-width="2" stroke-linecap="round"/>
        <path d="M20 90c30 0 30 20 60 20s30-20 60-20" stroke="#ffffff" stroke-opacity=".15" stroke-width="2" stroke-linecap="round"/>
      </svg>
    </div>
  </div>
</section>

<section class="light" id="about">
  <div class="container about-grid">
    <div class="about-graphic reveal">
      <svg viewBox="0 0 200 240" width="80%">
        <path d="M75 10h50v25l15 20v165a10 10 0 01-10 10H70a10 10 0 01-10-10V55l15-20V10z" fill="#F6FBFC" stroke="#123B44" stroke-width="2.5"/>
        <rect x="70" y="90" width="60" height="120" rx="4" fill="#2FB6D9" opacity=".85"/>
        <path d="M70 90c10 8 50 8 60 0" stroke="#EAF7FA" stroke-width="2" opacity=".6"/>
        <text x="100" y="150" text-anchor="middle" font-family="PT Serif, serif" font-size="15" fill="#0B1F24" font-weight="700">ключ</text>
      </svg>
    </div>
    <div class="about-text">
      <div class="eyebrow">О компании</div>
      <h2 style="font-size:34px; margin-bottom:20px;">ИП «Эврика» и наш «Ключ живой воды»</h2>
      <p>Мы начинали с простой идеи: у каждой семьи и офиса в Уральске должна быть под рукой по-настоящему чистая вода — без хлора, без лишних солей, без сомнений в качестве.</p>
      <p>Сегодня «Ключ живой воды» — это собственная линия розлива, регулярный лабораторный контроль и доставка, которая приезжает точно тогда, когда обещали.</p>
      <div class="stat-row">
        <div><strong>Уральск</strong><span>город, который мы обслуживаем</span></div>
        <div><strong>19 л</strong><span>основной формат для кулеров</span></div>
        <div><strong>1–2 дня</strong><span>средний срок доставки</span></div>
      </div>
    </div>
  </div>
</section>

<section id="products">
  <div class="container">
    <div class="section-head reveal">
      <div class="eyebrow">Продукция</div>
      <h2>Выберите свой формат</h2>
      <p>Три формата — под дом, офис и путешествия. Тара обменивается при следующей доставке.</p>
    </div>
    <div class="product-grid">
      <div class="product-card reveal">
        <span class="badge">Хит продаж</span>
        <h3>Бутыль 19 л</h3>
        <p>Для кулеров дома и в офисе. Идеально для семьи или небольшой команды — хватает на 1–2 недели.</p>
        <div class="product-price">от 900 ₸ <span>/ бутыль, с обменом тары</span></div>
      </div>
      <div class="product-card reveal">
        <span class="badge">Компактно</span>
        <h3>Бутыль 5 л</h3>
        <p>Удобно, если нет кулера: для готовки, чая и питья каждый день. Лёгкая, не занимает много места.</p>
        <div class="product-price">от 400 ₸ <span>/ бутыль</span></div>
      </div>
      <div class="product-card reveal">
        <span class="badge">С собой</span>
        <h3>Упаковка 1.5 л (×6)</h3>
        <p>Для дачи, дороги и подарков к столу. Продаётся упаковками по 6 бутылок.</p>
        <div class="product-price">от 2 400 ₸ <span>/ упаковка</span></div>
      </div>
    </div>
  </div>
</section>

<section class="deep" id="benefits">
  <div class="container">
    <div class="section-head reveal">
      <div class="eyebrow">Почему выбирают нас</div>
      <h2>Просто, честно, вовремя</h2>
      <p>Мы убрали из процесса всё, что обычно раздражает в доставке воды.</p>
    </div>
    <div class="benefit-grid">
      <div class="benefit-card reveal">
        <svg viewBox="0 0 24 24" fill="none" stroke="#2FB6D9" stroke-width="1.8"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3 3"/></svg>
        <h3>Быстрая доставка</h3>
        <p>Заявка сегодня — бутыль у вас в течение 1–2 дней по Уральску.</p>
      </div>
      <div class="benefit-card reveal">
        <svg viewBox="0 0 24 24" fill="none" stroke="#2FB6D9" stroke-width="1.8"><path d="M12 3l8 4v5c0 5-3.5 8-8 9-4.5-1-8-4-8-9V7l8-4z"/></svg>
        <h3>Контроль качества</h3>
        <p>Каждая партия проходит лабораторную проверку перед розливом.</p>
      </div>
      <div class="benefit-card reveal">
        <svg viewBox="0 0 24 24" fill="none" stroke="#2FB6D9" stroke-width="1.8"><path d="M4 12a8 8 0 0114-5M20 12a8 8 0 01-14 5"/><path d="M18 3v4h-4M6 21v-4h4"/></svg>
        <h3>Обмен тары</h3>
        <p>Пустую бутыль забираем при следующей доставке — доплачивать не нужно.</p>
      </div>
      <div class="benefit-card reveal">
        <svg viewBox="0 0 24 24" fill="none" stroke="#2FB6D9" stroke-width="1.8"><path d="M3 12h18M3 6h18M3 18h18"/></svg>
        <h3>Гибкие тарифы</h3>
        <p>Разовый заказ или подписка на регулярную доставку — выбираете сами.</p>
      </div>
    </div>
  </div>
</section>

<section class="light" id="reviews">
  <div class="container">
    <div class="section-head reveal">
      <div class="eyebrow">Отзывы</div>
      <h2>Что говорят клиенты</h2>
      <p>Несколько примеров того, как выглядит хороший отзыв — замените на реальные, когда они появятся.</p>
    </div>
    <div class="review-grid">
      <div class="review-card reveal">
        <div class="stars">★★★★★</div>
        <p>«Заказываем каждую неделю в офис — ни разу не подвели со временем доставки, вода без привкуса.»</p>
        <div class="review-name">Айгуль К.</div>
        <div class="review-note">пример отзыва</div>
      </div>
      <div class="review-card reveal">
        <div class="stars">★★★★★</div>
        <p>«Понравилось, что тару забирают сразу, не нужно никуда её возить самим.»</p>
        <div class="review-name">Данияр С.</div>
        <div class="review-note">пример отзыва</div>
      </div>
      <div class="review-card reveal">
        <div class="stars">★★★★☆</div>
        <p>«Вода хорошая, вкус приятный. Хотелось бы чуть больше слотов доставки по выходным.»</p>
        <div class="review-name">Марина Т.</div>
        <div class="review-note">пример отзыва</div>
      </div>
    </div>
    <div class="review-cta reveal">
      <div>
        <h3>Уже заказывали у нас воду?</h3>
        <p>Оставьте отзыв в 2ГИС или Google — это займёт минуту и очень помогает нам расти.</p>
      </div>
      <div class="review-links">
        <a href="#" class="btn btn-dark">Отзыв в 2ГИС</a>
        <a href="#" class="btn btn-dark">Отзыв в Google</a>
      </div>
    </div>
  </div>
</section>

<section class="deep" id="contact">
  <div class="container contact-grid">
    <div>
      <div class="eyebrow">Контакты</div>
      <h2 style="font-size:32px; margin-bottom:28px;">Закажите воду прямо сейчас</h2>
      <div class="contact-info-item">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M22 16.9v3a2 2 0 01-2.2 2 19.8 19.8 0 01-8.6-3 19.5 19.5 0 01-6-6 19.8 19.8 0 01-3-8.7A2 2 0 014.1 2h3a2 2 0 012 1.7c.1 1 .3 2 .6 3a2 2 0 01-.5 2.1L8 10a16 16 0 006 6l1.2-1.2a2 2 0 012.1-.5c1 .3 2 .5 3 .6a2 2 0 011.7 2z"/></svg>
        <div><h4>Телефон / WhatsApp</h4><p>+7 700 000-00-00</p></div>
      </div>
      <div class="contact-info-item">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M21 10c0 7-9 12-9 12s-9-5-9-12a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
        <div><h4>Адрес</h4><p>г. Уральск, ул. Примерная, 1</p></div>
      </div>
      <div class="contact-info-item">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3 3"/></svg>
        <div><h4>Режим работы</h4><p>Пн–Сб: 9:00–19:00</p></div>
      </div>
    </div>
    <div class="contact-form reveal">
      <h3>Оставить заявку</h3>
      <p>Укажите объём и адрес — перезвоним в течение часа.</p>
      <form id="orderForm">
        <div class="form-row">
          <div><label>Имя</label><input type="text" required placeholder="Как к вам обращаться"></div>
          <div><label>Телефон</label><input type="tel" required placeholder="+7 ___ ___-__-__"></div>
        </div>
        <div style="margin-bottom:16px;">
          <label>Адрес доставки</label>
          <input type="text" required placeholder="Улица, дом, квартира">
        </div>
        <div style="margin-bottom:16px;">
          <label>Комментарий</label>
          <textarea placeholder="Например: 2 бутыли по 19 л, желательно после 18:00"></textarea>
        </div>
        <button type="submit" class="btn btn-primary" style="width:100%;">Отправить заявку</button>
        <div id="formMsg">Спасибо! Заявка получена — мы свяжемся с вами в ближайшее время.</div>
        <p class="form-note">Форма пока не подключена к реальной отправке — свяжитесь с разработчиком, чтобы подключить приём заявок на WhatsApp, почту или CRM.</p>
      </form>
    </div>
  </div>
</section>

<footer>
  <div class="container footer-row">
    <div>© 2026 ИП «Эврика» · «Ключ живой воды» · г. Уральск</div>
    <div>Сделано с заботой о качестве воды</div>
  </div>
</footer>

<script>
  const header = document.getElementById('siteHeader');
  window.addEventListener('scroll', () => {
    header.classList.toggle('scrolled', window.scrollY > 40);
  });

  const revealEls = document.querySelectorAll('.reveal');
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('in'); });
  }, { threshold: 0.15 });
  revealEls.forEach(el => io.observe(el));

  const burger = document.getElementById('burger');
  const navLinks = document.querySelector('.nav-links');
  burger.addEventListener('click', () => {
    const open = navLinks.style.display === 'flex';
    navLinks.style.display = open ? 'none' : 'flex';
    navLinks.style.cssText += open ? '' : 'position:fixed; top:70px; left:0; right:0; background:#0B1F24; flex-direction:column; padding:24px; gap:20px;';
  });

  const form = document.getElementById('orderForm');
  const msg = document.getElementById('formMsg');
  form.addEventListener('submit', (e) => {
    e.preventDefault();
    msg.style.display = 'block';
    form.reset();
  });
</script>

</body>
</html>

