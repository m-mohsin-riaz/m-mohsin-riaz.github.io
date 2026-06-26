---
layout: home
---

<style>
  .site-header { display: none !important; }
  .page-content { padding: 0 !important; }
  .wrapper { max-width: 100% !important; padding: 0 !important; }

  body { background: #0f0e17 !important; font-family: 'Poppins', sans-serif; transition: background 0.3s; }
  body.light-mode { background: #f0f2f8 !important; }

  .gn-wrap {
    background: linear-gradient(145deg, #1a1a2e 0%, #16213e 100%);
    border-radius: 20px; padding: 32px 28px;
    max-width: 900px; margin: 32px auto;
    box-shadow: 0 24px 64px rgba(0,0,0,0.55);
    transition: background 0.3s;
  }
  body.light-mode .gn-wrap {
    background: linear-gradient(145deg, #ffffff 0%, #f4f6fb 100%);
    box-shadow: 0 20px 50px rgba(0,0,0,0.12);
  }

  .gn-hero {
    display: flex; align-items: center; justify-content: space-between;
    background: rgba(255,255,255,0.06); border: 1px solid rgba(255,255,255,0.12);
    border-radius: 18px; padding: 28px 32px; margin-bottom: 32px;
    gap: 28px; backdrop-filter: blur(12px); transition: background 0.3s;
  }
  body.light-mode .gn-hero { background: rgba(255,255,255,0.9); border-color: rgba(0,0,0,0.08); }

  .gn-left { display: flex; align-items: center; gap: 24px; flex: 1; }

  .gn-left img {
    width: 112px; height: 112px; border-radius: 50%; object-fit: cover;
    border: 3px solid #e94560; box-shadow: 0 0 24px rgba(233,69,96,0.5);
    flex-shrink: 0; transition: transform 0.3s, box-shadow 0.3s;
  }
  .gn-left img:hover { transform: scale(1.07); box-shadow: 0 0 36px rgba(233,69,96,0.85); }

  .gn-left h1 { font-size: 24px; font-weight: 700; color: #ffffff; margin: 0 0 6px; }
  body.light-mode .gn-left h1 { color: #1a1a2e; }
  .gn-left p { font-size: 13px; color: #c0c8e0; margin: 0; }
  body.light-mode .gn-left p { color: #555; }

  .gn-navgrid { display: grid; grid-template-columns: 1fr 1fr; gap: 14px 32px; }

  .gn-link {
    display: flex; flex-direction: column; align-items: center; gap: 6px;
    text-decoration: none; cursor: pointer; background: none; border: none;
    transition: transform 0.2s;
  }
  .gn-link:hover { transform: translateY(-3px); }
  .gn-ic { font-size: 26px; }
  .gn-link .lbl { font-size: 11px; color: #e8edf8; font-weight: 600; white-space: nowrap; }
  body.light-mode .gn-link .lbl { color: #1a1a2e; }

  .gn-label { text-align: center; margin: 0 0 22px; }
  .gn-label .eyebrow { display: block; font-size: 11px; letter-spacing: 2px; text-transform: uppercase; color: #e94560; margin-bottom: 7px; font-weight: 600; }
  .gn-label h2 { font-size: 23px; color: #ffffff; margin: 0; font-weight: 700; }
  body.light-mode .gn-label h2 { color: #1a1a2e; }

  .gn-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; margin-bottom: 16px; }

  .gn-card {
    background: rgba(255,255,255,0.08); border: 1px solid rgba(255,255,255,0.11);
    border-left: 4px solid #e94560; border-radius: 14px; padding: 20px;
    transition: transform 0.25s, box-shadow 0.25s;
  }
  .gn-card:hover { transform: translateY(-4px); box-shadow: 0 14px 32px rgba(233,69,96,0.22); }
  body.light-mode .gn-card { background: #ffffff; border-color: rgba(0,0,0,0.07); }

  .gn-card-head { display: flex; align-items: center; justify-content: space-between; gap: 6px; margin-bottom: 12px; }
  .gn-card-head h3 { font-size: 13.5px; color: #ffffff; margin: 0; font-weight: 700; }
  body.light-mode .gn-card-head h3 { color: #1a1a2e; }
  .gn-card-head .ic { font-size: 18px; }

  .gn-card p { font-size: 12px; line-height: 1.65; color: #c8d2e8; margin: 0; }
  body.light-mode .gn-card p { color: #444; }

  .gn-card ul { margin: 0; padding: 0; list-style: none; }
  .gn-card ul li { font-size: 12px; line-height: 1.75; color: #c8d2e8; padding-left: 14px; position: relative; }
  body.light-mode .gn-card ul li { color: #444; }
  .gn-card ul li::before { content: ""; position: absolute; left: 0; top: 8px; width: 5px; height: 5px; border-radius: 50%; background: #e94560; }

  .gn-fact .gn-card-head h3 { font-size: 10px; text-transform: uppercase; letter-spacing: 1.2px; color: #6b7a99; font-weight: 600; }
  body.light-mode .gn-fact .gn-card-head h3 { color: #aaa; }
  .gn-fact p { font-size: 16px !important; font-weight: 700 !important; color: #ffffff !important; }
  body.light-mode .gn-fact p { color: #1a1a2e !important; }

  @media (max-width: 600px) {
    .gn-hero { flex-direction: column; align-items: flex-start; }
    .gn-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="gn-wrap">
  <div class="gn-hero">
    <div class="gn-left">
      <img src="/mohsin.jpg.jpeg" alt="Mohsin Riaz">
      <div>
        <h1>Mohsin Riaz</h1>
        <p>Computer Engineer</p>
      </div>
    </div>
    <div class="gn-navgrid">
      <a href="/myjourney/" class="gn-link"><span class="gn-ic">📖</span><span class="lbl">My Journey</span></a>
      <a href="/about/" class="gn-link"><span class="gn-ic">👤</span><span class="lbl">About Me</span></a>
      <a href="/contact/" class="gn-link"><span class="gn-ic">✉️</span><span class="lbl">Contact Me</span></a>
      <button class="gn-link" id="theme-btn" onclick="toggleTheme()">
        <span class="gn-ic" id="theme-icon">🌙</span>
        <span class="lbl" id="theme-lbl">Dark Mode</span>
      </button>
    </div>
  </div>

  <div class="gn-label">
    <span class="eyebrow">Overview</span>
    <h2>Professional Profile</h2>
  </div>

  <div class="gn-grid">
    <div class="gn-card">
      <div class="gn-card-head"><h3>Professional Profile</h3><span class="ic">🧑‍💻</span></div>
      <p>Welcome to my official academic portfolio documenting my 8-semester journey in Computer Engineering.</p>
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
      <p>Build a comprehensive repository of academic projects across all 8 semesters.</p>
    </div>
  </div>

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
  function toggleTheme() {
    var isLight = document.body.classList.toggle('light-mode');
    document.getElementById('theme-icon').textContent = isLight ? '☀️' : '🌙';
    document.getElementById('theme-lbl').textContent = isLight ? 'Light Mode' : 'Dark Mode';
    localStorage.setItem('theme', isLight ? 'light' : 'dark');
  }
  (function() {
    if (localStorage.getItem('theme') === 'light') {
      document.body.classList.add('light-mode');
      document.getElementById('theme-icon').textContent = '☀️';
      document.getElementById('theme-lbl').textContent = 'Light Mode';
    }
  })();
</script>
