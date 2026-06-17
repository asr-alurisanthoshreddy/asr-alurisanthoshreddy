<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Aluri Santhosh Reddy — AI & ML Engineer, Salesforce Agentforce Specialist, Deep Learning Researcher. Based in Hyderabad, India. Open to full-time roles."/>
  <meta property="og:title" content="Aluri Santhosh Reddy · AI/ML Engineer | Salesforce Developer"/>
  <meta property="og:description" content="92.8% ML accuracy · Salesforce Agentforce Specialist · Trailhead Ranger · Open to Work"/>
  <title>Aluri Santhosh Reddy · AI/ML Engineer | Salesforce Developer</title>

  <link rel="preconnect" href="https://fonts.googleapis.com"/>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600;700&display=swap" rel="stylesheet"/>

  <style>
    /* ════════════════════════════════════════
       TOKENS & RESET
    ════════════════════════════════════════ */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --gh-bg:        #0d1117;
      --gh-surface:   #161b22;
      --gh-card:      #21262d;
      --gh-hover:     #2d333b;
      --gh-border:    #30363d;
      --gh-muted-bd:  #21262d;

      --text-1: #e6edf3;
      --text-2: #8b949e;
      --text-3: #6e7681;

      --sf:          #00A1E0;   /* Salesforce blue  */
      --sf-glow:     rgba(0,161,224,.14);
      --ai:          #9D4EDD;   /* AI/ML purple     */
      --ai-soft:     #c084fc;
      --ai-glow:     rgba(157,78,221,.15);
      --ok:          #3fb950;   /* green / success  */
      --ok-glow:     rgba(63,185,80,.14);
      --warn:        #e3b341;
      --warn-glow:   rgba(227,179,65,.12);
      --danger:      #ff7b72;

      --mono: 'JetBrains Mono', 'Cascadia Code', monospace;
      --sans: 'Inter', system-ui, -apple-system, sans-serif;

      --r-sm:   6px;
      --r:     10px;
      --r-lg:  16px;
      --r-xl:  22px;

      --shadow: 0 4px 24px rgba(0,0,0,.45);
      --glow-ai: 0 0 28px rgba(157,78,221,.22);
      --glow-sf: 0 0 28px rgba(0,161,224,.18);
    }

    html { scroll-behavior: smooth; font-size: 16px; }

    body {
      background: var(--gh-bg);
      color: var(--text-1);
      font-family: var(--sans);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }

    a { color: inherit; text-decoration: none; }
    img { max-width: 100%; display: block; }

    /* ════════════════════════════════════════
       LAYOUT
    ════════════════════════════════════════ */
    .wrap {
      max-width: 880px;
      margin: 0 auto;
      padding: 0 20px;
    }

    /* ════════════════════════════════════════
       KEYFRAMES
    ════════════════════════════════════════ */
    @keyframes blink      { 0%,100%{opacity:1} 50%{opacity:0} }
    @keyframes fadeUp     { from{opacity:0;transform:translateY(18px)} to{opacity:1;transform:none} }
    @keyframes pulse-ring {
      0%,100%{ box-shadow:0 0 0 0 var(--ok-glow); }
      60%    { box-shadow:0 0 0 7px transparent; }
    }
    @keyframes gradMove   {
      0%  { background-position:0% 50%; }
      50% { background-position:100% 50%; }
      100%{ background-position:0% 50%; }
    }
    @keyframes float      {
      0%,100%{ transform:translateY(0); }
      50%    { transform:translateY(-6px); }
    }

    /* ════════════════════════════════════════
       SCROLL REVEAL
    ════════════════════════════════════════ */
    .reveal { opacity:0; transform:translateY(20px); transition:opacity .55s ease,transform .55s ease; }
    .reveal.in { opacity:1; transform:none; }
    .reveal.d1 { transition-delay:.08s; }
    .reveal.d2 { transition-delay:.16s; }
    .reveal.d3 { transition-delay:.24s; }

    /* ════════════════════════════════════════
       SECTION CARD
    ════════════════════════════════════════ */
    .panel {
      background: var(--gh-surface);
      border: 1px solid var(--gh-border);
      border-radius: var(--r-xl);
      padding: 28px;
      margin-bottom: 14px;
    }

    .section-head {
      display: flex;
      align-items: center;
      gap: 10px;
      font-size: .92rem;
      font-weight: 700;
      color: var(--text-1);
      margin-bottom: 22px;
      padding-bottom: 14px;
      border-bottom: 1px solid var(--gh-border);
      letter-spacing: .01em;
    }
    .section-head .bar {
      width: 3px; height: 20px;
      background: linear-gradient(180deg, var(--ai) 0%, var(--sf) 100%);
      border-radius: 2px;
      flex-shrink: 0;
    }

    /* ════════════════════════════════════════
       HEADER
    ════════════════════════════════════════ */
    .header { padding: 60px 0 44px; }

    .prompt {
      font-family: var(--mono);
      font-size: .78rem;
      color: var(--ok);
      margin-bottom: 6px;
      letter-spacing: .02em;
    }

    .hero-name {
      font-size: clamp(2rem, 5.5vw, 3.1rem);
      font-weight: 800;
      line-height: 1.1;
      margin-bottom: 10px;
      letter-spacing: -.02em;
    }
    .hero-name .grad {
      background: linear-gradient(135deg, var(--ai-soft) 0%, var(--sf) 60%, var(--ok) 100%);
      background-size: 200% 200%;
      animation: gradMove 5s ease infinite;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero-role {
      font-family: var(--mono);
      font-size: .95rem;
      color: var(--text-2);
      min-height: 1.55rem;
      margin-bottom: 26px;
    }
    .cursor-dot {
      display: inline-block;
      width: 2px; height: 1em;
      background: var(--ai);
      vertical-align: text-bottom;
      margin-left: 2px;
      animation: blink 1s step-end infinite;
    }

    /* ── Tags ── */
    .tag-row { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 34px; }

    .tag {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      font-family: var(--mono);
      font-size: .72rem;
      font-weight: 600;
      padding: 5px 12px;
      border-radius: 20px;
      border: 1px solid;
      cursor: default;
      user-select: none;
    }
    .t-sf   { color:var(--sf);   border-color:rgba(0,161,224,.45);  background:var(--sf-glow);  }
    .t-ai   { color:var(--ai-soft); border-color:rgba(192,132,252,.4); background:var(--ai-glow); }
    .t-ok   { color:var(--ok);   border-color:rgba(63,185,80,.45);  background:var(--ok-glow);
               animation: pulse-ring 2.6s ease infinite; }
    .t-warn { color:var(--warn); border-color:rgba(227,179,65,.45); background:var(--warn-glow); }

    /* ── Stat counters ── */
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 10px;
    }
    .stat-box {
      background: var(--gh-card);
      border: 1px solid var(--gh-border);
      border-radius: var(--r);
      padding: 22px 12px;
      text-align: center;
      transition: border-color .2s, box-shadow .2s, transform .2s;
      cursor: default;
    }
    .stat-box:hover {
      border-color: var(--ai);
      box-shadow: var(--glow-ai);
      transform: translateY(-2px);
    }
    .stat-num {
      font-family: var(--mono);
      font-size: 1.9rem;
      font-weight: 700;
      color: var(--ai-soft);
      line-height: 1;
      margin-bottom: 6px;
    }
    .stat-lbl {
      font-size: .7rem;
      color: var(--text-3);
      text-transform: uppercase;
      letter-spacing: .07em;
    }

    /* ════════════════════════════════════════
       ABOUT GRID
    ════════════════════════════════════════ */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      margin-bottom: 14px;
    }
    .about-cell {
      background: var(--gh-card);
      border: 1px solid var(--gh-border);
      border-radius: var(--r);
      padding: 15px 17px;
      transition: border-color .2s;
    }
    .about-cell:hover { border-color: var(--gh-hover); }
    .about-lbl {
      font-family: var(--mono);
      font-size: .66rem;
      font-weight: 700;
      color: var(--text-3);
      text-transform: uppercase;
      letter-spacing: .09em;
      margin-bottom: 5px;
    }
    .about-val { font-size: .87rem; color: var(--text-1); line-height: 1.5; }
    .about-val strong { color: var(--ai-soft); font-weight: 600; }
    .about-val .sf  { color: var(--sf); }

    .quote {
      border-left: 3px solid var(--ai);
      padding: 14px 18px;
      background: var(--ai-glow);
      border-radius: 0 var(--r) var(--r) 0;
    }
    .quote p {
      font-style: italic;
      font-size: .9rem;
      color: var(--text-2);
      line-height: 1.7;
    }

    /* ════════════════════════════════════════
       REPO CARDS
    ════════════════════════════════════════ */
    .repos-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 12px;
    }
    .repo-card {
      background: var(--gh-card);
      border: 1px solid var(--gh-border);
      border-radius: var(--r-lg);
      padding: 18px;
      display: flex;
      flex-direction: column;
      gap: 10px;
      position: relative;
      transition: border-color .2s, box-shadow .2s, transform .22s;
      text-decoration: none;
    }
    .repo-card:hover {
      border-color: var(--ai);
      box-shadow: var(--glow-ai);
      transform: translateY(-3px);
    }
    .pinned-badge {
      position: absolute; top: 12px; right: 12px;
      font-family: var(--mono);
      font-size: .62rem;
      color: var(--text-3);
      background: var(--gh-surface);
      border: 1px solid var(--gh-border);
      border-radius: 10px;
      padding: 2px 8px;
    }
    .repo-top { display:flex; align-items:flex-start; gap:10px; }
    .repo-ico {
      width:36px; height:36px;
      border-radius:9px;
      display:flex; align-items:center; justify-content:center;
      font-size:1.05rem;
      flex-shrink:0;
    }
    .ri-sf  { background:var(--sf-glow);   border:1px solid rgba(0,161,224,.3); }
    .ri-ai  { background:var(--ai-glow);   border:1px solid rgba(157,78,221,.3); }
    .ri-ok  { background:var(--ok-glow);   border:1px solid rgba(63,185,80,.3); }
    .ri-warn{ background:var(--warn-glow); border:1px solid rgba(227,179,65,.3); }

    .repo-name {
      font-family: var(--mono);
      font-size: .87rem;
      font-weight: 700;
      color: var(--sf);
      display: flex;
      align-items: center;
      gap: 6px;
      flex-wrap: wrap;
    }
    .repo-badge {
      font-size: .6rem;
      padding: 2px 7px;
      border-radius: 10px;
      border: 1px solid;
      font-weight: 600;
    }
    .rb-sf  { color:var(--sf);      border-color:rgba(0,161,224,.4);  background:var(--sf-glow); }
    .rb-ai  { color:var(--ai-soft); border-color:rgba(192,132,252,.4); background:var(--ai-glow); }
    .rb-ok  { color:var(--ok);      border-color:rgba(63,185,80,.4);   background:var(--ok-glow); }
    .rb-warn{ color:var(--warn);    border-color:rgba(227,179,65,.4);  background:var(--warn-glow); }

    .repo-desc {
      font-size: .81rem;
      color: var(--text-2);
      line-height: 1.55;
      flex: 1;
    }
    .repo-meta {
      display: flex;
      align-items: center;
      gap: 14px;
      font-family: var(--mono);
      font-size: .72rem;
      color: var(--text-3);
    }
    .lang-dot {
      display: inline-block;
      width: 10px; height: 10px;
      border-radius: 50%;
      margin-right: 4px;
      vertical-align: middle;
    }

    /* ════════════════════════════════════════
       TECH STACK
    ════════════════════════════════════════ */
    .tech-group  { margin-bottom: 18px; }
    .tech-group:last-child { margin-bottom: 0; }
    .tech-cat {
      font-family: var(--mono);
      font-size: .67rem;
      font-weight: 700;
      color: var(--text-3);
      text-transform: uppercase;
      letter-spacing: .1em;
      margin-bottom: 10px;
    }
    .pills { display:flex; flex-wrap:wrap; gap:8px; }

    .pill {
      font-family: var(--mono);
      font-size: .73rem;
      font-weight: 500;
      padding: 5px 11px;
      border-radius: 20px;
      border: 1px solid;
      transition: transform .15s, filter .15s;
      cursor: default;
      user-select: none;
    }
    .pill:hover { transform:translateY(-2px); filter:brightness(1.25); }
    .p-sf  { color:var(--sf);      border-color:rgba(0,161,224,.4);  background:var(--sf-glow); }
    .p-ai  { color:var(--ai-soft); border-color:rgba(192,132,252,.4); background:var(--ai-glow); }
    .p-dt  { color:var(--warn);    border-color:rgba(227,179,65,.4);  background:var(--warn-glow); }

    /* ════════════════════════════════════════
       CONTRIBUTION GRAPH
    ════════════════════════════════════════ */
    .graph-wrap {
      background: var(--gh-card);
      border: 1px solid var(--gh-border);
      border-radius: var(--r);
      padding: 20px;
    }
    .graph-wrap img { width:100%; border-radius:4px; }
    .graph-meta { font-family:var(--mono); font-size:.73rem; color:var(--text-3); margin-top:10px; }

    /* ════════════════════════════════════════
       EXPERIENCE
    ════════════════════════════════════════ */
    .exp-item {
      display: flex;
      gap: 16px;
      padding: 16px 0;
      border-bottom: 1px solid var(--gh-border);
    }
    .exp-item:last-child { border-bottom: none; padding-bottom: 0; }
    .exp-dot {
      width: 10px; height: 10px;
      border-radius: 50%;
      background: var(--sf);
      margin-top: 6px;
      flex-shrink: 0;
      box-shadow: 0 0 8px var(--sf);
    }
    .exp-role { font-size:.9rem; font-weight:700; color:var(--text-1); }
    .exp-where { font-family:var(--mono); font-size:.75rem; color:var(--sf); margin: 2px 0; }
    .exp-when  { font-family:var(--mono); font-size:.72rem; color:var(--text-3); margin-bottom:8px; }
    .exp-desc  { font-size:.83rem; color:var(--text-2); line-height:1.55; }

    /* ════════════════════════════════════════
       CERTIFICATIONS
    ════════════════════════════════════════ */
    .certs-row {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      margin-bottom: 10px;
    }
    .cert-card {
      background: var(--gh-card);
      border: 1px solid var(--gh-border);
      border-radius: var(--r);
      padding: 16px;
      display: flex;
      align-items: flex-start;
      gap: 12px;
      transition: border-color .2s, transform .2s;
    }
    .cert-card:hover { border-color: var(--sf); transform: translateY(-2px); }
    .cert-ico {
      width: 38px; height: 38px;
      border-radius: 9px;
      background: var(--gh-surface);
      border: 1px solid var(--gh-border);
      display: flex; align-items: center; justify-content: center;
      font-size: 1rem;
      flex-shrink: 0;
    }
    .cert-name { font-size:.82rem; font-weight:600; color:var(--text-1); line-height:1.3; margin-bottom:4px; }
    .cert-by   { font-family:var(--mono); font-size:.7rem; color:var(--text-3); }

    .cert-featured {
      background: linear-gradient(135deg,rgba(0,161,224,.1) 0%,rgba(0,161,224,.04) 100%);
      border: 1px solid rgba(0,161,224,.35);
      border-radius: var(--r);
      padding: 18px 20px;
      display: flex;
      align-items: center;
      gap: 16px;
      transition: box-shadow .2s;
    }
    .cert-featured:hover { box-shadow: var(--glow-sf); }
    .cf-ico  { font-size: 2.2rem; line-height:1; animation: float 3.5s ease-in-out infinite; }
    .cf-name { font-family:var(--mono); font-weight:700; font-size:.95rem; color:var(--sf); margin-bottom:4px; }
    .cf-det  { font-size:.8rem; color:var(--text-2); line-height:1.5; }

    /* ════════════════════════════════════════
       CONNECT
    ════════════════════════════════════════ */
    .connect-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
    }
    .connect-card {
      background: var(--gh-card);
      border: 1px solid var(--gh-border);
      border-radius: var(--r);
      padding: 14px 16px;
      display: flex;
      align-items: center;
      gap: 12px;
      text-decoration: none;
      transition: border-color .2s, background .2s, transform .2s;
      cursor: pointer;
    }
    .connect-card:hover {
      border-color: var(--ai);
      background: var(--gh-hover);
      transform: translateY(-2px);
    }
    .cc-ico {
      width: 36px; height: 36px;
      border-radius: 9px;
      display: flex; align-items: center; justify-content: center;
      font-size: 1rem;
      flex-shrink: 0;
    }
    .cc-label { font-size:.8rem; font-weight:600; color:var(--text-1); margin-bottom:2px; }
    .cc-val   { font-family:var(--mono); font-size:.7rem; color:var(--text-3); word-break:break-all; }

    /* ════════════════════════════════════════
       FOOTER
    ════════════════════════════════════════ */
    .footer {
      padding: 28px 0 40px;
      text-align: center;
      border-top: 1px solid var(--gh-border);
      margin-top: 4px;
    }
    .footer-views {
      display: inline-flex; align-items: center; gap: 8px;
      font-family: var(--mono); font-size: .8rem; color: var(--text-3);
    }
    .footer-views img { height: 20px; border-radius: 4px; }
    .footer-note { font-size: .78rem; color: var(--text-3); margin-top: 8px; }
    .footer-note a { color: var(--ai); }
    .footer-note a:hover { text-decoration: underline; }

    /* ════════════════════════════════════════
       RESPONSIVE
    ════════════════════════════════════════ */
    @media (max-width: 680px) {
      .stats-grid    { grid-template-columns: repeat(2, 1fr); }
      .about-grid    { grid-template-columns: 1fr; }
      .repos-grid    { grid-template-columns: 1fr; }
      .certs-row     { grid-template-columns: 1fr 1fr; }
      .connect-grid  { grid-template-columns: 1fr 1fr; }
      .header        { padding: 40px 0 30px; }
    }
    @media (max-width: 440px) {
      .certs-row    { grid-template-columns: 1fr; }
      .connect-grid { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

<div class="wrap">

  <!-- ╔══════════════════════════════╗
       ║          HEADER              ║
       ╚══════════════════════════════╝ -->
  <header class="header reveal">
    <p class="prompt">// 👋 portfolio.ts · loaded successfully</p>
    <h1 class="hero-name">Hi, I'm <span class="grad">Aluri Santhosh Reddy</span></h1>
    <p class="hero-role" id="role-line"><span id="role-txt"></span><span class="cursor-dot"></span></p>

    <div class="tag-row">
      <span class="tag t-sf">⚡ Salesforce Agentforce Specialist</span>
      <span class="tag t-ai">🧠 AI &amp; ML Engineer</span>
      <span class="tag t-warn">🎓 B.Tech AI &amp; ML · 2026</span>
      <span class="tag t-ai">🔬 Deep Learning Researcher</span>
      <span class="tag t-ok">🟢 Open to Work</span>
    </div>

    <div class="stats-grid">
      <div class="stat-box">
        <div class="stat-num" data-to="3"   data-sfx="">0</div>
        <div class="stat-lbl">projects</div>
      </div>
      <div class="stat-box">
        <div class="stat-num" data-to="100" data-sfx="+">0</div>
        <div class="stat-lbl">badges</div>
      </div>
      <div class="stat-box">
        <div class="stat-num" data-to="92.8" data-sfx="%" data-dec="1">0</div>
        <div class="stat-lbl">model acc.</div>
      </div>
      <div class="stat-box">
        <div class="stat-num" data-to="4"   data-sfx="">0</div>
        <div class="stat-lbl">certs</div>
      </div>
    </div>
  </header>


  <!-- ╔══════════════════════════════╗
       ║          ABOUT ME            ║
       ╚══════════════════════════════╝ -->
  <section class="panel reveal d1">
    <div class="section-head"><div class="bar"></div>👤 About me</div>

    <div class="about-grid">
      <div class="about-cell">
        <div class="about-lbl">Currently Building</div>
        <div class="about-val">Tourism Management System on <span class="sf">Salesforce</span> — full lifecycle automation with Apex, Flows &amp; REST API integrations</div>
      </div>
      <div class="about-cell">
        <div class="about-lbl">Education</div>
        <div class="about-val">B.Tech AI &amp; ML · CMR College, Hyderabad · Graduating <strong>May 2026</strong> · CGPA 7.03</div>
      </div>
      <div class="about-cell">
        <div class="about-lbl">Research</div>
        <div class="about-val">HSSAN — multi-modal DL for spectral-spatial flower classification (<strong>92.8% acc.</strong>, F1 91.8%, +6–8pp over CNN baseline)</div>
      </div>
      <div class="about-cell">
        <div class="about-lbl">Ask Me About</div>
        <div class="about-val"><span class="sf">Apex, LWC, Agentforce, Einstein AI, REST APIs</span> · PyTorch, XGBoost, Hyperspectral Imaging</div>
      </div>
      <div class="about-cell">
        <div class="about-lbl">Location</div>
        <div class="about-val">📍 Hyderabad, Telangana, India · Open to Remote / Relocate</div>
      </div>
      <div class="about-cell">
        <div class="about-lbl">Fun Fact</div>
        <div class="about-val">Built a football fixture generator in C++ just to practice algorithms 🏟️ &nbsp;·&nbsp; Debug Apex &amp; PyTorch loss functions in the same afternoon 🤯</div>
      </div>
    </div>

    <div class="quote" style="margin-top:14px;">
      <p>"I build things that are measurably better — 92.8% accuracy beats baselines, ~60% manual workload eliminated, zero seat overbookings."</p>
    </div>
  </section>


  <!-- ╔══════════════════════════════╗
       ║       PINNED REPOS           ║
       ╚══════════════════════════════╝ -->
  <section class="panel reveal d1">
    <div class="section-head"><div class="bar"></div>📁 Pinned repositories</div>

    <div class="repos-grid">

      <a class="repo-card" href="https://github.com/asr-alurisanthoshreddy/tourism-mgmt-sf" target="_blank" rel="noopener">
        <span class="pinned-badge">Pinned</span>
        <div class="repo-top">
          <div class="repo-ico ri-sf">🗺️</div>
          <div>
            <div class="repo-name">
              tourism-mgmt-sf
              <span class="repo-badge rb-sf">Salesforce</span>
            </div>
          </div>
        </div>
        <p class="repo-desc">Full-stack Salesforce platform automating travel agency operations — seat reservation, payment reminders, hotel/transport API integrations. Zero manual intervention.</p>
        <div class="repo-meta">
          <span><span class="lang-dot" style="background:#f1913c"></span>Apex</span>
          <span>⭐ 4</span>
          <span>🍴 2</span>
        </div>
      </a>

      <a class="repo-card" href="https://github.com/asr-alurisanthoshreddy/hssan-flower-classifier" target="_blank" rel="noopener">
        <span class="pinned-badge">Pinned</span>
        <div class="repo-top">
          <div class="repo-ico ri-ai">🌸</div>
          <div>
            <div class="repo-name">
              hssan-flower-classifier
              <span class="repo-badge rb-ai">Deep Learning</span>
            </div>
          </div>
        </div>
        <p class="repo-desc">Hybrid Spectral-Spatial Attention Network fusing RGB + multispectral + hyperspectral inputs. 92.8% accuracy, F1 91.8%, +6–8pp over CNN baseline.</p>
        <div class="repo-meta">
          <span><span class="lang-dot" style="background:#3572A5"></span>Python</span>
          <span>⭐ 11</span>
          <span>🍴 3</span>
        </div>
      </a>

      <a class="repo-card" href="https://github.com/asr-alurisanthoshreddy/cervical-cancer-risk-xgb" target="_blank" rel="noopener">
        <span class="pinned-badge">Pinned</span>
        <div class="repo-top">
          <div class="repo-ico ri-ok">🩺</div>
          <div>
            <div class="repo-name">
              cervical-cancer-risk-xgb
              <span class="repo-badge rb-ok">Medical AI</span>
            </div>
          </div>
        </div>
        <p class="repo-desc">XGBoost binary risk classifier on clinical data. 95.35% accuracy with full EDA, feature engineering, and interpretable risk-factor ranking for medical teams.</p>
        <div class="repo-meta">
          <span><span class="lang-dot" style="background:#3572A5"></span>Python</span>
          <span>⭐ 7</span>
          <span>🍴 1</span>
        </div>
      </a>

      <a class="repo-card" href="https://github.com/asr-alurisanthoshreddy/football-fixture-gen" target="_blank" rel="noopener">
        <span class="pinned-badge">Pinned</span>
        <div class="repo-top">
          <div class="repo-ico ri-warn">🏟️</div>
          <div>
            <div class="repo-name">
              football-fixture-gen
              <span class="repo-badge rb-warn">C++</span>
            </div>
          </div>
        </div>
        <p class="repo-desc">Round-robin tournament fixture generator in C++. Built for fun to sharpen DSA skills — scheduling algorithm handles any number of teams and match weeks.</p>
        <div class="repo-meta">
          <span><span class="lang-dot" style="background:#f34b7d"></span>C++</span>
          <span>⭐ 2</span>
          <span>🍴 0</span>
        </div>
      </a>

    </div>
  </section>


  <!-- ╔══════════════════════════════╗
       ║         TECH STACK           ║
       ╚══════════════════════════════╝ -->
  <section class="panel reveal d2">
    <div class="section-head"><div class="bar"></div>🛠️ Tech stack</div>

    <div class="tech-group">
      <div class="tech-cat">Salesforce Platform</div>
      <div class="pills">
        <span class="pill p-sf">Apex</span>
        <span class="pill p-sf">Async Apex</span>
        <span class="pill p-sf">LWC</span>
        <span class="pill p-sf">SOQL / SOSL</span>
        <span class="pill p-sf">Flows</span>
        <span class="pill p-sf">REST APIs</span>
        <span class="pill p-sf">Named Credentials</span>
        <span class="pill p-sf">Agentforce</span>
        <span class="pill p-sf">Einstein AI</span>
        <span class="pill p-sf">Prompt Builder</span>
        <span class="pill p-sf">Sales Cloud</span>
        <span class="pill p-sf">Service Cloud</span>
        <span class="pill p-sf">Security Model</span>
        <span class="pill p-sf">SFDX · CLI</span>
      </div>
    </div>

    <div class="tech-group">
      <div class="tech-cat">AI / ML / Deep Learning</div>
      <div class="pills">
        <span class="pill p-ai">Python</span>
        <span class="pill p-ai">PyTorch</span>
        <span class="pill p-ai">TensorFlow</span>
        <span class="pill p-ai">XGBoost</span>
        <span class="pill p-ai">scikit-learn</span>
        <span class="pill p-ai">OpenCV</span>
        <span class="pill p-ai">CNN · Attention</span>
        <span class="pill p-ai">Hyperspectral Imaging</span>
        <span class="pill p-ai">Feature Engineering</span>
        <span class="pill p-ai">C++</span>
      </div>
    </div>

    <div class="tech-group">
      <div class="tech-cat">Data &amp; Infrastructure</div>
      <div class="pills">
        <span class="pill p-dt">SQL</span>
        <span class="pill p-dt">Oracle DB</span>
        <span class="pill p-dt">OCI</span>
        <span class="pill p-dt">AWS</span>
        <span class="pill p-dt">Git · GitHub</span>
        <span class="pill p-dt">VS Code</span>
        <span class="pill p-dt">Data Loader</span>
        <span class="pill p-dt">Change Sets</span>
      </div>
    </div>
  </section>


  <!-- ╔══════════════════════════════╗
       ║     CONTRIBUTION GRAPH       ║
       ╚══════════════════════════════╝ -->
  <section class="panel reveal d2">
    <div class="section-head"><div class="bar"></div>📊 GitHub contribution graph</div>
    <div class="graph-wrap">
      <img
        src="https://ghchart.rshah.org/9D4EDD/asr-alurisanthoshreddy"
        alt="GitHub Contribution Chart"
        onerror="this.style.display='none';this.nextElementSibling.style.display='block'"
      />
      <div style="display:none;padding:20px;text-align:center;font-family:var(--mono);font-size:.8rem;color:var(--text-3)">
        📊 Contribution graph loads once your GitHub account has activity.<br/>
        <a href="https://github.com/asr-alurisanthoshreddy" target="_blank" style="color:var(--sf)">View on GitHub →</a>
      </div>
      <div class="graph-meta">Past 12 months — contributions streak</div>
    </div>
  </section>


  <!-- ╔══════════════════════════════╗
       ║         EXPERIENCE           ║
       ╚══════════════════════════════╝ -->
  <section class="panel reveal d1">
    <div class="section-head"><div class="bar"></div>💼 Experience</div>

    <div class="exp-item">
      <div class="exp-dot"></div>
      <div>
        <div class="exp-role">Salesforce AI Agent Developer Trainee</div>
        <div class="exp-where">SmartBridge · Hyderabad, India</div>
        <div class="exp-when">Jul 2025 – Oct 2025</div>
        <div class="exp-desc">
          Completed structured training across Apex, Triggers, SOQL, Flows, Async Apex, REST API integrations, Security Model, Sales Cloud, Service Cloud, LWC, and Agentforce. Earned Trailhead Ranger rank with 100+ badges. Built the Tourism Management System end-to-end as capstone — data modelling, Apex automation, security config, and live dashboards in a single production-grade Salesforce app.
        </div>
      </div>
    </div>

    <div class="exp-item">
      <div class="exp-dot" style="background:var(--ai);box-shadow:0 0 8px var(--ai)"></div>
      <div>
        <div class="exp-role">AI/ML Research — Deep Learning (Independent)</div>
        <div class="exp-where">CMR College of Engineering &amp; Technology · Hyderabad</div>
        <div class="exp-when">Nov 2025</div>
        <div class="exp-desc">
          Designed and implemented HSSAN — a multi-modal deep learning framework fusing RGB, multispectral, and hyperspectral inputs via 2D/3D conv layers and a dual attention mechanism. Achieved 92.8% accuracy (F1 91.8%) on fine-grained flower classification — a 6–8 percentage point improvement over the RGB-only CNN baseline.
        </div>
      </div>
    </div>
  </section>


  <!-- ╔══════════════════════════════╗
       ║       CERTIFICATIONS         ║
       ╚══════════════════════════════╝ -->
  <section class="panel reveal d2">
    <div class="section-head"><div class="bar"></div>🏆 Certifications</div>

    <div class="certs-row">
      <div class="cert-card">
        <div class="cert-ico">☁️</div>
        <div>
          <div class="cert-name">Salesforce Agentforce Specialist</div>
          <div class="cert-by">Salesforce · Dec 2025</div>
        </div>
      </div>
      <div class="cert-card">
        <div class="cert-ico">🗄️</div>
        <div>
          <div class="cert-name">Oracle DB @ AWS — Architect Pro</div>
          <div class="cert-by">Oracle · Oct 2025</div>
        </div>
      </div>
      <div class="cert-card">
        <div class="cert-ico">🤖</div>
        <div>
          <div class="cert-name">OCI 2025 AI Foundations Associate</div>
          <div class="cert-by">Oracle · Aug 2025</div>
        </div>
      </div>
    </div>

    <div class="cert-featured">
      <div class="cf-ico">🏅</div>
      <div>
        <div class="cf-name">Salesforce Trailhead Ranger</div>
        <div class="cf-det">100+ hands-on badges · Apex · LWC · Agentforce · Security · Integrations · Admin</div>
      </div>
    </div>
  </section>


  <!-- ╔══════════════════════════════╗
       ║        CONNECT WITH ME       ║
       ╚══════════════════════════════╝ -->
  <section class="panel reveal d3">
    <div class="section-head"><div class="bar"></div>✉️ Connect with me</div>

    <div class="connect-grid">
      <a class="connect-card" href="https://linkedin.com/in/aluri-santhosh-reddy" target="_blank" rel="noopener">
        <div class="cc-ico" style="background:rgba(10,102,194,.15);border:1px solid rgba(10,102,194,.3)">💼</div>
        <div><div class="cc-label">LinkedIn</div><div class="cc-val">alurisanthoshreddy</div></div>
      </a>
      <a class="connect-card" href="https://github.com/asr-alurisanthoshreddy" target="_blank" rel="noopener">
        <div class="cc-ico" style="background:rgba(110,118,129,.12);border:1px solid rgba(110,118,129,.3)">🐙</div>
        <div><div class="cc-label">GitHub</div><div class="cc-val">@asr-alurisanthoshreddy</div></div>
      </a>
      <a class="connect-card" href="mailto:alurisanthoshreddy963@gmail.com">
        <div class="cc-ico" style="background:rgba(234,67,53,.1);border:1px solid rgba(234,67,53,.3)">📧</div>
        <div><div class="cc-label">Email</div><div class="cc-val">alurisanthoshreddy963<br/>@gmail.com</div></div>
      </a>
      <a class="connect-card" href="mailto:asr.ac@outlook.com">
        <div class="cc-ico" style="background:rgba(0,120,212,.1);border:1px solid rgba(0,120,212,.3)">📨</div>
        <div><div class="cc-label">Alt Email</div><div class="cc-val">asr.ac@outlook.com</div></div>
      </a>
      <a class="connect-card" href="tel:+916300865527">
        <div class="cc-ico" style="background:rgba(37,211,102,.1);border:1px solid rgba(37,211,102,.3)">📱</div>
        <div><div class="cc-label">Phone</div><div class="cc-val">+91 6300865527</div></div>
      </a>
      <div class="connect-card" style="cursor:default">
        <div class="cc-ico" style="background:rgba(157,78,221,.1);border:1px solid rgba(157,78,221,.3)">📍</div>
        <div><div class="cc-label">Location</div><div class="cc-val">Hyderabad, India</div></div>
      </div>
    </div>
  </section>


  <!-- ╔══════════════════════════════╗
       ║           FOOTER             ║
       ╚══════════════════════════════╝ -->
  <footer class="footer reveal">
    <div class="footer-views">
      👁 Profile views &nbsp;
      <img
        src="https://komarev.com/ghpvc/?username=asr-alurisanthoshreddy&style=flat-square&color=9D4EDD&label="
        alt="views"
      />
    </div>
    <p class="footer-note">⭐ If this profile helped you, consider <a href="https://github.com/asr-alurisanthoshreddy" target="_blank" rel="noopener">starring my repos!</a></p>
  </footer>

</div><!-- /wrap -->


<!-- ╔══════════════════════════════════════════════════════╗
     ║                    SCRIPTS                          ║
     ╚══════════════════════════════════════════════════════╝ -->
<script>
  /* ── 1. Typing animation ────────────────────────────── */
  const ROLES = [
    '> Salesforce Developer · Agentforce Specialist · AI/ML Engineer',
    '> Trailhead Ranger · 100+ Badges · Apex &amp; LWC Expert',
    '> Deep Learning Researcher · HSSAN · 92.8% Accuracy',
    '> Oracle OCI Certified · AWS Architect Professional',
    '> B.Tech AI &amp; ML 2026 · Open to Full-Time Roles',
  ];
  let ri = 0, ci = 0, del = false;
  const rt = document.getElementById('role-txt');

  function type() {
    const cur = ROLES[ri];
    if (!del) {
      rt.innerHTML = cur.slice(0, ++ci);
      if (ci === cur.length) { del = true; setTimeout(type, 2400); return; }
      setTimeout(type, 36);
    } else {
      rt.innerHTML = cur.slice(0, --ci);
      if (ci === 0) { del = false; ri = (ri + 1) % ROLES.length; setTimeout(type, 340); return; }
      setTimeout(type, 16);
    }
  }
  type();

  /* ── 2. Animated counters ──────────────────────────── */
  function countUp(el, target, sfx, dec, dur) {
    const t0 = performance.now();
    (function step(now) {
      const p = Math.min((now - t0) / dur, 1);
      const e = 1 - Math.pow(1 - p, 3);           // ease-out-cubic
      const v = e * target;
      el.textContent = (dec > 0 ? v.toFixed(dec) : Math.floor(v)) + sfx;
      if (p < 1) requestAnimationFrame(step);
    })(performance.now());
  }

  /* ── 3. Intersection Observer ──────────────────────── */
  let countersDone = false;
  const counters   = document.querySelectorAll('.stat-num[data-to]');
  const revEls     = document.querySelectorAll('.reveal');

  const io = new IntersectionObserver(entries => {
    entries.forEach(e => {
      if (!e.isIntersecting) return;
      e.target.classList.add('in');

      // trigger counters when stat grid scrolls in
      if (!countersDone && e.target.closest && e.target.closest('.stats-grid')) {
        countersDone = true;
        counters.forEach(c => {
          countUp(c,
            parseFloat(c.dataset.to),
            c.dataset.sfx  || '',
            parseInt(c.dataset.dec || '0'),
            1600
          );
        });
      }
    });
  }, { threshold: 0.15 });

  revEls.forEach(el => io.observe(el));

  // Also observe stat grid specifically
  const sg = document.querySelector('.stats-grid');
  if (sg) io.observe(sg);
</script>
</body>
</html>