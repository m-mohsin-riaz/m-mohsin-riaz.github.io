---
layout: home
---

<style>
  .gn-wrap {
    background: linear-gradient(145deg, #0a1628 0%, #050b18 100%);
    border: 1px solid rgba(0,229,255,0.12);
    border-radius: 20px; padding: 36px 30px;
    max-width: 920px; margin: 36px auto;
    box-shadow: 0 0 60px rgba(0,229,255,0.07), 0 24px 64px rgba(0,0,0,0.6);
    transition: all 0.4s;
    position: relative; overflow: hidden;
  }
  .gn-wrap::before {
    content: '';
    position: absolute; top: -100px; right: -100px;
    width: 350px; height: 350px;
    background: radial-gradient(circle, rgba(0,229,255,0.08) 0%, transparent 70%);
    pointer-events: none;
  }
  body.light-mode .gn-wrap {
    background: linear-gradient(145deg, #ffffff 0%, #f0f4ff 100%);
    border-color: rgba(0,119,204,0.15);
    box-shadow: 0 20px 50px rgba(0,119,204,0.08);
  }

  .gn-hero {
    display: flex; align-items: center; justify-content: space-between;
    background: rgba(0,229,255,0.04);
    border: 1px solid rgba(0,229,255,0.12);
    border-radius: 18px; padding: 30px 34px;
    margin-bottom: 36px; gap: 28px;
    backdrop-filter: blur(12px);
    position: relative;
  }
  body.light-mode .gn-hero {
    background: rgba(0,119,204,0.04);
    border-color: rgba(0,119,204,0.15);
  }

  .gn-left { display: flex; align-items: center; gap: 26px; flex: 1; }

  .gn-left img {
    width: 120px; height: 120px; border-radius: 50%; object-fit: cover;
    border: 2px solid rgba(0,229,255,0.6);
    box-shadow: 0 0 28px rgba(0,229,255,0.35), 0 0 60px rgba(0,229,255,0.12);
    flex-shrink: 0;
    transition: transform 0.3s, box-shadow 0.3s;
  }
  .gn-left img:hover {
    transform: scale(1.06);
    box-shadow: 0 0 40px rgba(0,229,255,0.6), 0 0 80px rgba(0,229,255,0.2);
  }
  body.light-mode .gn-left img {
    border-color: rgba(0,119,204,0.6);
    box-shadow: 0 0 24px rgba(0,119,204,0.25);
  }

  .gn-name-block h1 {
    font-size: 26px; font-weight: 700;
    color: #ffffff !important;
    margin: 0 0 4px;
    font-family: 'Inter', sans-serif;
    letter-spacing: -0.3px;
  }
  body.light-mode .gn-name-block h1 { color: #0f172a !important; }

  .gn-name-block .role {
    font-size: 13px;
    color: #00e5ff;
    font-family: 'Fira Code', monospace;
    margin: 0 0 6px;
    letter-spacing: 0.3px;
  }
  body.light-mode .gn-name-block .role { color: #0077cc; }

  .gn-name-block .sub {
    font-size: 12px; color: #7a90b8;
    margin: 0;
  }
  body.light-mode .gn-name-block .sub { color: #4a5568; }

  /* Status badge */
  .status-badge {
    display: inline-flex; align-items: center; gap: 6px;
    background: rgba(0,229,255,0.08);
    border: 1px solid rgba(0,229,255,0.2);
    border-radius: 20px; padding: 4px 12px;
    font-size: 11px; color: #00e5ff;
    font-family: 'Fira Code', monospace;
    margin-top: 10px;
  }
  .status-dot {
    width: 6px; height: 6px; border-radius: 50%;
    background: #00e5ff;
    box-shadow: 0 0 6px #00e5ff;
    animation: pulse 2s infinite;
  }
  @keyframes pulse { 0%,100%{opacity:1;} 50%{opacity:0.4;} }
  body.light-mode .status-badge {
    background: rgba(0,119,204,0.08);
    border-color: rgba(0,119,204,0.2);
    color: #0077cc;
  }
  body.light-mode .status-dot { background: #0077cc; box-shadow: 0 0 6px #0077cc; }

  .gn-navgrid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px 24px; }

  .gn-link {
    display: flex; flex-direction: column; align-items: center; gap: 6px;
    text-decoration: none; cursor: pointer;
    background: rgba(0,229,255,0.05);
    border: 1px solid rgba(0,229,255,0.12);
    border-radius: 12px; padding: 12px 16px;
    transition: all 0.25s;
    color: inherit;
  }
  .gn-link:hover {
    background: rgba(0,229,255,0.12);
    border-color: rgba(0,229,255,0.35);
    transform: translateY(-2px);
    box-shadow: 0 8px 24px rgba(0,229,255,0.12);
  }
  body.light-mode .gn-link {
    background: rgba(0,119,204,0.05);
    border-color: rgba(0,119,204,0.15);
  }
  body.light-mode .gn-link:hover {
    background: rgba(0,119,204,0.1);
    border-color: rgba(0,119,204,0.3);
    box-shadow: 0 8px 24px rgba(0,119,204,0.1);
  }

  .gn-ic { font-size: 22px; }
  .gn-link .lbl { font-size: 11px; color: #00e5ff; font-weight: 600; white-space: nowrap; font-family: 'Fira Code', monospace; }
  body.light-mode .gn-link .lbl { color: #0077cc; }

  /* Section label */
  .gn-label { text-align: center; margin: 0 0 24px; }
  .gn-label .eyebrow {
    display: block; font-size: 10px; letter-spacing: 3px;
    text-transform: uppercase; color: #00e5ff;
    margin-bottom: 8px; font-weight: 600;
    font-family: 'Fira Code', monospace;
  }
  body.light-mode .gn-label .eyebrow { color: #0077cc; }
  .gn-label h2 { font-size: 22px; color: #ffffff !important; margin: 0; font-weight: 700; }
  body.light-mode .gn-label h2 { color: #0f172a !important; }

  /* Cards */
  .gn-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; margin-bottom: 14px; }

  .gn-card {
    background: rgba(0,229,255,0.04);
    border: 1px solid rgba(0,229,255,0.1);
    border-top: 2px solid rgba(0,229,255,0.4);
    border-radius: 14px; padding: 20px;
    transition: transform 0.25s, box-shadow 0.25s, border-color 0.25s;
    position: relative; overflow: hidden;
  }
  .gn-card::after {
    content: '';
    position: absolute; bottom: 0; left: 0; right: 0;
    height: 1px;
    background: linear-gradient(90deg, transparent, rgba(0,229,255,0.3), transparent);
  }
  .gn-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 32px rgba(0,229,255,0.1);
    border-color: rgba(0,229,255,0.25);
  }
  body.light-mode .gn-card {
    background: #ffffff;
    border-color: rgba(0,119,204,0.1);
    border-top-color: rgba(0,119,204,0.5);
    box-shadow: 0 2px 12px rgba(0,119,204,0.06);
  }
  body.light-mode .gn-card:hover {
    box-shadow: 0 12px 32px rgba(0,119,204,0.12);
    border-color: rgba(0,119,204,0.25);
  }

  .gn-card-head { display: flex; align-items: center; justify-content: space-between; margin-bottom: 12px; }
  .gn-card-head h3 { font-size: 13px; color: #ffffff !important; margin: 0; font-weight: 700; letter-spacing: 0.2px; }
  body.light-mode .gn-card-head h3 { color: #0f172a !important; }
  .gn-card-head .ic { font-size: 17px; }

  .gn-card p { font-size: 12px; line-height: 1.7; color: #7a90b8 !important; margin: 0; }
  body.light-mode .gn-card p { color: #4a5568 !important; }

  .gn-card ul { margin: 0; padding: 0; list-style: none; }
  .gn-card ul li {
    font-size: 12px; line-height: 1.8; color: #7a90b8 !important;
    padding-left: 16px; position: relative;
  }
  body.light-mode .gn-card ul li { color: #4a5568 !important; }
  .gn-card ul li::before {
    content: ""; position: absolute; left: 0; top: 9px;
    width: 5px; height: 5px; border-radius: 50%;
    background: #00e5ff;
    box-shadow: 0 0 6px rgba(0,229,255,0.6);
  }
  body.light-mode .gn-card ul li::before { background: #0077cc; box-shadow: none; }

  /* Stat cards */
  .gn-fact .gn-card-head h3 {
    font-size: 10px; text-transform: uppercase;
    letter-spacing: 1.5px; color: #7a90b8 !important;
    font-weight: 600; font-family: 'Fira Code', monospace;
  }
  body.light-mode .gn-fact .gn-card-head h3 { color: #94a3b8 !important; }
  .gn-fact p {
    font-size: 15px !important; font-weight: 700 !important;
    color: #00e5ff !important;
    font-family: 'Fira Code', monospace;
  }
  body.light-mode .gn-fact p { color: #0077cc !important; }

  /* Divider */
  .gn-divider {
    height: 1px;
    background: linear-gradient(90deg, transparent, rgba(0,229,255,0.2), transparent);
    margin: 28px 0;
  }

  @media (max-width: 650px) {
    .gn-hero { flex-direction: column; }
    .gn-grid { grid-template-columns: 1fr; }
    .gn-navgrid { grid-template-columns: 1fr 1fr; }
  }
</style>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Fira+Code:wght@400;500&display=swap" rel="stylesheet">

<div class="gn-wrap">
  <div class="gn-hero">
    <div class="gn-left">
      <img src="/mohsin.jpg.jpeg" alt="Mohsin Riaz">
      <div class="gn-name-block">
        <h1>Mohsin Riaz</h1>
        <p class="role">&lt;Computer Engineer /&gt;</p>
        <p class="sub">UET Faisalabad · Lahore, Pakistan</p>
        <div class="status-badge">
          <span class="status-dot"></span>
          Available for Opportunities
        </div>
      </div>
    </div>
    <div class="gn-navgrid">
      <a href="/myjourney/" class="gn-link"><span class="gn-ic">📖</span><span class="lbl">My Journey</span></a>
      <a href="/about/" class="gn-link"><span class="gn-ic">👤</span><span class="lbl">About Me</span></a>
      <a href="/contact/" class="gn-link"><span class="gn-ic">✉️</span><span class="lbl">Contact Me</span></a>
      <button class="gn-link" id="home-theme-btn" onclick="toggleGlobalTheme()" style="border:none;">
        <span class="gn-ic" id="theme-icon">🌙</span>
        <span class="lbl" id="theme-lbl">Dark</span>
      </button>
    </div>
  </div>

  <div class="gn-label">
    <span class="eyebrow">// Overview</span>
    <h2>Professional Profile</h2>
  </div>

  <div class="gn-grid">
    <div class="gn-card">
      <div class="gn-card-head"><h3>About</h3><span class="ic">🧑‍💻</span></div>
      <p>Official academic portfolio documenting my 8-semester journey in Computer Engineering at UET Faisalabad.</p>
    </div>
    <div class="gn-card">
      <div class="gn-card-head"><h3>Current Focus</h3><span class="ic">🎯</span></div>
      <ul>
        <li>Programming Fundamentals</li>
        <li>Database Management</li>
        <li>C++, MySQL, GitHub, Jekyll</li>
      </ul>
    </div>
    <div class="gn-card">
      <div class="gn-card-head"><h3>Objective</h3><span class="ic">🏆</span></div>
      <p>Build a comprehensive repository of academic projects and growth across all 8 semesters.</p>
    </div>
  </div>

  <div class="gn-divider"></div>

  <div class="gn-grid" style="margin-bottom:0">
    <div class="gn-card gn-fact">
      <div class="gn-card-head"><h3>Degree</h3><span class="ic">🎓</span></div>
      <p>BS Computer Engineering</p>
    </div>
    <div class="gn-card gn-fact">
      <div class="gn-card-head"><h3>University</h3><span class="ic">🏛️</span></div>
      <p>UET Faisalabad</p>
    </div>
    <div class="gn-card gn-fact">
      <div class="gn-card-head"><h3>Home City</h3><span class="ic">🏙️</span></div>
      <p>Lahore</p>
    </div>
  </div>
</div>

<script>
  // Sync home page theme icons with global state
  document.addEventListener('DOMContentLoaded', function() {
    var isLight = document.body.classList.contains('light-mode');
    var ic = document.getElementById('theme-icon');
    var lbl = document.getElementById('theme-lbl');
    if (ic) ic.textContent = isLight ? '☀️' : '🌙';
    if (lbl) lbl.textContent = isLight ? 'Light' : 'Dark';
  });
</script>
