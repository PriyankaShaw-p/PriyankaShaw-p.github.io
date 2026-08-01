
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Priyanka Shaw — Cloud Operations &amp; FinOps</title>
<meta name="description" content="Priyanka Shaw — Cloud Operations Associate &amp; FinOps Cost Consultant specializing in Microsoft Azure infrastructure and cost optimization.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#0A1120;
    --panel:#111B2E;
    --panel-2:#16223A;
    --panel-border: rgba(231,236,244,0.09);
    --text:#E9EEF7;
    --muted:#8996B3;
    --muted-2:#5D6B8A;
    --accent:#34D8C6;
    --accent-dim: rgba(52,216,198,0.14);
    --amber:#F2A65A;
    --amber-dim: rgba(242,166,90,0.14);
    --radius: 14px;
  }

  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    margin:0;
    background:
      radial-gradient(1100px 560px at 82% -8%, rgba(52,216,198,0.10), transparent 60%),
      radial-gradient(900px 500px at -5% 10%, rgba(242,166,90,0.07), transparent 55%),
      var(--bg);
    color:var(--text);
    font-family:'Inter', sans-serif;
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
  }
  h1,h2,h3,.display{ font-family:'Space Grotesk', sans-serif; letter-spacing:-0.01em; }
  .mono{ font-family:'JetBrains Mono', monospace; }
  a{ color:inherit; }
  ::selection{ background:var(--accent); color:#04201C; }
  :focus-visible{ outline:2px solid var(--accent); outline-offset:3px; border-radius:4px; }
  svg{ display:block; }
  .icon{ width:16px; height:16px; flex-shrink:0; }

  .wrap{ max-width:1120px; margin:0 auto; padding:0 28px; }

  /* ---------- Nav ---------- */
  .nav{
    position:sticky; top:0; z-index:50;
    backdrop-filter:saturate(140%) blur(10px);
    background:rgba(10,17,32,0.72);
    border-bottom:1px solid var(--panel-border);
  }
  .nav .wrap{ display:flex; align-items:center; justify-content:space-between; height:64px; }
  .nav-mark{ display:flex; align-items:center; gap:10px; font-weight:600; font-size:0.98rem; }
  .nav-mark .dot{ width:8px; height:8px; border-radius:50%; background:var(--accent); box-shadow:0 0 0 3px var(--accent-dim); }
  .nav-links{ display:flex; gap:28px; font-size:0.88rem; color:var(--muted); }
  .nav-links a{ text-decoration:none; transition:color .15s ease; }
  .nav-links a:hover{ color:var(--text); }
  .nav-cta{
    display:inline-flex; align-items:center; gap:7px;
    font-size:0.82rem; padding:8px 14px; border-radius:8px;
    border:1px solid var(--panel-border); color:var(--text); text-decoration:none;
    transition:border-color .15s ease, background .15s ease;
  }
  .nav-cta:hover{ border-color:var(--accent); background:var(--accent-dim); }
  @media (max-width:760px){ .nav-links{ display:none; } }

  /* ---------- Hero ---------- */
  .hero{ padding:88px 0 64px; }
  .hero-grid{ display:grid; grid-template-columns: 1.1fr 0.9fr; gap:48px; align-items:center; }
  @media (max-width:900px){ .hero-grid{ grid-template-columns:1fr; } }

  .stage-track{ display:flex; align-items:center; gap:6px; margin-bottom:22px; }
  .stage{
    font-family:'JetBrains Mono', monospace; font-size:0.68rem; letter-spacing:0.12em;
    text-transform:uppercase; color:var(--muted-2); padding:4px 9px; border-radius:6px;
    border:1px solid var(--panel-border);
  }
  .stage.active{ color:var(--accent); border-color:rgba(52,216,198,0.35); background:var(--accent-dim); }
  .stage-arrow{ color:var(--muted-2); font-size:0.75rem; }

  .hero h1{ font-size:2.7rem; margin:0 0 8px; line-height:1.08; }
  .hero h1 .accent{ color:var(--accent); }
  .hero .role{ font-size:1.05rem; color:var(--muted); margin:0 0 20px; font-weight:500; }
  .hero p.thesis{ color:var(--muted); font-size:1rem; max-width:46ch; margin:0 0 28px; }

  .cta-row{ display:flex; flex-wrap:wrap; gap:12px; }
  .btn{
    display:inline-flex; align-items:center; gap:8px;
    padding:11px 18px; border-radius:9px; font-size:0.88rem; font-weight:600;
    text-decoration:none; transition:transform .15s ease, box-shadow .15s ease, background .15s ease;
  }
  .btn-primary{ background:var(--accent); color:#04201C; }
  .btn-primary:hover{ transform:translateY(-1px); box-shadow:0 8px 22px rgba(52,216,198,0.25); }
  .btn-ghost{ border:1px solid var(--panel-border); color:var(--text); }
  .btn-ghost:hover{ border-color:var(--muted); background:rgba(255,255,255,0.03); }

  /* ---------- Signature diagram ---------- */
  .diagram-card{
    background:linear-gradient(180deg, var(--panel), var(--panel-2));
    border:1px solid var(--panel-border); border-radius:var(--radius);
    padding:22px 20px 18px; position:relative; overflow:hidden;
  }
  .diagram-card::before{
    content:"deployment.trace"; position:absolute; top:14px; right:18px;
    font-family:'JetBrains Mono', monospace; font-size:0.65rem; color:var(--muted-2); letter-spacing:0.06em;
  }
  svg#arch{ width:100%; height:auto; display:block; }
  .node-label{ font-family:'JetBrains Mono', monospace; font-size:9.5px; fill:var(--muted); }
  .node-box{ fill:var(--panel-2); stroke:var(--panel-border); stroke-width:1; }
  .node-box.dashboard{ stroke:var(--amber); fill:var(--amber-dim); }
  .edge{ stroke:var(--panel-border); stroke-width:1.4; fill:none; }
  .pulse{ fill:var(--accent); filter:drop-shadow(0 0 4px rgba(52,216,198,0.8)); }
  .savings-tag{ font-family:'JetBrains Mono', monospace; font-size:11px; fill:var(--amber); font-weight:600; }

  @keyframes travel1{ 0%{ offset-distance:0%; opacity:0; } 8%{ opacity:1; } 92%{opacity:1;} 100%{ offset-distance:100%; opacity:0; } }
  .p1{ offset-path: path("M20,40 L120,40 L150,90 L250,90"); animation: travel1 3.2s linear infinite; }
  .p2{ offset-path: path("M20,90 L90,90 L120,40 L250,90"); animation: travel1 3.6s linear infinite 0.6s; }
  .p3{ offset-path: path("M20,140 L120,140 L150,90 L250,90"); animation: travel1 2.9s linear infinite 1.1s; }

  @keyframes spin-slow{ from{ transform:rotate(0deg); } to{ transform:rotate(360deg); } }
  @media (prefers-reduced-motion: reduce){
    .p1,.p2,.p3{ animation:none; opacity:0.9; }
    .loop-ring{ animation:none !important; }
    html{ scroll-behavior:auto; }
  }

  /* ---------- Section shell ---------- */
  section{ padding:64px 0; border-top:1px solid var(--panel-border); }
  .section-head{ display:flex; align-items:baseline; justify-content:space-between; margin-bottom:34px; flex-wrap:wrap; gap:12px; }
  .section-head h2{ font-size:1.5rem; margin:0; }
  .section-tag{ font-family:'JetBrains Mono', monospace; font-size:0.72rem; color:var(--muted-2); letter-spacing:0.1em; text-transform:uppercase; }

  /* ---------- About ---------- */
  .about-grid{ display:grid; grid-template-columns: 1.3fr 0.7fr; gap:40px; }
  @media (max-width:820px){ .about-grid{ grid-template-columns:1fr; } }
  .about-grid p{ color:var(--muted); font-size:0.98rem; max-width:62ch; }
  .stat-list{ display:flex; flex-direction:column; gap:16px; }
  .stat{ border:1px solid var(--panel-border); border-radius:10px; padding:14px 16px; background:var(--panel); }
  .stat .num{ font-family:'Space Grotesk', sans-serif; font-size:1.35rem; font-weight:600; color:var(--accent); }
  .stat .lab{ font-size:0.78rem; color:var(--muted); margin-top:2px; }

  /* ---------- FinOps loop visual ---------- */
  .loop-wrap{ display:grid; grid-template-columns: 0.55fr 1.45fr; gap:40px; align-items:center; }
  @media (max-width:820px){ .loop-wrap{ grid-template-columns:1fr; } }
  .loop-ring{ animation: spin-slow 26s linear infinite; transform-origin:100px 100px; }
  .loop-steps{ display:flex; flex-direction:column; gap:16px; }
  .loop-step{ display:flex; gap:14px; align-items:flex-start; border:1px solid var(--panel-border); border-radius:10px; padding:14px 16px; background:var(--panel); }
  .loop-step .num-badge{
    font-family:'JetBrains Mono', monospace; font-size:0.72rem; font-weight:600; color:var(--bg);
    background:var(--accent); width:24px; height:24px; border-radius:6px; display:flex; align-items:center; justify-content:center; flex-shrink:0;
  }
  .loop-step h4{ margin:0 0 4px; font-size:0.94rem; }
  .loop-step p{ margin:0; font-size:0.85rem; color:var(--muted); }

  /* ---------- Skills ---------- */
  .skills-cols{ display:grid; grid-template-columns:1fr 1fr; gap:20px; }
  @media (max-width:820px){ .skills-cols{ grid-template-columns:1fr; } }
  .skill-card{
    background:var(--panel); border:1px solid var(--panel-border); border-radius:var(--radius); padding:22px;
  }
  .skill-card h3{ font-size:0.98rem; margin:0 0 14px; display:flex; align-items:center; gap:10px; }
  .skill-icon{ width:22px; height:22px; padding:5px; border-radius:7px; background:var(--accent-dim); color:var(--accent); flex-shrink:0; }
  .skill-icon.amber{ background:var(--amber-dim); color:var(--amber); }
  .tag-cloud{ display:flex; flex-wrap:wrap; gap:8px; }
  .tag{
    font-size:0.78rem; padding:6px 11px; border-radius:7px; border:1px solid var(--panel-border);
    color:var(--muted); background:rgba(255,255,255,0.02);
  }
  .soft-list{ list-style:none; margin:0; padding:0; display:flex; flex-direction:column; gap:10px; }
  .soft-list li{ font-size:0.9rem; color:var(--muted); padding-left:18px; position:relative; }
  .soft-list li::before{ content:"—"; position:absolute; left:0; color:var(--amber); }

  /* ---------- Experience ---------- */
  .pipeline{ position:relative; padding-left:28px; }
  .pipeline::before{ content:""; position:absolute; left:6px; top:6px; bottom:6px; width:1px; background:var(--panel-border); }
  .job{ position:relative; margin-bottom:36px; }
  .job:last-child{ margin-bottom:0; }
  .job::before{
    content:""; position:absolute; left:-28px; top:4px; width:12px; height:12px; border-radius:50%;
    background:var(--bg); border:2px solid var(--accent);
  }
  .job-head{ display:flex; justify-content:space-between; flex-wrap:wrap; gap:6px; margin-bottom:6px; }
  .job-head h3{ margin:0; font-size:1.08rem; }
  .job-head .dates{ font-family:'JetBrains Mono', monospace; font-size:0.76rem; color:var(--muted-2); }
  .job-co{ font-size:0.86rem; color:var(--accent); margin-bottom:12px; font-weight:500; }
  .job ul{ margin:0; padding-left:18px; color:var(--muted); font-size:0.92rem; }
  .job ul li{ margin-bottom:7px; }
  .job ul ul{ margin-top:7px; }

  /* ---------- Certifications ---------- */
  .cert-grid{ display:grid; grid-template-columns:repeat(4, 1fr); gap:14px; }
  @media (max-width:900px){ .cert-grid{ grid-template-columns:repeat(2,1fr); } }
  @media (max-width:480px){ .cert-grid{ grid-template-columns:1fr; } }
  .cert{
    border:1px solid var(--panel-border); border-radius:10px; padding:16px; background:var(--panel);
    transition:border-color .15s ease, transform .15s ease;
    display:flex; gap:12px; align-items:flex-start;
  }
  .cert:hover{ border-color:var(--accent); transform:translateY(-2px); }
  .cert .badge-icon{ width:26px; height:26px; flex-shrink:0; color:var(--accent); }
  .cert .code{ font-family:'JetBrains Mono', monospace; font-size:0.95rem; color:var(--accent); font-weight:600; }
  .cert .name{ font-size:0.8rem; color:var(--muted); margin-top:4px; }

  /* ---------- Education + languages ---------- */
  .split{ display:grid; grid-template-columns:1fr 1fr; gap:40px; }
  @media (max-width:820px){ .split{ grid-template-columns:1fr; } }
  .edu-item{ margin-bottom:18px; }
  .edu-item h3{ font-size:0.98rem; margin:0 0 3px; }
  .edu-item .meta{ font-size:0.82rem; color:var(--muted-2); font-family:'JetBrains Mono', monospace; }
  .lang-row{ display:flex; align-items:center; justify-content:space-between; padding:11px 0; border-bottom:1px solid var(--panel-border); font-size:0.9rem; }
  .lang-row:last-child{ border-bottom:none; }
  .lang-level{ font-family:'JetBrains Mono', monospace; font-size:0.76rem; color:var(--accent); }

  /* ---------- Contact ---------- */
  .contact-grid{ display:grid; grid-template-columns:1fr 1fr; gap:18px; }
  @media (max-width:700px){ .contact-grid{ grid-template-columns:1fr; } }
  .contact-card{
    display:flex; align-items:center; gap:16px; text-decoration:none; color:var(--text);
    border:1px solid var(--panel-border); border-radius:var(--radius); padding:22px;
    background:var(--panel); transition:border-color .15s ease, transform .15s ease, background .15s ease;
  }
  .contact-card:hover{ border-color:var(--accent); transform:translateY(-2px); background:var(--panel-2); }
  .contact-card .icon-wrap{
    width:44px; height:44px; border-radius:10px; background:var(--accent-dim); color:var(--accent);
    display:flex; align-items:center; justify-content:center; flex-shrink:0;
  }
  .contact-card .icon-wrap svg{ width:22px; height:22px; }
  .contact-card .c-label{ font-size:0.74rem; text-transform:uppercase; letter-spacing:0.1em; color:var(--muted-2); font-family:'JetBrains Mono', monospace; }
  .contact-card .c-value{ font-size:0.98rem; font-weight:600; margin-top:2px; word-break:break-word; }

  footer{ padding:56px 0 44px; border-top:1px solid var(--panel-border); }
  .footer-note{ font-size:0.78rem; color:var(--muted-2); margin-top:28px; text-align:center; }
</style>
</head>
<body>

<nav class="nav">
  <div class="wrap">
    <div class="nav-mark"><span class="dot"></span> Priyanka Shaw</div>
    <div class="nav-links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#experience">Experience</a>
      <a href="#certifications">Certifications</a>
      <a href="#contact">Contact</a>
    </div>
    <a class="nav-cta" href="#contact">
      <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16v16H4z" opacity="0"/><path d="M3 7l9 6 9-6"/><path d="M3 7v10h18V7"/></svg>
      Get in touch
    </a>
  </div>
</nav>

<header class="hero">
  <div class="wrap hero-grid">
    <div>
      <div class="stage-track">
        <span class="stage active">Inform</span>
        <span class="stage-arrow">→</span>
        <span class="stage">Optimize</span>
        <span class="stage-arrow">→</span>
        <span class="stage">Operate</span>
      </div>
      <h1>Priyanka Shaw<br><span class="accent">Cloud Ops &amp; FinOps,</span> built on Azure.</h1>
      <p class="role">Cloud Operations Associate · FinOps Cost Consultant · Kolkata, India</p>
      <p class="thesis">I run and secure Azure IaaS/PaaS environments, then turn the billing data those environments generate into rightsizing, tiering, and autoscaling decisions leadership can act on.</p>
      <div class="cta-row">
        <a class="btn btn-primary" href="mailto:priyanka251020000@gmail.com">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 7l9 6 9-6"/><path d="M3 7v10h18V7"/></svg>
          Email me
        </a>
        <a class="btn btn-ghost" href="https://www.linkedin.com/in/priyanka-shaw-b51507215" target="_blank" rel="noopener">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="7" cy="6" r="2.4"/><path d="M7 10.5v9"/><path d="M12 19.5v-5.2c0-2 1.4-3.3 3.1-3.3 1.7 0 2.9 1.2 2.9 3.3v5.2"/><path d="M12 10.5v9"/></svg>
          LinkedIn
        </a>
        <a class="btn btn-ghost" href="https://github.com/priyankashaw-p" target="_blank" rel="noopener">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="8 7 3 12 8 17"/><polyline points="16 7 21 12 16 17"/></svg>
          GitHub
        </a>
      </div>
    </div>

    <div class="diagram-card">
      <svg id="arch" viewBox="0 0 270 165" xmlns="http://www.w3.org/2000/svg">
        <path class="edge" d="M20,40 L120,40 L150,90 L250,90"/>
        <path class="edge" d="M20,90 L90,90 L120,40 L250,90"/>
        <path class="edge" d="M20,140 L120,140 L150,90 L250,90"/>

        <rect class="node-box" x="0" y="30" width="40" height="20" rx="5"/>
        <text class="node-label" x="20" y="43" text-anchor="middle">VM</text>

        <rect class="node-box" x="0" y="80" width="40" height="20" rx="5"/>
        <text class="node-label" x="20" y="93" text-anchor="middle">AKS</text>

        <rect class="node-box" x="0" y="130" width="40" height="20" rx="5"/>
        <text class="node-label" x="20" y="143" text-anchor="middle">Storage</text>

        <rect class="node-box" x="100" y="30" width="40" height="20" rx="5"/>
        <text class="node-label" x="120" y="43" text-anchor="middle">Gateway</text>

        <rect class="node-box" x="100" y="130" width="40" height="20" rx="5"/>
        <text class="node-label" x="120" y="143" text-anchor="middle">RBAC</text>

        <rect class="node-box dashboard" x="205" y="76" width="60" height="28" rx="6"/>
        <text class="node-label" x="235" y="91" text-anchor="middle" fill="#F2A65A">Cost Dashboard</text>
        <text class="savings-tag" x="235" y="118" text-anchor="middle">savings ↑</text>

        <circle class="pulse p1" r="2.6"/>
        <circle class="pulse p2" r="2.6"/>
        <circle class="pulse p3" r="2.6"/>
      </svg>
    </div>
  </div>
</header>

<main>

  <section id="about">
    <div class="wrap">
      <div class="section-head">
        <h2>Professional summary</h2>
        <span class="section-tag"></span>
      </div>
      <div class="about-grid">
        <p>
          Cloud operations professional with 3+ years architecting and managing Microsoft Azure IaaS/PaaS environments,
          with hands-on FinOps expertise driving measurable cost savings through Azure Cost Management, budgeting, and
          optimization initiatives. Comfortable across Infrastructure-as-Code (Terraform), CI/CD-based deployment, and
          security &amp; compliance (IAM, RBAC, NSGs, WAF) — and equally comfortable presenting the resulting savings to
          leadership through Power BI and Excel dashboards. Azure-certified across the Administrator, Developer, and
          Solutions Architect Expert tracks, with a track record of translating cloud spend data into rightsizing,
          storage-tiering, and autoscaling recommendations that improve ROI while holding the line on SLA-grade availability.
        </p>
        <div class="stat-list">
          <div class="stat"><div class="num">3+ yrs</div><div class="lab">Azure operations &amp; FinOps</div></div>
          <div class="stat"><div class="num">7</div><div class="lab">Microsoft certifications</div></div>
          <div class="stat"><div class="num">4</div><div class="lab">Languages spoken</div></div>
        </div>
      </div>
    </div>
  </section>

  <section id="approach">
    <div class="wrap">
      <div class="section-head">
        <h2>How I approach cloud spend</h2>
        <span class="section-tag">Framework</span>
      </div>
      <div class="loop-wrap">
        <svg viewBox="0 0 200 200" width="100%" height="auto">
          <g class="loop-ring">
            <circle cx="100" cy="100" r="78" fill="none" stroke="var(--panel-border)" stroke-width="1"/>
            <path d="M100,22 A78,78 0 0 1 167.5,139" fill="none" stroke="var(--accent)" stroke-width="3" stroke-linecap="round"/>
            <path d="M167.5,139 A78,78 0 0 1 32.5,139" fill="none" stroke="var(--amber)" stroke-width="3" stroke-linecap="round"/>
            <path d="M32.5,139 A78,78 0 0 1 100,22" fill="none" stroke="#5D6B8A" stroke-width="3" stroke-linecap="round"/>
          </g>
          <circle cx="100" cy="100" r="46" fill="var(--panel-2)" stroke="var(--panel-border)"/>
          <text x="100" y="96" text-anchor="middle" fill="var(--text)" font-family="Space Grotesk" font-size="13" font-weight="600">FinOps</text>
          <text x="100" y="112" text-anchor="middle" fill="var(--muted-2)" font-family="JetBrains Mono" font-size="9">loop</text>
        </svg>
        <div class="loop-steps">
          <div class="loop-step">
            <span class="num-badge">1</span>
            <div><h4>Inform</h4><p>Surface spend visibility with Cost Management, Billing exports, and Power BI dashboards that stakeholders can read at a glance.</p></div>
          </div>
          <div class="loop-step">
            <span class="num-badge">2</span>
            <div><h4>Optimize</h4><p>Turn that visibility into rightsizing, storage tiering, spot instances, and reserved-instance planning.</p></div>
          </div>
          <div class="loop-step">
            <span class="num-badge">3</span>
            <div><h4>Operate</h4><p>Keep it governed — autoscaling, budget alerts, and anomaly detection so savings hold over time.</p></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="skills">
    <div class="wrap">
      <div class="section-head">
        <h2>Skills</h2>
        <span class="section-tag"></span>
      </div>
      <div class="skills-cols">
        <div class="skill-card">
          <h3>
            <svg class="skill-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M17 18H6a4 4 0 1 1 .7-7.94A5.5 5.5 0 0 1 17 8.5a4 4 0 0 1 0 9.5z"/></svg>
            Azure Cloud &amp; Infrastructure
          </h3>
          <div class="tag-cloud">
            <span class="tag">Virtual Machines</span><span class="tag">App Services</span>
            <span class="tag">AKS</span><span class="tag">Azure Functions</span>
            <span class="tag">Storage Accounts</span><span class="tag">Application Gateway</span>
            <span class="tag">Load Balancers</span><span class="tag">Recovery Services Vault</span>
            <span class="tag">Azure AD</span><span class="tag">RBAC</span>
            <span class="tag">NSGs</span><span class="tag">WAF</span>
            <span class="tag">Private Endpoints</span>
          </div>
        </div>
        <div class="skill-card">
          <h3>
            <svg class="skill-icon amber" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="9"/><path d="M12 7v10M9 9.5c0-1.4 1.3-2.5 3-2.5s3 1 3 2.3c0 3-6 1.4-6 4.4 0 1.3 1.3 2.3 3 2.3s3-1.1 3-2.5"/></svg>
            FinOps &amp; Cost Optimization
          </h3>
          <div class="tag-cloud">
            <span class="tag">Azure Cost Management</span><span class="tag">Azure Advisor</span>
            <span class="tag">Billing Exports</span><span class="tag">Power BI Dashboards</span>
            <span class="tag">Budget Alerts</span><span class="tag">Anomaly Detection</span>
            <span class="tag">Rightsizing</span><span class="tag">Storage Tiering</span>
            <span class="tag">Spot Instances</span><span class="tag">Autoscaling</span>
            <span class="tag">Reserved Instances</span><span class="tag">Showback / Chargeback</span>
          </div>
        </div>
        <div class="skill-card">
          <h3>
            <svg class="skill-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 17l6-6-6-6M12 19h8"/></svg>
            DevOps &amp; Infrastructure-as-Code
          </h3>
          <div class="tag-cloud">
            <span class="tag">Terraform</span><span class="tag">Azure DevOps Pipelines</span>
            <span class="tag">Azure Repos &amp; Boards</span><span class="tag">Bitbucket</span>
            <span class="tag">Git Bash</span><span class="tag">CI/CD Automation</span>
            <span class="tag">IaC Governance</span>
          </div>
        </div>
        <div class="skill-card">
          <h3>
            <svg class="skill-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="4" width="18" height="12" rx="2"/><path d="M8 20h8M12 16v4"/></svg>
            Monitoring, ITSM &amp; Admin
          </h3>
          <div class="tag-cloud">
            <span class="tag">Azure Monitor</span><span class="tag">Log Analytics</span>
            <span class="tag">Application Insights</span><span class="tag">ITIL / ITSM</span>
            <span class="tag">Incident Mgmt</span><span class="tag">Change Mgmt</span>
            <span class="tag">Windows Server</span><span class="tag">Linux (basic)</span>
          </div>
        </div>
      </div>

      <div class="skill-card" style="margin-top:20px;">
        <h3>
          <svg class="skill-icon amber" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="9" cy="8" r="3.2"/><path d="M3 20c0-3.3 2.7-6 6-6s6 2.7 6 6"/><path d="M16.5 6.5a3.2 3.2 0 1 1 0 4.9M22 20c0-2.8-1.9-5-4.5-5.7"/></svg>
          Soft skills, at the level of strategic business operations
        </h3>
        <ul class="soft-list">
          <li><strong>Stakeholder communication</strong> — turning complex work into clear, decision-ready narratives leadership can act on.</li>
          <li><strong>Critical thinking</strong> — weighing trade-offs so decisions hold up against the bigger business picture, not just the task at hand.</li>
          <li><strong>Cross-functional collaboration</strong> — aligning different teams around a shared operational goal.</li>
          <li><strong>Client-facing consulting</strong> — understanding what a client actually needs and shaping the engagement around that.</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="experience">
    <div class="wrap">
      <div class="section-head">
        <h2>Experience</h2>
        <span class="section-tag"></span>
      </div>
      <div class="pipeline">
        <div class="job">
          <div class="job-head">
            <h3>Cloud Operations Associate</h3>
            <span class="dates mono">Sep 2023 — Present</span>
          </div>
          <div class="job-co">Accenture</div>
          <ul>
            <li>Designed and delivered scalable, secure, highly available Azure infrastructure (IaaS &amp; PaaS) spanning VMs, App Services, Functions, and AKS.</li>
            <li>Provisioned Storage Accounts, Load Balancers, and Recovery Services Vault; implemented Azure Backup across production servers.</li>
            <li>Published client-facing apps through Application Gateway with WAF, including custom rules tailored to client security requirements.</li>
            <li>Configured NSGs and private endpoints across Storage, App Services, and Azure Databases to enforce least-privilege access.</li>
            <li>Automated deployment with Terraform and Azure DevOps pipelines, using Bitbucket for version control and Git Bash for local scripting.</li>
            <li>Enforced IAM via Azure AD and RBAC; monitored environment health with Azure Monitor, Log Analytics, and Application Insights.</li>
            <li>
              FinOps &amp; cost optimization:
              <ul>
                <li>Built recurring cost/savings dashboards in Power BI and Excel for real-time visibility into Azure spend and budget variance.</li>
                <li>Used Cost Management + Billing and Azure Advisor to surface optimization opportunities and generate anomaly &amp; forecast reports.</li>
                <li>Ran billing exports into Excel/Power BI for chargeback and showback reporting across business units.</li>
                <li>Delivered savings through rightsizing, storage tiering (Hot/Cool/Archive), spot instances, autoscaling, and reserved instance planning.</li>
              </ul>
            </li>
          </ul>
        </div>
        <div class="job">
          <div class="job-head">
            <h3>Business Process Operations Analyst</h3>
            <span class="dates mono">Nov 2022 — Sep 2023</span>
          </div>
          <div class="job-co">Tata Consultancy Services</div>
          <ul>
            <li>Conducted in-depth market research on mergers and acquisitions to support client decision-making.</li>
            <li>Analyzed business processes and supported operational efficiency and project execution initiatives.</li>
            <li>Prepared reports, dashboards, and data analysis deliverables aligned to business requirements.</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <section id="certifications">
    <div class="wrap">
      <div class="section-head">
        <h2>Certifications</h2>
        <span class="section-tag"></span>
      </div>
      <div class="cert-grid">
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">AZ-305</div><div class="name">Azure Solutions Architect Expert</div></div></div>
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">AZ-104</div><div class="name">Azure Administrator Associate</div></div></div>
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">AZ-204</div><div class="name">Azure Developer Associate</div></div></div>
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">SC-900</div><div class="name">Security, Compliance &amp; Identity Fundamentals</div></div></div>
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">AI-900</div><div class="name">Azure AI Fundamentals</div></div></div>
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">AZ-900</div><div class="name">Azure Fundamentals</div></div></div>
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">MS-900</div><div class="name">Microsoft 365 Fundamentals</div></div></div>
        <div class="cert"><svg class="badge-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 2l8 3.5v6c0 5-3.4 8.4-8 10.5-4.6-2.1-8-5.5-8-10.5v-6L12 2z"/><path d="M8.5 12l2.3 2.3L16 9.5"/></svg><div><div class="code">GH-100</div><div class="name">GitHub Administration</div></div></div>
      </div>
    </div>
  </section>

  <section id="education">
    <div class="wrap">
      <div class="section-head">
        <h2>Education &amp; languages</h2>
        <span class="section-tag"></span>
      </div>
      <div class="split">
        <div>
          <div class="edu-item">
            <h3>Bachelor of Commerce — Electronic Business &amp; Computer Application (Honours)</h3>
            <div class="meta">Bhawanipur Education Society College, Kolkata · Aug 2022</div>
          </div>
          <div class="edu-item">
            <h3>ISC (12th Standard)</h3>
            <div class="meta">Young Horizons School, Kolkata · May 2019</div>
          </div>
          <div class="edu-item">
            <h3>ICSE (10th Standard)</h3>
            <div class="meta">Young Horizons School, Kolkata · May 2017</div>
          </div>
        </div>
        <div>
          <div class="lang-row"><span>Hindi</span><span class="lang-level">First language</span></div>
          <div class="lang-row"><span>English</span><span class="lang-level">Proficient · C2</span></div>
          <div class="lang-row"><span>Bengali</span><span class="lang-level">Proficient · C2</span></div>
          <div class="lang-row"><span>Spanish</span><span class="lang-level">Beginner · A1</span></div>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <div class="wrap">
      <div class="section-head">
        <h2>Get in touch</h2>
        <span class="section-tag">Contact</span>
      </div>
      <div class="contact-grid">
        <a class="contact-card" href="mailto:priyanka251020000@gmail.com">
          <span class="icon-wrap">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 7l9 6 9-6"/><path d="M3 7v10h18V7"/></svg>
          </span>
          <div>
            <div class="c-label">Email</div>
            <div class="c-value">priyanka251020000@gmail.com</div>
          </div>
        </a>
        <a class="contact-card" href="https://www.linkedin.com/in/priyanka-shaw-b51507215" target="_blank" rel="noopener">
          <span class="icon-wrap">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="7" cy="6" r="2.4"/><path d="M7 10.5v9"/><path d="M12 19.5v-5.2c0-2 1.4-3.3 3.1-3.3 1.7 0 2.9 1.2 2.9 3.3v5.2"/><path d="M12 10.5v9"/></svg>
          </span>
          <div>
            <div class="c-label">LinkedIn</div>
            <div class="c-value">/in/priyanka-shaw-b51507215</div>
          </div>
        </a>
      </div>
    </div>
  </section>

</main>

<footer>
  <div class="wrap">
    <p class="footer-note">Open to Cloud Operations and FinOps roles globally, with strong adjacent fit for Infrastructure/IT Support and strategic or functional positions.</p>
  </div>
</footer>

</body>
</html>
