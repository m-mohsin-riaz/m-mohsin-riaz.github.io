---
layout: default
title: About
---
<style>
  /* Header */
  .about-header {
    background: linear-gradient(135deg, #4f46e5, #6366f1);
    color: white;
    border-radius: 15px;
    padding: 50px 30px;
    margin-bottom: 30px;
    text-align: center;
  }
  .about-header h1 {
    font-size: 36px;
    font-weight: 800;
    margin: 0 0 10px 0;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 12px;
  }
  .about-header h1 span.me { color: #c7c2ff; }

  /* Intro */
  .intro-card {
    background: white;
    border-radius: 14px;
    padding: 36px;
    margin-bottom: 24px;
    box-shadow: 0 3px 16px rgba(0,0,0,0.07);
    display: flex;
    align-items: flex-start;
    gap: 28px;
  }
  .intro-avatar { font-size: 64px; flex-shrink: 0; line-height: 1; }
  .intro-card h2 { font-size: 24px; font-weight: 800; margin: 0 0 14px 0; color: #1a1a2e; }
  .intro-card h2 span { color: #4f46e5; }
  .intro-card p { font-size: 15px; color: #555; line-height: 1.8; margin: 0 0 12px 0; text-align: left; word-spacing: normal; letter-spacing: normal; }
  .intro-card p:last-child { margin: 0; }
  .intro-card strong { color: #1a1a2e; }

  /* Info Grid */
  .info-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin-bottom: 30px;
  }
  .info-tile {
    background: white;
    border-radius: 12px;
    padding: 20px 18px;
    box-shadow: 0 3px 14px rgba(0,0,0,0.06);
    border-left: 4px solid #4f46e5;
    display: flex;
    align-items: center;
    gap: 14px;
    min-width: 0;
  }
  .info-tile .tile-icon { font-size: 32px; flex-shrink: 0; line-height: 1; }
  .info-tile .tile-text { min-width: 0; }
  .info-tile .tile-label {
    font-size: 11px;
    font-weight: 600;
    color: #888;
    letter-spacing: 1px;
    text-transform: uppercase;
    margin: 0 0 4px 0;
    white-space: nowrap;
  }
  .info-tile .tile-value {
    font-size: 14px;
    font-weight: 700;
    color: #1a1a2e;
    margin: 0;
    line-height: 1.3;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .tile-value.open { color: #16a34a; }

  /* Section Heading - FORCED LEFT ALIGNED */
  .section-heading {
    font-size: 22px !important;
    font-weight: 800 !important;
    color: #1a1a2e !important;
    margin: 0 0 6px 0 !important;
    display: flex !important;
    align-items: center !important;
    gap: 10px !important;
    text-align: left !important;
    justify-content: flex-start !important;
    width: 100% !important;
  }
  .section-divider {
    border: none;
    border-top: 2px solid #e5e7eb;
    margin: 0 0 20px 0;
  }

  /* Education */
  .edu-wrap {
    background: white;
    border-radius: 14px;
    padding: 28px 32px;
    margin-bottom: 28px;
    box-shadow: 0 3px 16px rgba(0,0,0,0.07);
  }
  .edu-entry {
    display: flex;
    align-items: flex-start;
    gap: 20px;
    padding: 20px 0;
    border-bottom: 1px solid #f0f0f0;
  }
  .edu-entry:last-child { border-bottom: none; padding-bottom: 0; }
  .edu-entry:first-child { padding-top: 0; }
  .edu-icon { font-size: 44px; flex-shrink: 0; line-height: 1; }
  .edu-entry h3 { font-size: 17px; font-weight: 800; color: #1a1a2e; margin: 0 0 4px 0; text-align: left; }
  .edu-entry .edu-inst { color: #4f46e5; font-size: 14px; font-weight: 600; margin: 0 0 4px 0; text-align: left; }
  .edu-entry .edu-meta { color: #888; font-size: 13px; margin: 0; text-align: left; word-spacing: normal; letter-spacing: normal; }

  /* Skills */
  .skills-wrap {
    background: white;
    border-radius: 14px;
    padding: 28px 32px;
    margin-bottom: 28px;
    box-shadow: 0 3px 16px rgba(0,0,0,0.07);
  }
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 14px;
  }
  .skill-card {
    background: #f8f7ff;
    border-radius: 12px;
    padding: 22px 12px 18px;
    border-top: 3px solid #4f46e5;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 10px;
    transition: transform 0.2s;
  }
  .skill-card:hover { transform: translateY(-4px); }
  .skill-card .sk-icon { font-size: 38px; line-height: 1; }
  .skill-card .sk-name { font-size: 13px; font-weight: 600; color: #1a1a2e; margin: 0; }

  /* Journey */
  .journey-wrap {
    background: white;
    border-radius: 14px;
    padding: 28px 32px;
    margin-bottom: 24px;
    box-shadow: 0 3px 16px rgba(0,0,0,0.07);
  }
  .journey-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
  }
  .journey-card {
    background: #f8f7ff;
    border-radius: 12px;
    padding: 28px 18px 24px;
    text-align: center;
    transition: transform 0.2s;
  }
  .journey-card:hover { transform: translateY(-4px); }
  .journey-card .jc-icon { font-size: 46px; line-height: 1; margin-bottom: 14px; display: block; }
  .journey-card h3 { font-size: 16px; font-weight: 700; color: #4f46e5; margin: 0 0 10px 0; }
  .journey-card p { font-size: 13px; color: #666; line-height: 1.7; margin: 0; text-align: center; word-spacing: normal; letter-spacing: normal; }

  @media (max-width: 820px) {
    .info-grid { grid-template-columns: repeat(2, 1fr); }
    .skills-grid { grid-template-columns: repeat(3, 1fr); }
    .journey-grid { grid-template-columns: 1fr; }
    .intro-card { flex-direction: column; align-items: center; text-align: center; }
  }
  @media (max-width: 520px) {
    .info-grid { grid-template-columns: 1fr; }
    .skills-grid { grid-template-columns: repeat(2, 1fr); }
    .info-tile .tile-value { white-space: normal; }
  }
</style>

<!-- Header -->
<div class="about-header">
  <h1>👤 About <span class="me">Me</span></h1>
</div>

<!-- Intro -->
<div class="intro-card">
  <div class="intro-avatar">👋🏼</div>
  <div>
    <h2>Hi, I'm <span>Mohsin Riaz</span></h2>
    <p>A <strong>Computer Engineering student</strong> from Lahore, Pakistan. I love building clean websites and sharing my real life experiences through writing.</p>
    <p>I came to university leaving my comfort zone behind — facing nervousness, distance from home, and many unexpected challenges. But every difficulty taught me something new about patience, resilience, and growth.</p>
    <p>When I'm not coding, I'm writing about my <strong>university journey</strong> — the friendships, the tough weeks, the exams, and everything in between. Real stories, real emotions.</p>
  </div>
</div>

<!-- Info Tiles -->
<div class="info-grid">
  <div class="info-tile">
    <span class="tile-icon">🎓</span>
    <div class="tile-text">
      <p class="tile-label">University</p>
      <p class="tile-value">UET Faisalabad</p>
    </div>
  </div>
  <div class="info-tile">
    <span class="tile-icon">📚</span>
    <div class="tile-text">
      <p class="tile-label">Degree</p>
      <p class="tile-value">BS Computer Engg.</p>
    </div>
  </div>
  <div class="info-tile">
    <span class="tile-icon">📋</span>
    <div class="tile-text">
      <p class="tile-label">Registration No</p>
      <p class="tile-value">2025-BSCPE-110</p>
    </div>
  </div>
  <div class="info-tile">
    <span class="tile-icon">📅</span>
    <div class="tile-text">
      <p class="tile-label">Semester</p>
      <p class="tile-value">Semester 2 — 2026</p>
    </div>
  </div>
  <div class="info-tile">
    <span class="tile-icon">📍</span>
    <div class="tile-text">
      <p class="tile-label">Location</p>
      <p class="tile-value">Lahore, Pakistan</p>
    </div>
  </div>
  <div class="info-tile">
    <span class="tile-icon">💼</span>
    <div class="tile-text">
      <p class="tile-label">Status</p>
      <p class="tile-value open">Open to Work ✅</p>
    </div>
  </div>
</div>

<!-- Education -->
<h2 class="section-heading">🎓 Education</h2>
<hr class="section-divider">
<div class="edu-wrap">
  <div class="edu-entry">
    <span class="edu-icon">📘</span>
    <div>
      <h3>Matric — Computer Science</h3>
      <p class="edu-inst">Secondary School Certificate</p>
      <p class="edu-meta">Completed | Board of Intermediate &amp; Secondary Education</p>
    </div>
  </div>
  <div class="edu-entry">
    <span class="edu-icon">📗</span>
    <div>
      <h3>Intermediate — ICS (Inter with Computer Science)</h3>
      <p class="edu-inst">Higher Secondary School Certificate</p>
      <p class="edu-meta">Completed | Board of Intermediate &amp; Secondary Education</p>
    </div>
  </div>
  <div class="edu-entry">
    <span class="edu-icon">🏛️</span>
    <div>
      <h3>BS Computer Engineering</h3>
      <p class="edu-inst">University of Engineering &amp; Technology, Faisalabad</p>
      <p class="edu-meta">2025 — Present &nbsp;|&nbsp; Semester 2 &nbsp;|&nbsp; Reg: 2025-BSCPE-110</p>
    </div>
  </div>
</div>

<!-- Skills -->
<h2 class="section-heading">⚡ Skills</h2>
<hr class="section-divider">
<div class="skills-wrap">
  <div class="skills-grid">
    <div class="skill-card">
      <span class="sk-icon">🌐</span>
      <p class="sk-name">HTML &amp; CSS</p>
    </div>
    <div class="skill-card">
      <span class="sk-icon">⚙️</span>
      <p class="sk-name">JavaScript</p>
    </div>
    <div class="skill-card">
      <span class="sk-icon">💎</span>
      <p class="sk-name">Jekyll</p>
    </div>
    <div class="skill-card">
      <span class="sk-icon">🐙</span>
      <p class="sk-name">Git &amp; GitHub</p>
    </div>
    <div class="skill-card">
      <span class="sk-icon">💻</span>
      <p class="sk-name">C++</p>
    </div>
    <div class="skill-card">
      <span class="sk-icon">🐍</span>
      <p class="sk-name">Python</p>
    </div>
    <div class="skill-card">
      <span class="sk-icon">🗄️</span>
      <p class="sk-name">MySQL</p>
    </div>
    <div class="skill-card">
      <span class="sk-icon">🤖</span>
      <p class="sk-name">Machine Learning</p>
    </div>
  </div>
</div>

<!-- My Journey -->
<h2 class="section-heading">🗺️ My Journey</h2>
<hr class="section-divider">
<div class="journey-wrap">
  <div class="journey-grid">
    <div class="journey-card">
      <span class="jc-icon">🏫</span>
      <h3>University Life</h3>
      <p>Left home, faced challenges, made lifelong friends in a hostel I never expected to love.</p>
    </div>
    <div class="journey-card">
      <span class="jc-icon">💻</span>
      <h3>Coder &amp; Builder</h3>
      <p>Building real projects while managing semester pressure, exams, and online classes.</p>
    </div>
    <div class="journey-card">
      <span class="jc-icon">✍️</span>
      <h3>Writer &amp; Blogger</h3>
      <p>Sharing honest stories about student life — the good, the bad, and everything in between.</p>
    </div>
  </div>
</div>
