<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>LogMyDrive — Every supervised mile, counted</title>
<meta name="description" content="LogMyDrive tracks learner-permit driving hours by GPS, flags night driving automatically, and tells you when your teen is ready for the road test. One-time purchase. Every driver in your family. All data stays on your phone." />

<!-- Fonts (degrade gracefully to system stack if offline) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Space+Grotesk:wght@500;600;700&display=swap" rel="stylesheet">

<style>
  :root{
    --ink:#0B1020;        /* night sky / base */
    --ink-2:#0E1426;
    --slab:#141C30;       /* panels */
    --slab-2:#1A2440;
    --line:#27324F;       /* hairlines */
    --blue:#2E7DF6;       /* primary, the app's confident blue */
    --sky:#5EC2FF;        /* light accent */
    --mint:#38D39F;       /* readiness / success */
    --amber:#FFB23E;      /* headlight glow / night */
    --paper:#EAF0FF;      /* primary text */
    --muted:#8A97B5;      /* secondary text */
    --danger:#FF6B6B;
    --r:18px;
    --display:"Space Grotesk", ui-sans-serif, system-ui, sans-serif;
    --body:"Inter", ui-sans-serif, system-ui, -apple-system, sans-serif;
    --mono:ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  }

  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    margin:0;
    font-family:var(--body);
    color:var(--paper);
    background:var(--ink);
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
  }
  a{color:inherit;text-decoration:none;}
  h1,h2,h3{font-family:var(--display);font-weight:700;line-height:1.05;margin:0;letter-spacing:-0.02em;}
  p{margin:0;}
  :focus-visible{outline:2px solid var(--sky);outline-offset:3px;border-radius:6px;}

  .wrap{max-width:1140px;margin:0 auto;padding:0 24px;}
  .eyebrow{
    font-family:var(--mono);font-size:.72rem;letter-spacing:.22em;text-transform:uppercase;
    color:var(--sky);display:inline-block;margin-bottom:14px;
  }

  /* ---------- lane-line section divider (signature structure) ---------- */
  .lanes{height:46px;width:100%;position:relative;overflow:hidden;opacity:.5;}
  .lanes::before{
    content:"";position:absolute;left:50%;top:0;bottom:0;width:6px;transform:translateX(-50%);
    background:repeating-linear-gradient(to bottom,var(--amber) 0 22px,transparent 22px 44px);
    -webkit-mask:linear-gradient(to right,transparent,#000 30%,#000 70%,transparent);
            mask:linear-gradient(to right,transparent,#000 30%,#000 70%,transparent);
    animation:lane 1.1s linear infinite;
  }
  @keyframes lane{from{background-position-y:0}to{background-position-y:44px}}

  /* ---------- nav ---------- */
  header.nav{position:sticky;top:0;z-index:50;backdrop-filter:blur(10px);
    background:rgba(11,16,32,.72);border-bottom:1px solid var(--line);}
  .nav-row{display:flex;align-items:center;justify-content:space-between;height:66px;}
  .brand{display:flex;align-items:center;gap:10px;font-family:var(--display);font-weight:700;font-size:1.15rem;letter-spacing:-.01em;}
  .brand svg{display:block;}
  .nav-links{display:flex;gap:28px;align-items:center;}
  .nav-links a{color:var(--muted);font-size:.93rem;font-weight:500;transition:color .2s;}
  .nav-links a:hover{color:var(--paper);}
  .btn{
    display:inline-flex;align-items:center;gap:8px;font-family:var(--body);font-weight:600;
    border:none;cursor:pointer;border-radius:999px;padding:11px 20px;font-size:.92rem;
    background:linear-gradient(135deg,var(--blue),#1E6FEB);color:#fff;transition:transform .15s, box-shadow .2s;
    box-shadow:0 6px 20px rgba(46,125,246,.35);
  }
  .btn:hover{transform:translateY(-1px);box-shadow:0 10px 26px rgba(46,125,246,.5);}
  .nav-cta{padding:9px 18px;}
  @media(max-width:860px){.nav-links a:not(.nav-cta){display:none;}}

  /* ---------- hero ---------- */
  .hero{position:relative;padding:84px 0 96px;overflow:hidden;}
  .hero-bg{position:absolute;inset:0;z-index:0;pointer-events:none;}
  /* headlight beam */
  .beam{position:absolute;top:-10%;left:50%;width:120%;height:120%;transform:translateX(-50%);
    background:radial-gradient(60% 50% at 50% 0%,rgba(94,194,255,.16),transparent 60%),
               radial-gradient(40% 40% at 70% 20%,rgba(255,178,62,.12),transparent 60%);}
  /* receding road lanes */
  .road{position:absolute;left:50%;bottom:0;transform:translateX(-50%);width:70%;height:100%;
    background:
      repeating-linear-gradient(to bottom, rgba(255,178,62,.20) 0 26px, transparent 26px 60px);
    -webkit-mask:radial-gradient(120% 90% at 50% 100%,#000 30%,transparent 72%);
            mask:radial-gradient(120% 90% at 50% 100%,#000 30%,transparent 72%);
    background-size:5px 60px;background-position:center;background-repeat:repeat-y;
    animation:road 1.4s linear infinite;opacity:.5;}
  @keyframes road{from{background-position-y:0}to{background-position-y:60px}}

  .hero-grid{position:relative;z-index:1;display:grid;grid-template-columns:1.05fr .95fr;gap:48px;align-items:center;}
  .hero h1{font-size:clamp(2.5rem,5.4vw,4rem);}
  .hero h1 .hl{color:var(--mint);}
  .hero p.lead{color:var(--muted);font-size:1.16rem;margin-top:20px;max-width:33ch;}
  .cta-row{display:flex;gap:14px;flex-wrap:wrap;margin-top:30px;}
  .microline{margin-top:16px;font-size:.9rem;color:var(--muted);}
  .microline b{color:var(--paper);font-weight:600;}
  .trust{display:flex;gap:10px;flex-wrap:wrap;margin-top:26px;}
  .chip{font-family:var(--mono);font-size:.72rem;letter-spacing:.06em;color:var(--sky);
    border:1px solid var(--line);background:var(--slab);border-radius:999px;padding:7px 13px;}

  /* store buttons */
  .store{display:inline-flex;align-items:center;gap:11px;background:#0a0f1d;border:1px solid #2b3550;
    border-radius:14px;padding:10px 18px;transition:transform .15s,border-color .2s;min-width:172px;}
  .store:hover{transform:translateY(-2px);border-color:var(--sky);}
  .store svg{flex:none;}
  .store .st{display:flex;flex-direction:column;line-height:1.1;}
  .store .st small{font-size:.64rem;color:var(--muted);letter-spacing:.04em;}
  .store .st span{font-family:var(--display);font-weight:600;font-size:1.02rem;}

  /* ---------- phone mockup ---------- */
  .phone{justify-self:center;width:280px;height:570px;border-radius:42px;
    background:linear-gradient(160deg,#202b46,#0d1322);padding:13px;
    box-shadow:0 40px 90px rgba(0,0,0,.55), inset 0 0 0 1px rgba(255,255,255,.05);
    position:relative;}
  .phone::after{content:"";position:absolute;top:18px;left:50%;transform:translateX(-50%);
    width:96px;height:7px;border-radius:99px;background:#05080f;}
  .screen{height:100%;border-radius:30px;background:linear-gradient(180deg,#0c1426,#0a1020);
    overflow:hidden;display:flex;flex-direction:column;}
  .scr-top{padding:26px 18px 8px;display:flex;align-items:center;gap:10px;}
  .scr-ava{width:30px;height:30px;border-radius:50%;background:linear-gradient(135deg,var(--blue),var(--sky));
    display:flex;align-items:center;justify-content:center;font-family:var(--display);font-weight:700;font-size:.85rem;color:#fff;}
  .scr-top b{font-family:var(--display);font-size:.98rem;}
  .scr-top small{color:var(--muted);font-size:.72rem;display:block;margin-top:-2px;}
  .scr-card{margin:8px 14px;border-radius:18px;padding:16px;
    background:linear-gradient(150deg,rgba(56,211,159,.22),rgba(56,211,159,.05));border:1px solid rgba(56,211,159,.25);}
  .dial-wrap{display:flex;align-items:center;gap:14px;}
  .dial{position:relative;width:84px;height:84px;flex:none;}
  .dial .val{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;}
  .dial .val b{font-family:var(--display);font-size:1.5rem;line-height:1;}
  .dial .val small{font-size:.55rem;color:var(--muted);letter-spacing:.08em;}
  .scr-card .verdict{font-family:var(--display);font-weight:600;font-size:1.05rem;color:var(--mint);}
  .scr-card .verdict small{display:block;color:var(--muted);font-weight:400;font-family:var(--body);font-size:.74rem;margin-top:2px;}
  .bars{padding:4px 16px 0;}
  .bar-row{margin:12px 0;}
  .bar-row .lab{display:flex;justify-content:space-between;font-size:.74rem;color:var(--muted);margin-bottom:5px;}
  .bar-row .lab b{color:var(--paper);font-family:var(--mono);}
  .track{height:8px;border-radius:99px;background:#1a2238;overflow:hidden;}
  .fill{height:100%;border-radius:99px;}
  .fill.blue{background:linear-gradient(90deg,var(--blue),var(--sky));}
  .fill.amber{background:linear-gradient(90deg,#b9772a,var(--amber));}
  .scr-night{margin:6px 16px;display:inline-flex;align-self:flex-start;gap:6px;align-items:center;
    background:rgba(255,178,62,.14);border:1px solid rgba(255,178,62,.3);color:var(--amber);
    border-radius:99px;padding:5px 11px;font-size:.72rem;font-weight:600;}
  .scr-start{margin:auto 16px 22px;background:linear-gradient(135deg,var(--blue),#1E6FEB);color:#fff;
    text-align:center;border-radius:14px;padding:13px;font-family:var(--display);font-weight:600;
    box-shadow:0 10px 24px rgba(46,125,246,.4);}

  /* ---------- generic section ---------- */
  section{padding:84px 0;}
  .sec-head{max-width:640px;margin-bottom:46px;}
  .sec-head h2{font-size:clamp(1.9rem,3.6vw,2.8rem);}
  .sec-head p{color:var(--muted);font-size:1.1rem;margin-top:14px;}

  /* feature grid */
  .feat-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;}
  .feat{background:var(--slab);border:1px solid var(--line);border-radius:var(--r);padding:24px;
    transition:transform .2s,border-color .2s,background .2s;}
  .feat:hover{transform:translateY(-4px);border-color:#33406a;background:var(--slab-2);}
  .feat .ico{width:46px;height:46px;border-radius:12px;display:flex;align-items:center;justify-content:center;
    background:rgba(46,125,246,.14);margin-bottom:16px;}
  .feat h3{font-size:1.12rem;margin-bottom:7px;}
  .feat p{color:var(--muted);font-size:.95rem;}
  @media(max-width:880px){.feat-grid{grid-template-columns:1fr 1fr;}}
  @media(max-width:560px){.feat-grid{grid-template-columns:1fr;}}

  /* privacy spotlight */
  .privacy{background:
      radial-gradient(80% 120% at 100% 0%,rgba(56,211,159,.12),transparent 55%),
      var(--ink-2);
    border-top:1px solid var(--line);border-bottom:1px solid var(--line);}
  .priv-grid{display:grid;grid-template-columns:1.1fr 1fr;gap:50px;align-items:center;}
  .priv-list{display:grid;gap:14px;margin-top:8px;}
  .priv-item{display:flex;gap:13px;align-items:flex-start;background:var(--slab);
    border:1px solid var(--line);border-radius:14px;padding:15px 17px;}
  .priv-item svg{flex:none;margin-top:2px;}
  .priv-item b{font-family:var(--display);font-weight:600;}
  .priv-item p{color:var(--muted);font-size:.9rem;margin-top:2px;}
  .lock-badge{display:flex;align-items:center;justify-content:center;}
  .lock-badge .ring{width:230px;height:230px;border-radius:50%;
    background:radial-gradient(circle,rgba(56,211,159,.14),transparent 70%);
    display:flex;align-items:center;justify-content:center;border:1px solid rgba(56,211,159,.25);}
  @media(max-width:820px){.priv-grid{grid-template-columns:1fr;}.lock-badge{order:-1;}}

  /* your state */
  .state-grid{display:grid;grid-template-columns:1fr 1fr;gap:50px;align-items:center;}
  .state-points{display:grid;gap:18px;margin-top:6px;}
  .state-points li{list-style:none;display:flex;gap:13px;align-items:flex-start;}
  .state-points b{font-family:var(--display);font-weight:600;}
  .state-points span{color:var(--muted);font-size:.95rem;}
  .state-num{font-family:var(--mono);color:var(--amber);font-size:.8rem;border:1px solid var(--line);
    border-radius:8px;padding:3px 7px;flex:none;}
  .states-cloud{display:flex;flex-wrap:wrap;gap:7px;align-content:flex-start;
    background:var(--slab);border:1px solid var(--line);border-radius:var(--r);padding:20px;}
  .states-cloud span{font-family:var(--mono);font-size:.74rem;color:var(--muted);
    border:1px solid var(--line);border-radius:7px;padding:5px 8px;transition:.2s;}
  .states-cloud span.on{color:var(--ink);background:var(--sky);border-color:var(--sky);font-weight:600;}
  @media(max-width:820px){.state-grid{grid-template-columns:1fr;}}

  /* pricing */
  .price-grid{display:grid;grid-template-columns:1fr 1fr;gap:22px;max-width:820px;margin:0 auto;}
  .price{background:var(--slab);border:1px solid var(--line);border-radius:22px;padding:30px;position:relative;}
  .price.pro{background:linear-gradient(160deg,var(--slab-2),#101830);border-color:#2f6fd0;
    box-shadow:0 24px 60px rgba(46,125,246,.18);}
  .price .tag{font-family:var(--mono);font-size:.72rem;letter-spacing:.16em;text-transform:uppercase;color:var(--muted);}
  .price.pro .tag{color:var(--sky);}
  .price h3{font-size:1.6rem;margin:6px 0 4px;}
  .price .sub{color:var(--muted);font-size:.92rem;margin-bottom:18px;}
  .price .once{font-family:var(--display);font-weight:700;font-size:1.4rem;color:var(--mint);margin-bottom:4px;}
  .price ul{list-style:none;padding:0;margin:18px 0 0;display:grid;gap:11px;}
  .price li{display:flex;gap:10px;align-items:flex-start;font-size:.95rem;color:var(--paper);}
  .price li svg{flex:none;margin-top:3px;}
  .price li.off{color:var(--muted);}
  .pill-badge{position:absolute;top:-13px;right:24px;background:var(--mint);color:#06281c;
    font-family:var(--display);font-weight:700;font-size:.72rem;padding:6px 13px;border-radius:99px;letter-spacing:.03em;}
  @media(max-width:680px){.price-grid{grid-template-columns:1fr;}}

  /* about */
  .about{background:var(--ink-2);border-top:1px solid var(--line);}
  .about-card{max-width:760px;margin:0 auto;background:var(--slab);border:1px solid var(--line);
    border-radius:24px;padding:42px;position:relative;}
  .about-card .eyebrow{margin-bottom:18px;}
  .about-card h2{font-size:clamp(1.7rem,3vw,2.3rem);margin-bottom:18px;}
  .about-card p{color:var(--muted);font-size:1.06rem;margin-bottom:16px;}
  .about-card p b{color:var(--paper);font-weight:600;}
  .about-sign{font-family:var(--display);color:var(--paper);font-weight:600;margin-top:24px;}
  .about-sign small{display:block;color:var(--muted);font-weight:400;font-family:var(--body);font-size:.9rem;}

  /* final cta */
  .final{text-align:center;}
  .final h2{font-size:clamp(2rem,4vw,3rem);max-width:18ch;margin:0 auto 14px;}
  .final p{color:var(--muted);font-size:1.1rem;margin-bottom:30px;}
  .final .cta-row{justify-content:center;}

  /* footer */
  footer{border-top:1px solid var(--line);padding:40px 0;color:var(--muted);font-size:.9rem;}
  .foot-row{display:flex;justify-content:space-between;align-items:center;gap:20px;flex-wrap:wrap;}
  .foot-links{display:flex;gap:22px;flex-wrap:wrap;}
  .foot-links a{color:var(--muted);transition:color .2s;}
  .foot-links a:hover{color:var(--paper);}
  .disclaimer{margin-top:22px;font-size:.78rem;color:#5b678a;max-width:720px;}

  /* reveal animation */
  .reveal{opacity:0;transform:translateY(24px);transition:opacity .7s ease,transform .7s ease;}
  .reveal.in{opacity:1;transform:none;}

  @media(prefers-reduced-motion:reduce){
    *{animation:none !important;scroll-behavior:auto;}
    .reveal{opacity:1;transform:none;transition:none;}
  }
</style>
</head>
<body>

<!-- ============ NAV ============ -->
<header class="nav">
  <div class="wrap nav-row">
    <a class="brand" href="#top" aria-label="LogMyDrive home">
      <svg width="26" height="26" viewBox="0 0 24 24" fill="none" aria-hidden="true">
        <path d="M5 11l1.5-4.5A2 2 0 0 1 8.4 5h7.2a2 2 0 0 1 1.9 1.5L19 11M5 11h14M5 11v6m14-6v6M6 17h2m8 0h2"
          stroke="#5EC2FF" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>
        <circle cx="8" cy="14.5" r="1" fill="#FFB23E"/><circle cx="16" cy="14.5" r="1" fill="#FFB23E"/>
      </svg>
      LogMyDrive
    </a>
    <nav class="nav-links" aria-label="Primary">
      <a href="#features">Features</a>
      <a href="#privacy">Privacy</a>
      <a href="#state">Your state</a>
      <a href="#pricing">Pricing</a>
      <a href="#about">About</a>
      <a class="btn nav-cta" href="#get">Get the app</a>
    </nav>
  </div>
</header>

<!-- ============ HERO ============ -->
<section class="hero" id="top">
  <div class="hero-bg" aria-hidden="true">
    <div class="beam"></div>
    <div class="road"></div>
  </div>
  <div class="wrap hero-grid">
    <div class="hero-copy">
      <span class="eyebrow">Learner-permit driving log</span>
      <h1>Every supervised mile, <span class="hl">counted.</span></h1>
      <p class="lead">LogMyDrive tracks practice hours by GPS, flags night driving on its own, and answers the one question that matters: <b style="color:var(--paper)">is your teen ready for the road test?</b></p>
      <div class="cta-row">
        <!-- Replace href with your real App Store URL -->
        <a class="store" href="https://www.apple.com/app-store/" aria-label="Download on the App Store">
          <svg width="22" height="26" viewBox="0 0 384 512" fill="#fff" aria-hidden="true"><path d="M318.7 268.7c-.2-36.7 16.4-64.4 50-84.8-18.8-26.9-47.2-41.7-84.7-44.6-35.5-2.8-74.3 20.7-88.5 20.7-15 0-49.4-19.7-76.4-19.7C63.3 141.2 4 184.8 4 273.5q0 39.3 14.4 81.2c12.8 36.7 59 126.7 107.2 125.2 25.2-.6 43-17.9 75.8-17.9 31.8 0 48.3 17.9 76.4 17.9 48.6-.7 90.4-82.5 102.6-119.3-65.2-30.7-61.7-90-61.7-91.9zm-56.6-164.2c27.3-32.4 24.8-61.9 24-72.5-24.1 1.4-52 16.4-67.9 34.9-17.5 19.8-27.8 44.3-25.6 71.9 26.1 2 49.9-11.4 69.5-34.3z"/></svg>
          <span class="st"><small>Download on the</small><span>App Store</span></span>
        </a>
        <!-- Replace href with your real Google Play URL -->
        <a class="store" href="https://play.google.com/store" aria-label="Get it on Google Play">
          <svg width="22" height="24" viewBox="0 0 512 512" aria-hidden="true">
            <path d="M48 59.5v393l219-196.5z" fill="#5EC2FF"/>
            <path d="M48 59.5 365 240l-66 59z" fill="#38D39F"/>
            <path d="M48 452.5 299 299l66 59z" fill="#FFB23E"/>
            <path d="M365 240l99 56c20 11 20 29 0 40l-99 56-66-59z" fill="#2E7DF6"/>
          </svg>
          <span class="st"><small>Get it on</small><span>Google Play</span></span>
        </a>
      </div>
      <p class="microline"><b>One-time purchase.</b> Every driver in your family. No subscription, ever.</p>
      <div class="trust">
        <span class="chip">All data on your phone</span>
        <span class="chip">No account needed</span>
        <span class="chip">Works offline</span>
      </div>
    </div>

    <!-- phone mockup -->
    <div class="phone reveal" aria-label="App dashboard preview" role="img">
      <div class="screen">
        <div class="scr-top">
          <div class="scr-ava">A</div>
          <div><b>Ava</b><small>Indiana</small></div>
        </div>
        <div class="scr-card">
          <div class="dial-wrap">
            <div class="dial">
              <svg width="84" height="84" viewBox="0 0 84 84">
                <circle cx="42" cy="42" r="36" fill="none" stroke="#1a2238" stroke-width="9"/>
                <circle id="dialArc" cx="42" cy="42" r="36" fill="none" stroke="#38D39F" stroke-width="9"
                  stroke-linecap="round" stroke-dasharray="226" stroke-dashoffset="226"
                  transform="rotate(-90 42 42)"/>
              </svg>
              <div class="val"><b>78</b><small>SCORE</small></div>
            </div>
            <div class="verdict">Almost Ready
              <small>12 hrs and a night session to go</small>
            </div>
          </div>
        </div>
        <div class="bars">
          <div class="bar-row">
            <div class="lab"><span>Total hours</span><b>38 / 50</b></div>
            <div class="track"><div class="fill blue" style="width:76%"></div></div>
          </div>
          <div class="bar-row">
            <div class="lab"><span>Night hours</span><b>4 / 10</b></div>
            <div class="track"><div class="fill amber" style="width:40%"></div></div>
          </div>
        </div>
        <div class="scr-night">🌙 Night driving detected</div>
        <div class="scr-start">Start Drive</div>
      </div>
    </div>
  </div>
</section>

<div class="lanes" aria-hidden="true"></div>

<!-- ============ FEATURES ============ -->
<section id="features">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="eyebrow">What it does</span>
      <h2>A full co-pilot for the permit year.</h2>
      <p>From the first parking-lot loop to the morning of the road test — every feature is built around one job: getting them ready, with proof.</p>
    </div>
    <div class="feat-grid">

      <div class="feat reveal">
        <div class="ico">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M12 21s-7-6.3-7-11a7 7 0 1 1 14 0c0 4.7-7 11-7 11z" stroke="#5EC2FF" stroke-width="1.7"/><circle cx="12" cy="10" r="2.4" stroke="#5EC2FF" stroke-width="1.7"/></svg>
        </div>
        <h3>Live GPS drive tracking</h3>
        <p>Tap Start Drive and the app records the route, distance, and duration on a live map — no manual stopwatch, no guesswork about how far they went.</p>
      </div>

      <div class="feat reveal">
        <div class="ico">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8z" stroke="#FFB23E" stroke-width="1.7" stroke-linejoin="round"/></svg>
        </div>
        <h3>Automatic night detection</h3>
        <p>Most families under-log night hours. LogMyDrive checks the real sunset for your location and time, flags night driving automatically, and counts it toward the night requirement.</p>
      </div>

      <div class="feat reveal">
        <div class="ico">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M3 13a9 9 0 0 1 18 0" stroke="#38D39F" stroke-width="1.7" stroke-linecap="round"/><path d="M12 13l4-3" stroke="#38D39F" stroke-width="1.7" stroke-linecap="round"/><circle cx="12" cy="13" r="1.6" fill="#38D39F"/></svg>
        </div>
        <h3>Readiness score</h3>
        <p>One clear verdict — Needs Practice, Almost Ready, or Test Ready — from hours, night time, variety, and skills. It won't say "ready" until the hard state requirements are actually met.</p>
      </div>

      <div class="feat reveal">
        <div class="ico">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M5 4h14v13l-7 3-7-3z" stroke="#5EC2FF" stroke-width="1.7" stroke-linejoin="round"/><path d="M9 11l2 2 4-4" stroke="#5EC2FF" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
        <h3>Coach mode</h3>
        <p>Turns the gaps into a short, ranked to-do list: "log 6 more night hours," "practice parallel parking," "try a rural road." Always know what to do next.</p>
      </div>

      <div class="feat reveal">
        <div class="ico">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M4 5h11a2 2 0 0 1 2 2v12H6a2 2 0 0 1-2-2z" stroke="#FFB23E" stroke-width="1.7" stroke-linejoin="round"/><path d="M8 9h6M8 12h6" stroke="#FFB23E" stroke-width="1.7" stroke-linecap="round"/></svg>
        </div>
        <h3>Skill guides with diagrams</h3>
        <p>Not sure how to coach parallel parking or a three-point turn? Each skill has a clear diagram, step-by-step instructions, and tips you can pull up roadside.</p>
      </div>

      <div class="feat reveal">
        <div class="ico">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M6 3h9l4 4v14H6z" stroke="#5EC2FF" stroke-width="1.7" stroke-linejoin="round"/><path d="M14 3v5h5M9 13h6M9 16h6" stroke="#5EC2FF" stroke-width="1.7" stroke-linecap="round"/></svg>
        </div>
        <h3>DMV-ready reports</h3>
        <p>Export a clean PDF of every logged drive, plus a log sheet formatted to match your state's official form — ready to print, sign, and hand to the examiner.</p>
      </div>

    </div>
  </div>
</section>

<div class="lanes" aria-hidden="true"></div>

<!-- ============ PRIVACY ============ -->
<section class="privacy" id="privacy">
  <div class="wrap priv-grid">
    <div class="reveal">
      <span class="eyebrow">Privacy by design</span>
      <h2 style="font-size:clamp(1.9rem,3.6vw,2.8rem)">Your family's driving stays on your phone.</h2>
      <p style="color:var(--muted);font-size:1.1rem;margin-top:14px">No app should quietly track where your teenager drives. LogMyDrive doesn't — there's no server for it to send anything to.</p>
      <div class="priv-list">
        <div class="priv-item">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none"><path d="M6 11V8a6 6 0 0 1 12 0v3" stroke="#38D39F" stroke-width="1.7"/><rect x="4" y="11" width="16" height="9" rx="2" stroke="#38D39F" stroke-width="1.7"/></svg>
          <div><b>No account, no login.</b><p>Open the app and start — there's nothing to sign up for and no password to forget.</p></div>
        </div>
        <div class="priv-item">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none"><path d="M4 16a4 4 0 0 1 1-7.5A5.5 5.5 0 0 1 16 7a4.5 4.5 0 0 1 1 8.9" stroke="#38D39F" stroke-width="1.7" stroke-linecap="round"/><path d="M12 13v6m0-6-2 2m2-2 2 2" stroke="#FF6B6B" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"/></svg>
          <div><b>No cloud, no servers.</b><p>Drives, routes, and notes are stored locally in the app — they never get uploaded.</p></div>
        </div>
        <div class="priv-item">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none"><circle cx="12" cy="12" r="9" stroke="#38D39F" stroke-width="1.7"/><path d="M7 17 17 7M9 8h.01M15 16h.01" stroke="#38D39F" stroke-width="1.7" stroke-linecap="round"/></svg>
          <div><b>Nothing sold, no ads.</b><p>You bought the app. You aren't the product — there's no data to sell and nobody to sell it to.</p></div>
        </div>
        <div class="priv-item">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none"><path d="M12 3v12m0-12 4 4m-4-4-4 4" stroke="#38D39F" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"/><path d="M5 15v4h14v-4" stroke="#38D39F" stroke-width="1.7" stroke-linecap="round"/></svg>
          <div><b>You control sharing.</b><p>A report only leaves your phone when you export the PDF — to print it or send it yourself.</p></div>
        </div>
      </div>
    </div>
    <div class="lock-badge reveal" aria-hidden="true">
      <div class="ring">
        <svg width="120" height="120" viewBox="0 0 24 24" fill="none">
          <rect x="4" y="10" width="16" height="11" rx="2.4" stroke="#38D39F" stroke-width="1.3"/>
          <path d="M7.5 10V7.5a4.5 4.5 0 0 1 9 0V10" stroke="#38D39F" stroke-width="1.3"/>
          <circle cx="12" cy="15" r="1.6" fill="#38D39F"/>
          <path d="M12 16.4V18" stroke="#38D39F" stroke-width="1.3" stroke-linecap="round"/>
        </svg>
      </div>
    </div>
  </div>
</section>

<!-- ============ YOUR STATE ============ -->
<section id="state">
  <div class="wrap state-grid">
    <div class="states-cloud reveal" id="statesCloud" aria-hidden="true"></div>
    <div class="reveal">
      <span class="eyebrow">Built for where you live</span>
      <h2 style="font-size:clamp(1.9rem,3.6vw,2.8rem)">Your state's rules, not a generic checklist.</h2>
      <p style="color:var(--muted);font-size:1.1rem;margin-top:14px">Requirements vary wildly — different total hours, night hours, and permit-holding periods. Set your state once and everything tunes to it.</p>
      <ul class="state-points">
        <li><span class="state-num">50+DC</span><div><b>Every state covered.</b><br><span>Total and night-hour targets plus the minimum permit-holding period for all 50 states and Washington, D.C.</span></div></li>
        <li><span class="state-num">LOG</span><div><b>Your state's log format.</b><br><span>Generate a supervised-driving log laid out to match the official form your DMV expects.</span></div></li>
        <li><span class="state-num">LINK</span><div><b>Straight to the source.</b><br><span>One tap to your state's official DMV site and its new-driver and teen-licensing pages.</span></div></li>
      </ul>
    </div>
  </div>
</section>

<div class="lanes" aria-hidden="true"></div>

<!-- ============ PRICING ============ -->
<section id="pricing">
  <div class="wrap">
    <div class="sec-head reveal" style="text-align:center;margin-left:auto;margin-right:auto;">
      <span class="eyebrow">Simple pricing</span>
      <h2>Pay once. Track the whole family.</h2>
      <p style="margin-left:auto;margin-right:auto;">No subscription, no renewals. Unlock it once and add a profile for every driver under your roof.</p>
    </div>
    <div class="price-grid">
      <div class="price reveal">
        <span class="tag">Free</span>
        <h3>Get started</h3>
        <p class="sub">Everything you need to start logging one driver.</p>
        <ul>
          <li><svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M5 12l4 4 10-10" stroke="#38D39F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>One driver profile</li>
          <li><svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M5 12l4 4 10-10" stroke="#38D39F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>GPS drive tracking &amp; readiness score</li>
          <li><svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M5 12l4 4 10-10" stroke="#38D39F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>Skill checklist and coach tips</li>
        </ul>
      </div>

      <div class="price pro reveal">
        <span class="pill-badge">Best value</span>
        <span class="tag">Pro · one-time</span>
        <h3>Unlock everything</h3>
        <p class="once">One-time purchase</p>
        <p class="sub">Pay once, own it forever — no subscription.</p>
        <ul>
          <li><svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M5 12l4 4 10-10" stroke="#5EC2FF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg><b style="font-family:var(--display)">Unlimited drivers — every kid you have</b></li>
          <li><svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M5 12l4 4 10-10" stroke="#5EC2FF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>PDF reports &amp; your state's official log sheet</li>
          <li><svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M5 12l4 4 10-10" stroke="#5EC2FF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>Full skill guides with diagrams</li>
          <li><svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M5 12l4 4 10-10" stroke="#5EC2FF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>Unlimited drive history &amp; light/dark themes</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- ============ ABOUT ============ -->
<section class="about" id="about">
  <div class="wrap">
    <div class="about-card reveal">
      <span class="eyebrow">Our story</span>
      <h2>Born out of a glovebox full of guesswork.</h2>
      <p>When our <b>third kid</b> got a learner's permit, we hit the same wall we had with the first two — except this time we admitted it was a real problem.</p>
      <p>The state wanted fifty logged hours, ten of them at night. What we actually had was a crumpled paper sheet in the glovebox, a few half-remembered drives, and a teenager who <b>genuinely could not tell us</b> how many hours they'd done. "A lot?" Nobody was writing it down in the moment, the night hours never got counted, and when the road test got close we were honestly guessing whether they were ready.</p>
      <p>So we built the tool we kept wishing existed: <b>start a drive, put the phone down, and let it record the route, the time, and whether it was night — automatically.</b> No paper. No arguments about what counted. Just an honest picture of where each kid stood.</p>
      <p>It worked for our family, so we cleaned it up to share with yours. <b>LogMyDrive was born out of necessity</b> — and a little bit out of stubbornness.</p>
      <div class="about-sign">— The parents behind LogMyDrive
        <small>Three permits down. We've been exactly where you are.</small>
      </div>
    </div>
  </div>
</section>

<div class="lanes" aria-hidden="true"></div>

<!-- ============ FINAL CTA ============ -->
<section class="final" id="get">
  <div class="wrap">
    <h2 class="reveal">Start counting the miles that count.</h2>
    <p class="reveal">Download LogMyDrive and turn the permit year into a clear, honest path to the road test.</p>
    <div class="cta-row reveal">
      <!-- Replace href with your real App Store URL -->
      <a class="store" href="https://www.apple.com/app-store/" aria-label="Download on the App Store">
        <svg width="22" height="26" viewBox="0 0 384 512" fill="#fff" aria-hidden="true"><path d="M318.7 268.7c-.2-36.7 16.4-64.4 50-84.8-18.8-26.9-47.2-41.7-84.7-44.6-35.5-2.8-74.3 20.7-88.5 20.7-15 0-49.4-19.7-76.4-19.7C63.3 141.2 4 184.8 4 273.5q0 39.3 14.4 81.2c12.8 36.7 59 126.7 107.2 125.2 25.2-.6 43-17.9 75.8-17.9 31.8 0 48.3 17.9 76.4 17.9 48.6-.7 90.4-82.5 102.6-119.3-65.2-30.7-61.7-90-61.7-91.9zm-56.6-164.2c27.3-32.4 24.8-61.9 24-72.5-24.1 1.4-52 16.4-67.9 34.9-17.5 19.8-27.8 44.3-25.6 71.9 26.1 2 49.9-11.4 69.5-34.3z"/></svg>
        <span class="st"><small>Download on the</small><span>App Store</span></span>
      </a>
      <!-- Replace href with your real Google Play URL -->
      <a class="store" href="https://play.google.com/store" aria-label="Get it on Google Play">
        <svg width="22" height="24" viewBox="0 0 512 512" aria-hidden="true">
          <path d="M48 59.5v393l219-196.5z" fill="#5EC2FF"/>
          <path d="M48 59.5 365 240l-66 59z" fill="#38D39F"/>
          <path d="M48 452.5 299 299l66 59z" fill="#FFB23E"/>
          <path d="M365 240l99 56c20 11 20 29 0 40l-99 56-66-59z" fill="#2E7DF6"/>
        </svg>
        <span class="st"><small>Get it on</small><span>Google Play</span></span>
      </a>
    </div>
  </div>
</section>

<!-- ============ FOOTER ============ -->
<footer>
  <div class="wrap">
    <div class="foot-row">
      <a class="brand" href="#top" style="font-size:1.05rem">
        <svg width="22" height="22" viewBox="0 0 24 24" fill="none" aria-hidden="true">
          <path d="M5 11l1.5-4.5A2 2 0 0 1 8.4 5h7.2a2 2 0 0 1 1.9 1.5L19 11M5 11h14M5 11v6m14-6v6M6 17h2m8 0h2"
            stroke="#5EC2FF" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>
          <circle cx="8" cy="14.5" r="1" fill="#FFB23E"/><circle cx="16" cy="14.5" r="1" fill="#FFB23E"/>
        </svg>
        LogMyDrive
      </a>
      <div class="foot-links">
        <a href="#features">Features</a>
        <a href="#privacy">Privacy</a>
        <a href="#state">Your state</a>
        <a href="#pricing">Pricing</a>
        <a href="#about">About</a>
      </div>
    </div>
    <p class="disclaimer">Hour requirements, forms, and DMV links in the app are a researched starting point to help you prepare — always verify the current rules with your state's licensing agency. The readiness score is a practice aid, not a guarantee of passing a road test.</p>
    <p style="margin-top:14px;">© <span id="yr"></span> LogMyDrive · Made by parents who'd been there.</p>
  </div>
</footer>

<script>
  // year
  document.getElementById('yr').textContent = new Date().getFullYear();

  // animate readiness dial when hero loads
  window.addEventListener('load', function(){
    var arc = document.getElementById('dialArc');
    if(arc && !window.matchMedia('(prefers-reduced-motion: reduce)').matches){
      // 78% of the 226 dash length
      setTimeout(function(){ arc.style.transition='stroke-dashoffset 1.4s ease'; arc.style.strokeDashoffset = 226 - (226*0.78); }, 250);
    } else if(arc){
      arc.style.strokeDashoffset = 226 - (226*0.78);
    }
  });

  // state cloud
  (function(){
    var states="AL AK AZ AR CA CO CT DE DC FL GA HI ID IL IN IA KS KY LA ME MD MA MI MN MS MO MT NE NV NH NJ NM NY NC ND OH OK OR PA RI SC SD TN TX UT VT VA WA WV WI WY".split(" ");
    var cloud=document.getElementById('statesCloud');
    if(!cloud) return;
    states.forEach(function(s){
      var el=document.createElement('span'); el.textContent=s; cloud.appendChild(el);
    });
    // gently highlight a rotating few
    var spans=cloud.querySelectorAll('span');
    if(window.matchMedia('(prefers-reduced-motion: reduce)').matches){ spans[14].classList.add('on'); return; }
    var i=0;
    setInterval(function(){
      spans.forEach(function(x){x.classList.remove('on');});
      for(var k=0;k<3;k++){ spans[(i+k*17)%spans.length].classList.add('on'); }
      i=(i+1)%spans.length;
    },900);
  })();

  // scroll reveal
  (function(){
    var els=document.querySelectorAll('.reveal');
    if(!('IntersectionObserver' in window)){ els.forEach(function(e){e.classList.add('in');}); return; }
    var io=new IntersectionObserver(function(entries){
      entries.forEach(function(en){ if(en.isIntersecting){ en.target.classList.add('in'); io.unobserve(en.target);} });
    },{threshold:.16});
    els.forEach(function(e){io.observe(e);});
  })();
</script>
</body>
</html>
