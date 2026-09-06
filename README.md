
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ключ здоровья — артезианская вода в Уральске</title>
<meta name="description" content="Ключ здоровья — природная артезианская вода. ИП Эврика, Уральск, Казахстан.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,500;0,9..144,600;1,9..144,500&family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #0b1017;
    --bg-alt: #101823;
    --bg-alt-2: #0a0f16;
    --text: #ece8de;
    --muted: #9fb0a9;
    --accent: #5FA8E0;
    --accent-soft: rgba(95,168,224,0.14);
    --accent-2: #cda874;
    --line: rgba(236,232,222,0.12);
    --line-strong: rgba(236,232,222,0.22);
    --serif: 'Fraunces', serif;
    --sans: 'Manrope', sans-serif;
  }

  *{margin:0;padding:0;box-sizing:border-box;}

  html{scroll-behavior:smooth;}

  body{
    background:var(--bg);
    color:var(--text);
    font-family:var(--sans);
    font-size:16px;
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
  }

  a{color:inherit;text-decoration:none;}
  ul{list-style:none;}
  img{max-width:100%;display:block;}

  .wrap{
    max-width:1180px;
    margin:0 auto;
    padding:0 32px;
  }

  .eyebrow{
    font-family:var(--sans);
    font-size:12.5px;
    font-weight:700;
    letter-spacing:0.22em;
    text-transform:uppercase;
    color:var(--accent);
  }

  h1,h2,h3{
    font-family:var(--serif);
    font-weight:500;
    line-height:1.08;
    letter-spacing:-0.01em;
  }

  p{color:var(--muted);}

  .btn{
    display:inline-flex;
    align-items:center;
    gap:10px;
    padding:15px 28px;
    border-radius:999px;
    font-family:var(--sans);
    font-weight:700;
    font-size:14.5px;
    letter-spacing:0.02em;
    cursor:pointer;
    transition:transform .35s cubic-bezier(.2,.8,.2,1), background .3s, border-color .3s, color .3s;
    border:1px solid transparent;
    white-space:nowrap;
  }
  .btn:hover{transform:translateY(-2px);}
  .btn-primary{background:var(--accent);color:#08120f;}
  .btn-primary:hover{background:#93d3c4;}
  .btn-ghost{border-color:var(--line-strong);color:var(--text);}
  .btn-ghost:hover{border-color:var(--accent);color:var(--accent);}

  /* ---------- HEADER ---------- */
  header{
    position:fixed;
    top:0;left:0;right:0;
    z-index:100;
    padding:22px 0;
    transition:background .4s, padding .4s, border-color .4s;
    border-bottom:1px solid transparent;
  }
  header.scrolled{
    background:rgba(11,21,18,0.86);
    backdrop-filter:blur(14px);
    -webkit-backdrop-filter:blur(14px);
    padding:14px 0;
    border-bottom:1px solid var(--line);
  }
  header .wrap{display:flex;align-items:center;justify-content:space-between;gap:24px;}

  .logo{
    font-family:var(--serif);
    font-size:19px;
    font-weight:600;
    letter-spacing:0.01em;
    display:flex;
    align-items:center;
    gap:10px;
  }
  .logo .mark{
    width:30px;height:30px;
    flex-shrink:0;
  }

  nav.mainnav ul{display:flex;gap:32px;}
  nav.mainnav a{
    font-size:12.5px;
    font-weight:700;
    letter-spacing:0.08em;
    text-transform:uppercase;
    color:var(--muted);
    transition:color .3s;
  }
  nav.mainnav a:hover{color:var(--text);}

  .header-right{display:flex;align-items:center;gap:14px;}
  .icon-btn{
    width:38px;height:38px;
    border-radius:50%;
    border:1px solid var(--line-strong);
    display:flex;
    align-items:center;
    justify-content:center;
    transition:border-color .3s, color .3s;
    color:var(--muted);
    flex-shrink:0;
  }
  .icon-btn:hover{border-color:var(--accent);color:var(--accent);}
  .icon-btn svg{width:16px;height:16px;}
  .header-phone{
    font-family:var(--serif);
    font-size:16px;
    font-weight:500;
    letter-spacing:0.01em;
  }
  .header-phone:hover{color:var(--accent);}

  .burger{display:none;width:26px;height:20px;position:relative;cursor:pointer;flex-shrink:0;}
  .burger span{position:absolute;left:0;right:0;height:2px;background:var(--text);transition:.3s;}
  .burger span:nth-child(1){top:0;}
  .burger span:nth-child(2){top:9px;}
  .burger span:nth-child(3){top:18px;}

  /* ---------- HERO ---------- */
  .hero{
    position:relative;
    min-height:100svh;
    display:flex;
    align-items:center;
    padding:140px 0 100px;
    overflow:hidden;
  }
  .ripple-field{
    position:absolute;
    top:50%;left:50%;
    width:1100px;height:1100px;
    transform:translate(-50%,-50%);
    pointer-events:none;
    z-index:0;
  }
  .ripple-field svg{width:100%;height:100%;}
  .ripple-field circle{
    fill:none;
    stroke:var(--accent);
    stroke-width:1;
    opacity:0;
    transform-origin:center;
    animation:ripple 7s ease-out infinite;
  }
  .ripple-field circle:nth-child(2){animation-delay:1.6s;}
  .ripple-field circle:nth-child(3){animation-delay:3.2s;}
  .ripple-field circle:nth-child(4){animation-delay:4.8s;}
  @keyframes ripple{
    0%{ r:20; opacity:0; }
    12%{ opacity:0.35; }
    100%{ r:540; opacity:0; }
  }

  .hero-inner{position:relative;z-index:2;max-width:760px;}
  .hero .eyebrow{margin-bottom:22px;display:block;}
  .hero h1{
    font-size:clamp(48px, 8vw, 92px);
    margin-bottom:26px;
  }
  .hero h1 em{
    font-style:italic;
    color:var(--accent);
  }
  .hero p.lead{
    font-size:19px;
    max-width:520px;
    margin-bottom:40px;
    color:var(--muted);
  }
  .hero-ctas{display:flex;gap:16px;flex-wrap:wrap;}

  .hero-scroll{
    position:absolute;
    bottom:36px;left:32px;
    z-index:2;
    display:flex;
    align-items:center;
    gap:10px;
    font-size:12px;
    letter-spacing:0.14em;
    text-transform:uppercase;
    color:var(--muted);
  }
  .hero-scroll .line{width:34px;height:1px;background:var(--line-strong);position:relative;overflow:hidden;}
  .hero-scroll .line::after{
    content:'';position:absolute;left:-100%;top:0;bottom:0;width:100%;
    background:var(--accent);
    animation:scrollline 2.2s ease-in-out infinite;
  }
  @keyframes scrollline{ 0%{left:-100%;} 50%{left:0;} 100%{left:100%;} }

  .hero-quote{
    position:absolute;
    right:32px;
    bottom:100px;
    z-index:2;
    max-width:300px;
    padding-left:20px;
    border-left:2px solid var(--accent);
  }
  .hero-quote p{
    font-family:var(--serif);
    font-style:italic;
    font-size:16.5px;
    line-height:1.45;
    color:var(--text);
    margin-bottom:14px;
  }
  .hero-quote .hq-source{
    font-size:11.5px;
    letter-spacing:0.1em;
    text-transform:uppercase;
    color:var(--muted);
    font-weight:700;
  }

  /* wave divider */
  .wave{display:block;width:100%;line-height:0;}
  .wave svg{width:100%;height:auto;display:block;}

  /* ---------- SECTION GENERIC ---------- */
  section{position:relative;}
  .section-pad{padding:120px 0;}
  .section-head{max-width:620px;margin-bottom:64px;}
  .section-head .eyebrow{display:block;margin-bottom:18px;}
  .section-head h2{font-size:clamp(32px,4.2vw,46px);color:var(--text);}
  .section-head p{margin-top:18px;font-size:16.5px;}

  [data-reveal]{
    opacity:0;
    transform:translateY(28px);
    transition:opacity .9s cubic-bezier(.2,.7,.2,1), transform .9s cubic-bezier(.2,.7,.2,1);
  }
  [data-reveal].in{opacity:1;transform:translateY(0);}

  /* ---------- ABOUT ---------- */
  .about{background:var(--bg-alt);}
  .about-grid{
    display:grid;
    grid-template-columns:1.1fr 0.9fr;
    gap:70px;
    align-items:center;
  }
  .about-text h2{font-size:clamp(30px,3.6vw,42px);margin-bottom:24px;color:var(--text);}
  .about-text p{font-size:16.5px;margin-bottom:16px;}
  .about-text p:last-of-type{margin-bottom:0;}

  .about-visual{
    position:relative;
    aspect-ratio:1/1;
    border-radius:50%;
    background:radial-gradient(circle at 35% 30%, rgba(127,201,184,0.22), rgba(127,201,184,0.02) 65%);
    border:1px solid var(--line);
    display:flex;
    align-items:center;
    justify-content:center;
  }
  .about-visual .ring{
    position:absolute;
    border-radius:50%;
    border:1px solid var(--line);
  }
  .about-visual .ring.r1{inset:14%;}
  .about-visual .ring.r2{inset:28%;border-color:rgba(127,201,184,0.35);}
  .about-visual .core{
    text-align:center;
    font-family:var(--serif);
  }
  .about-visual .core .num{
    font-size:15px;
    letter-spacing:0.05em;
    color:var(--accent);
    text-transform:uppercase;
    font-family:var(--sans);
    font-weight:700;
  }
  .about-visual .core .label{
    font-size:22px;
    margin-top:10px;
    color:var(--text);
    max-width:180px;
  }

  /* ---------- FEATURES ---------- */
  .features-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:1px;
    background:var(--line);
    border:1px solid var(--line);
    border-radius:18px;
    overflow:hidden;
  }
  .feature{
    background:var(--bg);
    padding:42px 36px;
    transition:background .35s;
  }
  .feature:hover{background:var(--bg-alt-2);}
  .feature .ficon{
    width:38px;height:38px;
    margin-bottom:22px;
    color:var(--accent);
  }
  .feature h3{
    font-size:19px;
    color:var(--text);
    margin-bottom:10px;
    font-weight:500;
  }
  .feature p{font-size:14.5px;}

  /* ---------- NUMBERED LIST ---------- */
  .numbered-list{border-top:1px solid var(--line);}
  .num-row{
    display:grid;
    grid-template-columns:110px 1fr;
    gap:40px;
    align-items:start;
    padding:38px 0;
    border-bottom:1px solid var(--line);
  }
  .num-index{
    font-family:var(--serif);
    font-size:44px;
    font-weight:400;
    color:var(--accent);
    line-height:1;
  }
  .num-body h3{
    font-size:21px;
    color:var(--text);
    font-weight:500;
    margin-bottom:10px;
  }
  .num-body p{font-size:15.5px;max-width:560px;}

  /* ---------- ASSORTMENT ---------- */
  .assort{background:var(--bg-alt);}
  .assort-grid{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:16px;
  }
  .bottle-card{
    border:1px solid var(--line);
    border-radius:16px;
    padding:36px 26px;
    text-align:center;
    transition:border-color .35s, transform .35s;
  }
  .bottle-card:hover{border-color:var(--accent);transform:translateY(-6px);}
  .bottle-card svg{width:44px;height:auto;margin:0 auto 22px;color:var(--accent);}
  .bottle-card .vol{
    font-family:var(--serif);
    font-size:26px;
    color:var(--text);
    margin-bottom:8px;
  }
  .bottle-card .use{
    font-size:13px;
    color:var(--muted);
    letter-spacing:0.02em;
  }

  /* ---------- SPLIT (для дома / для бизнеса) ---------- */
  .split-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:1px;
    background:var(--line);
    border:1px solid var(--line);
    border-radius:18px;
    overflow:hidden;
  }
  .split-card{
    background:var(--bg);
    padding:56px 48px;
  }
  .split-card .eyebrow{display:block;margin-bottom:18px;}
  .split-card h3{font-size:26px;color:var(--text);margin-bottom:16px;font-weight:500;}
  .split-card p{font-size:15.5px;margin-bottom:26px;}
  .split-card ul{margin-bottom:30px;}
  .split-card li{
    font-size:14.5px;
    color:var(--muted);
    padding:10px 0;
    border-top:1px solid var(--line);
    display:flex;
    gap:12px;
  }
  .split-card li:first-of-type{border-top:none;}
  .split-card li::before{
    content:'—';
    color:var(--accent);
    flex-shrink:0;
  }

  /* ---------- CONTACT ---------- */
  .contact{
    background:var(--bg-alt-2);
    text-align:center;
    padding:130px 0 110px;
  }
  .contact .eyebrow{display:block;margin-bottom:22px;}
  .contact h2{
    font-size:clamp(30px,4vw,44px);
    max-width:640px;
    margin:0 auto 40px;
    color:var(--text);
  }
  .contact-phone{
    display:inline-block;
    font-family:var(--serif);
    font-size:clamp(38px,7vw,64px);
    font-weight:500;
    letter-spacing:-0.01em;
    color:var(--text);
    margin-bottom:14px;
    transition:color .3s;
  }
  .contact-phone:hover{color:var(--accent);}
  .contact-sub{font-size:15px;margin-bottom:44px;}
  .contact-ctas{display:flex;gap:16px;justify-content:center;flex-wrap:wrap;margin-bottom:56px;}
  .contact-meta{
    display:flex;
    justify-content:center;
    gap:52px;
    flex-wrap:wrap;
    padding-top:44px;
    border-top:1px solid var(--line);
    max-width:720px;
    margin:0 auto;
  }
  .contact-meta div{text-align:left;}
  .contact-meta .k{
    font-size:11.5px;
    letter-spacing:0.14em;
    text-transform:uppercase;
    color:var(--accent);
    margin-bottom:8px;
    font-weight:700;
  }
  .contact-meta .v{font-size:15px;color:var(--text);}

  /* ---------- FOOTER ---------- */
  .promo-bar{
    background:var(--bg-alt);
    border-top:1px solid var(--line);
    border-bottom:1px solid var(--line);
    padding:26px 0;
  }
  .promo-bar .wrap{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:24px;
    flex-wrap:wrap;
    text-align:center;
  }
  .promo-bar p{
    font-size:13px;
    font-weight:700;
    letter-spacing:0.1em;
    text-transform:uppercase;
    color:var(--text);
  }
  .promo-bar .btn{padding:11px 22px;}

  footer{
    padding:56px 0 36px;
    border-top:none;
  }
  footer .wrap{
    display:grid;
    grid-template-columns:1.2fr 1fr 1fr;
    gap:40px;
    align-items:start;
  }
  footer .fcol .k{
    font-size:11.5px;
    letter-spacing:0.14em;
    text-transform:uppercase;
    color:var(--accent);
    font-weight:700;
    margin-bottom:14px;
  }
  footer .fcol div.v{font-size:14px;color:var(--muted);margin-bottom:8px;line-height:1.5;}
  footer .fcol a.v{display:block;font-size:14px;color:var(--muted);margin-bottom:8px;transition:color .3s;}
  footer .fcol a.v:hover{color:var(--accent);}
  footer .fbottom{
    max-width:1180px;
    margin:44px auto 0;
    padding:22px 32px 0;
    border-top:1px solid var(--line);
    font-size:12.5px;
    color:var(--muted);
    display:flex;
    justify-content:space-between;
    flex-wrap:wrap;
    gap:10px;
  }

  /* ---------- RESPONSIVE ---------- */
  @media (max-width:900px){
    .about-grid{grid-template-columns:1fr;gap:44px;}
    .about-visual{max-width:340px;margin:0 auto;}
    .features-grid{grid-template-columns:1fr 1fr;}
    .assort-grid{grid-template-columns:1fr 1fr;}
    .split-grid{grid-template-columns:1fr;}
  }

  @media (max-width:720px){
    .wrap{padding:0 22px;}
    nav.mainnav{
      position:fixed;
      top:0;right:0;
      height:100svh;
      width:78%;
      max-width:320px;
      background:var(--bg-alt-2);
      border-left:1px solid var(--line);
      padding:110px 32px 40px;
      transform:translateX(100%);
      transition:transform .45s cubic-bezier(.2,.8,.2,1);
      z-index:99;
    }
    nav.mainnav.open{transform:translateX(0);}
    nav.mainnav ul{flex-direction:column;gap:26px;}
    nav.mainnav a{font-size:18px;}
    .header-phone{display:none;}
    .icon-btn{display:none;}
    .burger{display:block;}
    .hero{padding:120px 0 80px;min-height:auto;}
    .hero-scroll{display:none;}
    .hero-quote{display:none;}
    .section-pad{padding:80px 0;}
    .features-grid{grid-template-columns:1fr;}
    .num-row{grid-template-columns:1fr;gap:12px;}
    .num-index{font-size:32px;}
    .assort-grid{grid-template-columns:1fr 1fr;}
    .split-card{padding:40px 28px;}
    .contact-meta{flex-direction:column;gap:24px;align-items:center;}
    .contact-meta div{text-align:center;}
    footer .wrap{grid-template-columns:1fr;gap:32px;}
    .fbottom{flex-direction:column;text-align:center;}
  }

  @media (prefers-reduced-motion: reduce){
    *{animation:none !important;transition:none !important;}
    [data-reveal]{opacity:1;transform:none;}
  }

  :focus-visible{outline:2px solid var(--accent);outline-offset:3px;}
</style>
</head>
<body>

<header id="siteHeader">
  <div class="wrap">
    <a href="#top" class="logo">
      <svg class="mark" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M15 3C15 3 6 13.5 6 19.2C6 24.2 10 27 15 27C20 27 24 24.2 24 19.2C24 13.5 15 3 15 3Z" stroke="#5FA8E0" stroke-width="1.6"/>
      </svg>
      Ключ здоровья
    </a>

    <nav class="mainnav" id="mainNav">
      <ul>
        <li><a href="#about" class="nav-link">О воде</a></li>
        <li><a href="#features" class="nav-link">Преимущества</a></li>
        <li><a href="#locations" class="nav-link">Где купить</a></li>
        <li><a href="#assort" class="nav-link">Тара</a></li>
        <li><a href="#contact" class="nav-link">Для бизнеса</a></li>
        <li><a href="#contact" class="nav-link">Контакты</a></li>
      </ul>
    </nav>

    <div class="header-right">
      <a href="tel:+77055710028" class="header-phone">+7 705 571 00 28</a>
      <a href="tel:+77055710028" class="icon-btn" aria-label="Позвонить">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M6.6 10.8C8.1 13.7 10.3 15.9 13.2 17.4L15.4 15.2C15.7 14.9 16.1 14.8 16.5 15C17.7 15.4 19 15.6 20.3 15.6C20.9 15.6 21.4 16.1 21.4 16.7V20.2C21.4 20.8 20.9 21.3 20.3 21.3C10.7 21.3 2.7 13.3 2.7 3.7C2.7 3.1 3.2 2.6 3.8 2.6H7.3C7.9 2.6 8.4 3.1 8.4 3.7C8.4 5 8.6 6.3 9 7.5C9.1 7.9 9 8.3 8.7 8.6L6.6 10.8Z"/></svg>
      </a>
      <a href="https://wa.me/77055710028" class="icon-btn" target="_blank" rel="noopener" aria-label="WhatsApp">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2C6.5 2 2 6.5 2 12C2 13.8 2.5 15.5 3.3 17L2 22L7.2 20.7C8.6 21.5 10.3 22 12 22C17.5 22 22 17.5 22 12C22 6.5 17.5 2 12 2Z"/><path d="M8.5 8.5C8.5 8.5 9 8 9.5 8C10 8 10.5 9 10.7 9.5C10.9 10 10.1 10.6 10.1 11C10.1 11.4 10.6 12.2 11.3 12.9C12 13.6 12.8 14.1 13.2 14.1C13.6 14.1 14.2 13.3 14.7 13.5C15.2 13.7 16.2 14.2 16.2 14.7C16.2 15.2 15.7 15.7 15.2 15.9C14.6 16.1 13.7 16.1 12.2 15.5C10.5 14.8 9.1 13.4 8.4 11.7C7.8 10.2 7.8 9.3 8 8.7"/></svg>
      </a>
      <a href="#contact" class="btn btn-primary" style="padding:12px 22px;">Связаться</a>
      <div class="burger" id="burger"><span></span><span></span><span></span></div>
    </div>
  </div>
</header>

<main id="top">

  <!-- HERO -->
  <section class="hero">
    <div class="ripple-field" aria-hidden="true">
      <svg viewBox="0 0 1100 1100">
        <circle cx="550" cy="550" r="20"/>
        <circle cx="550" cy="550" r="20"/>
        <circle cx="550" cy="550" r="20"/>
        <circle cx="550" cy="550" r="20"/>
      </svg>
    </div>
    <div class="wrap hero-inner">
      <span class="eyebrow">Артезианская вода · Уральск</span>
      <h1>Вода из<br>настоящего <em>родника</em><br>земли Приуралья</h1>
      <p class="lead">«Ключ здоровья» — природная артезианская вода без лишней обработки. ИП Эврика бережно добывает и разливает воду, сохраняя её естественный минеральный состав.</p>
      <div class="hero-ctas">
        <a href="tel:+77055710028" class="btn btn-primary">Позвонить: +7 705 571 00 28</a>
        <a href="#about" class="btn btn-ghost">Узнать о воде</a>
      </div>
    </div>

    <div class="hero-quote" data-reveal>
      <span class="hq-bar"></span>
      <p>«Мы разливаем воду так, как хотели бы, чтобы её разливали для нашей собственной семьи»</p>
      <span class="hq-source">Ключ здоровья · Уральск</span>
    </div>
    <div class="hero-scroll"><span class="line"></span>Листайте вниз</div>
  </section>

  <div class="wave" aria-hidden="true">
    <svg viewBox="0 0 1440 90" preserveAspectRatio="none"><path d="M0,40 C240,90 480,0 720,30 C960,60 1200,10 1440,45 L1440,90 L0,90 Z" fill="#101823"/></svg>
  </div>

  <!-- ABOUT -->
  <section class="about" id="about">
    <div class="wrap section-pad">
      <div class="about-grid">
        <div class="about-text" data-reveal>
          <h2>Что делает воду<br>«Ключ здоровья» особенной</h2>
          <p>Вода добывается из артезианского горизонта Западно-Казахстанской области — территории, где подземные пласты веками фильтруют влагу через природные слои песка и известняка.</p>
          <p>Такая вода относится к гидрокарбонатному кальциево-магниевому типу — она физиологически сбалансирована и сохраняет минералы, которые организм получает вместе с питьевой водой каждый день.</p>
          <p>Мы не продаём готовую бутилированную воду — вода проходит многоступенчатую фильтрацию и наливается свежей прямо в вашу тару или в тару, которую можно купить у нас на месте.</p>
        </div>
        <div class="about-visual" data-reveal>
          <div class="ring r1"></div>
          <div class="ring r2"></div>
          <div class="core">
            <div class="num">Западно-Казахстанская область</div>
            <div class="label">Артезианский источник</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FEATURES -->
  <section class="section-pad" id="features">
    <div class="wrap">
      <div class="section-head" data-reveal>
        <span class="eyebrow">Преимущества</span>
        <h2>Почему выбирают «Ключ здоровья»</h2>
        <p>Каждая партия проходит контроль качества — от источника до готовой тары.</p>
      </div>

      <div class="numbered-list" data-reveal>
        <div class="num-row">
          <div class="num-index">01</div>
          <div class="num-body">
            <h3>Природная минерализация</h3>
            <p>Сбалансированный состав солей и минералов без искусственного обогащения — вода сохраняет то, что дала ей земля.</p>
          </div>
        </div>
        <div class="num-row">
          <div class="num-index">02</div>
          <div class="num-body">
            <h3>Контроль качества</h3>
            <p>Регулярная проверка состава и чистоты на каждом этапе — от источника до готовой тары.</p>
          </div>
        </div>
        <div class="num-row">
          <div class="num-index">03</div>
          <div class="num-body">
            <h3>Без лишней обработки</h3>
            <p>Минимальное вмешательство сохраняет естественный вкус воды таким, какой он есть у источника.</p>
          </div>
        </div>
        <div class="num-row">
          <div class="num-index">04</div>
          <div class="num-body">
            <h3>Тара под любой объём</h3>
            <p>Свою тару принесёте сами или купите чистую у нас — 1 л, 1,5 л, 5 л, 10 л и 19 л для кулера.</p>
          </div>
        </div>
        <div class="num-row">
          <div class="num-index">05</div>
          <div class="num-body">
            <h3>Стабильный вкус</h3>
            <p>Один и тот же источник — один и тот же узнаваемый вкус вне зависимости от сезона.</p>
          </div>
        </div>
        <div class="num-row">
          <div class="num-index">06</div>
          <div class="num-body">
            <h3>Местное производство</h3>
            <p>Работаем в Уральске — знаем регион и отвечаем за качество, а не за громкие обещания.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- LOCATIONS -->
  <section class="section-pad" id="locations">
    <div class="wrap">
      <div class="section-head" data-reveal>
        <span class="eyebrow">Где купить</span>
        <h2>Точки продажи в Уральске</h2>
        <p>Воду «Ключ здоровья» можно купить в нескольких точках города — выбирайте ближайшую.</p>
      </div>

      <div class="features-grid" data-reveal>
        <div class="feature">
          <svg class="ficon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M12 2C12 2 5 11 5 15.5C5 19.6 8.1 22 12 22C15.9 22 19 19.6 19 15.5C19 11 12 2 12 2Z"/><circle cx="12" cy="14" r="2.4"/></svg>
          <h3>Ул. Темира Масина, 16в</h3>
          <p>Также встречается как дом 16/1</p>
        </div>
        <div class="feature">
          <svg class="ficon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M12 2C12 2 5 11 5 15.5C5 19.6 8.1 22 12 22C15.9 22 19 19.6 19 15.5C19 11 12 2 12 2Z"/><circle cx="12" cy="14" r="2.4"/></svg>
          <h3>Пр. Абулхаир хана, 44/1в</h3>
          <p>&nbsp;</p>
        </div>
        <div class="feature">
          <svg class="ficon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M12 2C12 2 5 11 5 15.5C5 19.6 8.1 22 12 22C15.9 22 19 19.6 19 15.5C19 11 12 2 12 2Z"/><circle cx="12" cy="14" r="2.4"/></svg>
          <h3>Ул. 25 Чапаевской дивизии, 8/1Б</h3>
          <p>Посёлок Зачаганск</p>
        </div>
      </div>

      <p style="margin-top:28px;font-size:14.5px;">Уточняйте часы работы и наличие нужного объёма тары по телефону: <a href="tel:+77055710028" style="color:var(--accent);font-weight:600;">+7 705 571 00 28</a></p>
    </div>
  </section>

  <!-- ASSORTMENT -->
  <section class="assort" id="assort">
    <div class="wrap section-pad">
      <div class="section-head" data-reveal>
        <span class="eyebrow">Как это работает</span>
        <h2>Вода на разлив, а не бутилированная</h2>
        <p>Мы не продаём готовые запечатанные бутылки — вода наливается свежей, отфильтрованной, прямо при вас.</p>
      </div>

      <div class="split-grid" data-reveal style="margin-bottom:56px;">
        <div class="split-card">
          <span class="eyebrow">Вариант 1</span>
          <h3>Приходите со своей тарой</h3>
          <p>Принесите любую подходящую канистру или бутыль — нальём в неё свежую отфильтрованную воду нужного объёма.</p>
        </div>
        <div class="split-card">
          <span class="eyebrow">Вариант 2</span>
          <h3>Купите тару у нас</h3>
          <p>Нет своей тары — купите чистую пустую тару на месте, и мы сразу наполним её свежей водой.</p>
        </div>
      </div>

      <div class="section-head" data-reveal style="margin-bottom:36px;">
        <span class="eyebrow">Доступные объёмы</span>
        <h2 style="font-size:clamp(26px,3vw,34px);">Тара для налива</h2>
      </div>
      <div class="assort-grid" data-reveal>
        <div class="bottle-card">
          <svg viewBox="0 0 24 40" fill="none" stroke="currentColor" stroke-width="1.3"><path d="M9 2H15V7L17 10V37C17 38 16 39 15 39H9C8 39 7 38 7 37V10L9 7V2Z"/><line x1="7" y1="15" x2="17" y2="15"/></svg>
          <div class="vol">1 л</div>
          <div class="use">На каждый день</div>
        </div>
        <div class="bottle-card">
          <svg viewBox="0 0 24 40" fill="none" stroke="currentColor" stroke-width="1.3"><path d="M9 2H15V7L17 10V37C17 38 16 39 15 39H9C8 39 7 38 7 37V10L9 7V2Z"/><line x1="7" y1="16" x2="17" y2="16"/></svg>
          <div class="vol">1,5 л</div>
          <div class="use">Для дома</div>
        </div>
        <div class="bottle-card">
          <svg viewBox="0 0 24 40" fill="none" stroke="currentColor" stroke-width="1.3"><path d="M8 2H16V6L18 9V37C18 38 17 39 16 39H8C7 39 6 38 6 37V9L8 6V2Z"/><line x1="6" y1="18" x2="18" y2="18"/></svg>
          <div class="vol">5 л</div>
          <div class="use">Для дома и офиса</div>
        </div>
        <div class="bottle-card">
          <svg viewBox="0 0 24 40" fill="none" stroke="currentColor" stroke-width="1.3"><path d="M8 2H16V6L18 9V37C18 38 17 39 16 39H8C7 39 6 38 6 37V9L8 6V2Z"/><line x1="6" y1="18" x2="18" y2="18"/></svg>
          <div class="vol">10 л</div>
          <div class="use">Для семьи</div>
        </div>
        <div class="bottle-card">
          <svg viewBox="0 0 24 40" fill="none" stroke="currentColor" stroke-width="1.3"><path d="M7 2H17V6L19 10V37C19 38 18 39 17 39H7C6 39 5 38 5 37V10L7 6V2Z"/><line x1="5" y1="20" x2="19" y2="20"/></svg>
          <div class="vol">19 л</div>
          <div class="use">Для кулера</div>
        </div>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section class="contact" id="contact">
    <div class="wrap">
      <span class="eyebrow">Контакты</span>
      <h2>Остались вопросы о воде или объёме заказа? Звоните — ответим и подскажем.</h2>
      <a href="tel:+77055710028" class="contact-phone">+7 705 571 00 28</a>
      <div class="contact-sub">Ежедневно · Уральск, Казахстан</div>
      <div class="contact-ctas">
        <a href="tel:+77055710028" class="btn btn-primary">Позвонить</a>
        <a href="https://wa.me/77055710028" class="btn btn-ghost" target="_blank" rel="noopener">Написать в WhatsApp</a>
      </div>
      <div class="contact-meta">
        <div>
          <div class="k">Компания</div>
          <div class="v">ИП Эврика · «Ключ здоровья»</div>
        </div>
        <div>
          <div class="k">Город</div>
          <div class="v">Уральск, Западно-Казахстанская область</div>
        </div>
        <div>
          <div class="k">Телефон</div>
          <div class="v">+7 705 571 00 28</div>
        </div>
      </div>
    </div>
  </section>

</main>

<div class="promo-bar">
  <div class="wrap">
    <p>Несколько точек продажи в Уральске — выбирайте ближайшую</p>
    <a href="#locations" class="btn btn-primary">Смотреть адреса</a>
  </div>
</div>

<footer>
  <div class="wrap">
    <div class="fcol">
      <a href="#top" class="logo">
        <svg class="mark" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M15 3C15 3 6 13.5 6 19.2C6 24.2 10 27 15 27C20 27 24 24.2 24 19.2C24 13.5 15 3 15 3Z" stroke="#5FA8E0" stroke-width="1.6"/>
        </svg>
        Ключ здоровья
      </a>
      <div class="v" style="margin-top:16px;max-width:240px;">Природная артезианская вода в Уральске. ИП Эврика.</div>
    </div>
    <div class="fcol">
      <div class="k">Точки продажи</div>
      <div class="v">Ул. Темира Масина, 16в</div>
      <div class="v">Пр. Абулхаир хана, 44/1в</div>
      <div class="v">Ул. 25 Чапаевской дивизии, 8/1Б (Зачаганск)</div>
    </div>
    <div class="fcol">
      <div class="k">Контакты</div>
      <a href="tel:+77055710028" class="v">+7 705 571 00 28</a>
      <a href="https://wa.me/77055710028" class="v" target="_blank" rel="noopener">WhatsApp</a>
      <div class="v">Уральск, Западно-Казахстанская область</div>
    </div>
  </div>
  <div class="fbottom">
    <span>© 2026 «Ключ здоровья» · ИП Эврика</span>
    <span>Уральск, Казахстан</span>
  </div>
</footer>

<script>
  // header scroll state
  const header = document.getElementById('siteHeader');
  window.addEventListener('scroll', () => {
    header.classList.toggle('scrolled', window.scrollY > 40);
  });

  // mobile nav
  const burger = document.getElementById('burger');
  const nav = document.getElementById('mainNav');
  burger.addEventListener('click', () => {
    nav.classList.toggle('open');
  });
  document.querySelectorAll('.nav-link').forEach(l => {
    l.addEventListener('click', () => nav.classList.remove('open'));
  });

  // scroll reveal
  const revealEls = document.querySelectorAll('[data-reveal]');
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if(e.isIntersecting){
        e.target.classList.add('in');
        io.unobserve(e.target);
      }
    });
  }, {threshold:0.15});
  revealEls.forEach(el => io.observe(el));
</script>

</body>
</html>


