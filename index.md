---
layout: default
title: Home
---
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600;700&display=swap');

  /* ============ Hero Section ============ */
  .hero {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 18px;
    padding: 60px 20px 50px;
    text-align: center;
    margin-bottom: 45px;
    overflow: hidden;
    position: relative;
  }
  .hero::before {
    content: "";
    position: absolute;
    top: -60px;
    right: -60px;
    width: 220px;
    height: 220px;
    background: radial-gradient(circle, rgba(233,69,96,0.25), transparent 70%);
  }
  .hero img {
    width: 130px;
    height: 130px;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid #e94560;
    margin-bottom: 20px;
    display: block;
    margin-left: auto;
    margin-right: auto;
    position: relative;
    z-index: 1;
  }
  .hero h1 {
    font-family: 'Poppins', sans-serif;
    font-size: 32px;
    margin-bottom: 10px;
    font-weight: 700;
  }
  .hero p {
    font-size: 16px;
    color: #aaa;
    margin-bottom: 5px;
  }

  /* ============ Section Labels ============ */
  .section-label {
    text-align: center;
    margin: 0 0 22px;
  }
  .section-label .eyebrow {
    display: block;
    font-size: 12px;
    font-weight: 700;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    color: #e94560;
    margin-bottom: 6px;
  }
  .section-label h2 {
    font-family: 'Poppins', sans-serif;
    font-size: 22px;
    color: #1a1a2e;
    margin: 0;
  }

  /* ============ Shared Card Grid ============ */
  .cards-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
    max-width: 1050px;
    margin: 0 auto 50px;
  }

  /* ============ Highlight Cards (Profile / Focus / Objective) ============ */
  .highlight-card {
    background: white;
    border-radius: 14px;
    padding: 28px 24px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.06);
    border-left: 5px solid #e94560;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
  }
  .highlight-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 24px rgba(0,0,0,0.1);
  }
  .icon-badge {
    width: 48px;
    height: 48px;
    border-radius: 12px;
    background: rgba(233,69,96,0.1);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 22px;
    margin-bottom: 16px;
  }
  .highlight-card h3 {
    font-family: 'Poppins', sans-serif;
    font-size: 16px;
    color: #1a1a2e;
    margin: 0 0 10px;
  }
  .highlight-card p {
    font-size: 14px;
    line-height: 1.7;
    color: #555;
    margin: 0;
  }
  .highlight-card ul {
    margin: 0;
    padding-left: 0;
    list-style: none;
  }
  .highlight-card ul li {
    font-size: 14px;
    line-height: 1.7;
    color: #555;
    padding-left: 18px;
    position: relative;
    margin-bottom: 4px;
  }
  .highlight-card ul li::before {
    content: "";
    position: absolute;
    left: 0;
    top: 9px;
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: #e94560;
  }

  /* ============ Fact Cards (Degree / University / Home City) ============ */
  .fact-card {
    background: white;
    border-radius: 14px;
    padding: 26px 16px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.06);
    border-left: 5px solid #e94560;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    min-height: 150px;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
  }
  .fact-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 24px rgba(0,0,0,0.1);
  }
  .fact-card .icon-badge {
    width: 52px;
    height: 52px;
    border-radius: 50%;
    margin-bottom: 14px;
    font-size: 24px;
  }
  .fact-card h3 {
    font-size: 12px;
    color: #999;
    margin: 0 0 6px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.6px;
  }
  .fact-card p {
    font-size: 15px;
    font-weight: 700;
    color: #1a1a2e;
    margin: 0;
    line-height: 1.4;
  }

  /* ============ Top Navigation Icons (My Journey / About Me / Contact Me / Theme) ============
     Note: These selectors target the Type-on-Strap theme's navbar markup.
     If the icons don't visibly change after publishing, right-click one
     in the browser -> Inspect -> tell me the actual class name and I'll
     adjust the selector below. */
  header nav a i,
  header .menu a i,
  header li a i {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background: rgba(233,69,96,0.12);
    color: #e94560 !important;
    font-size: 14px;
    margin-bottom: 4px;
    transition: transform 0.2s ease, background 0.2s ease;
  }
  header nav a:hover i,
  header .menu a:hover i,
  header li a:hover i {
    transform: translateY(-3px);
    background: rgba(233,69,96,0.22);
  }
  header nav a,
  header .menu a,
  header li a {
    display: flex !important;
    flex-direction: column;
    align-items: center;
    gap: 2px;
    font-size: 11px;
    font-weight: 600;
  }

  /* ============ Hide duplicate site title in header (kept in hero already) ============ */
  header h1 {
    display: none;
  }

  /* ============ Mobile Responsive ============ */
  @media (max-width: 768px) {
    .cards-grid {
      grid-template-columns: 1fr;
      padding: 0 10px;
    }
    .fact-card { min-height: auto; }
  }
</style>

<div class="hero">
  <img src="/assets/images/mohsin.jpg.jpeg" alt="Mohsin Riaz">
  <h1>Mohsin Riaz</h1>
  <p>Computer Engineering Student</p>
</div>

<div class="section-label">
  <span class="eyebrow">Overview</span>
  <h2>Professional Profile</h2>
</div>
<div class="cards-grid">
  <div class="highlight-card">
    <div class="icon-badge">🧑‍💻</div>
    <h3>Professional Profile</h3>
    <p>Welcome to my official academic portfolio. This platform documents my 8-semester journey in Computer Engineering, focusing on technical excellence and structured learning.</p>
  </div>
  <div class="highlight-card">
    <div class="icon-badge">🎯</div>
    <h3>Current Focus</h3>
    <ul>
      <li>Programming Fundamentals</li>
      <li>Database Management Systems</li>
      <li>Technical Stack: C++, MySQL, GitHub, Jekyll</li>
    </ul>
  </div>
  <div class="highlight-card">
    <div class="icon-badge">🏆</div>
    <h3>Objective</h3>
    <p>To build a comprehensive repository of academic projects and lab implementations across all 8 semesters of Computer Engineering.</p>
  </div>
</div>

<div class="cards-grid">
  <div class="fact-card">
    <div class="icon-badge">🎓</div>
    <h3>Degree</h3>
    <p>BS Computer Engineering</p>
  </div>
  <div class="fact-card">
    <div class="icon-badge">🏛️</div>
    <h3>University</h3>
    <p>UET Faisalabad</p>
  </div>
  <div class="fact-card">
    <div class="icon-badge">🏙️</div>
    <h3>Home City</h3>
    <p>Lahore</p>
  </div>
</div>
