---
layout: default
title: Home
---
{% include theme-toggle.html %}

<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600;700&display=swap');

  .hero {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 18px;
    padding: 50px;
    margin-bottom: 45px;
    overflow: hidden;
    position: relative;
    display: flex;
    align-items: center;
    gap: 40px;
  }
  .hero::before {
    content: "";
    position: absolute;
    top: -60px; right: -60px;
    width: 220px; height: 220px;
    background: radial-gradient(circle, rgba(233,69,96,0.25), transparent 70%);
    pointer-events: none;
  }
  .hero-pic {
    flex-shrink: 0;
    width: 140px; height: 140px;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid #e94560;
    position: relative; z-index: 1;
  }
  .hero-text { position: relative; z-index: 1; }
  .hero-text h1 {
    font-family: 'Poppins', sans-serif;
    font-size: 34px; font-weight: 700;
    margin: 0 0 8px 0; color: white;
  }
  .hero-text p { font-size: 16px; color: #aaa; margin: 0; }

  .section-label { text-align: center; margin: 0 0 22px; }
  .section-label .eyebrow {
    display: block; font-size: 12px; font-weight: 700;
    letter-spacing: 1.5px; text-transform: uppercase;
    color: #e94560; margin-bottom: 6px;
  }
  .section-label h2 {
    font-family: 'Poppins', sans-serif;
    font-size: 22px; color: #1a1a2e; margin: 0;
  }

  .cards-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
    max-width: 1050px;
    margin: 0 auto 50px;
  }

  .highlight-card {
    background: white; border-radius: 14px;
    padding: 28px 24px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.06);
    border-left: 5px solid #e94560;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
  }
  .highlight-card:hover { transform: translateY(-6px); box-shadow: 0 10px 24px rgba(0,0,0,0.1); }
  .icon-badge {
    width: 48px; height: 48px; border-radius: 12px;
    background: rgba(233,69,96,0.1);
    display: flex; align-items: center; justify-content: center;
    font-size: 22px; margin-bottom: 16px;
  }
  .highlight-card h3 { font-family: 'Poppins', sans-serif; font-size: 16px; color: #1a1a2e; margin: 0 0 10px; }
  .highlight-card p { font-size: 14px; line-height: 1.7; color: #555; margin: 0; text-align: left; word-spacing: normal; letter-spacing: normal; }
  .highlight-card ul { margin: 0; padding-left: 0; list-style: none; }
  .highlight-card ul li {
    font-size: 14px; line-height: 1.7; color: #555;
    padding-left: 18px; position: relative;
    margin-bottom: 4px; text-align: left;
    word-spacing: normal; letter-spacing: normal;
  }
  .highlight-card ul li::before {
    content: ""; position: absolute; left: 0; top: 9px;
    width: 6px; height: 6px; border-radius: 50%; background: #e94560;
  }

  .fact-card {
    background: white; border-radius: 14px;
    padding: 26px 16px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.06);
    border-left: 5px solid #e94560;
    display: flex; flex-direction: column;
    align-items: center; justify-content: center;
    text-align: center; min-height: 150px;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
  }
  .fact-card:hover { transform: translateY(-6px); box-shadow: 0 10px 24px rgba(0,0,0,0.1); }
  .fact-card .icon-badge { width: 52px; height: 52px; border-radius: 50%; margin-bottom: 14px; font-size: 24px; }
  .fact-card h3 { font-size: 12px; color: #999; margin: 0 0 6px; font-weight: 600; text-transform: uppercase; letter-spacing: 0.6px; }
  .fact-card p { font-size: 15px; font-weight: 700; color: #1a1a2e; margin: 0; line-height: 1.4; word-spacing: normal; letter-spacing: normal; }

  /* Theme toggle in nav */
  .theme-toggle-wrap {
    display: inline-flex;
    align-items: center;
    margin-left: 8px;
  }

  header h1 { display: none; }

  @media (max-width: 768px) {
    .hero { flex-direction: column; text-align: center; padding: 40px 20px; }
    .cards-grid { grid-template-columns: 1fr; padding: 0 10px; }
    .fact-card { min-height: auto; }
  }
</style>

<!-- Theme Toggle Button (added next to nav) -->
<div style="position: fixed; top: 14px; right: 20px; z-index: 9999;">
  <button class="theme-toggle-btn" onclick="toggleTheme()" title="Toggle Theme">
    <i id="theme-icon" class="fa-regular fa-moon"></i>
    <span id="theme-label">Theme</span>
  </button>
</div>

<div class="hero">
  <img class="hero-pic" src="/assets/images/mohsin.jpg.jpeg" alt="Mohsin Riaz">
  <div class="hero-text">
    <h1>Mohsin Riaz</h1>
    <p>Computer Engineering Student</p>
  </div>
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
