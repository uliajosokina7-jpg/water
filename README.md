
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
  .logo-badge{
    display:inline-flex;
    align-items:center;
    background:#fff;
    border-radius:10px;
    padding:6px 10px;
    box-shadow:0 4px 14px rgba(0,0,0,0.25);
  }
  .logo-badge img{
    height:34px;
    width:auto;
    display:block;
  }
  footer .logo-badge img{height:44px;}

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
      <span class="logo-badge"><img 
