---
layout: default
title: Home
---
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600;700&display=swap');

  /* ============ Top Navigation: 2x2 icon grid, right side of header ============
     Matches the real "contrast" theme markup (header.hover.smooth > h1 + nav).
     The theme already places h1 on the left and nav on the right (flex,
     justify-content: space-between). We just grid the nav into 2 columns. */
  header.hover.smooth h1 {
    font-size: 18px;
  }
  header.hover.smooth nav {
    display: grid;
    grid-template-columns: repeat(2, auto);
    gap: 8px 28px;
    margin: 0.5em 0;
  }
  header.hover.smooth nav a {
    display: flex !important;
    flex-direction: column;
    align-items: center;
    gap: 4px;
    margin: 0 !important;
  }
  header.hover.smooth nav a svg {
    width: 24px;
    height: 24px;
    color: #1a1a2e;
  }
  header.hover.smooth nav a:hover svg {
    color: #e94560;
  }
  header.hover.smooth nav a span.nav-label {
    font-size: 11px;
    font-weight: 700;
  }

  /* ============ Hero Section: photo left, text right ============ */
  .hero-flex {
    display: flex;
    align-items: center;
    gap: 30px;
    background: #fff;
    border-radius: 16px;
    padding: 32px 36px;
    margin-bottom: 40px;
    box-shadow: 0 3px 15px rgba(0,0,0,0.06);
  }
  .hero-flex img {
    width: 130px;
    height: 130px;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid #e94560;
    flex-shrink: 0;
  }
  .hero-flex h1 {
    font-family: 'Poppins', sans-serif;
    font-size: 30px;
    font-weight: 700;
    color: #1a1a2e;
    margin: 0 0 6px;
  }
  .hero-flex p {
    font-size: 16px;
    color: #888;
    margin: 0;
  }

  /* ============ Section Labels ============ */
  .section-label {
    text-align: center;
    margin: 0 0 26px;
  }
  .section-label .eyebrow {
    display: block;
    font-size: 14px;
    color: #888;
    margin-bottom: 4px;
  }
  .section-label h2 {
    font-family: 'Poppins', sans-serif;
    font-size: 26px;
    color: #1a1a2e;
    margin: 0;
    font-weight: 700;
  }

  /* ============ Shared Card Grid ============ */
  .cards-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
    max-width: 1050px;
    margin: 0 auto 18px;
  }

  /* ============ Highlight Cards (Profile / Focus / Objective) ============ */
  .highlight-card {
    background: white;
    border-radius: 14px;
    padding: 24px 22px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.06);
    border-left: 5px solid #e94560;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
  }
  .highlight-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 24px rgba(0,0,0,0.1);
  }
  .card-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;
    margin-bottom: 12px;
  }
  .card-header h3 {
    font-family: 'Poppins', sans-serif;
    font-size: 17px;
    color: #1a1a2e;
    margin: 0;
  }
  .card-header .icon-glyph {
    font-size: 24px;
    flex-shrink: 0;
  }
  .highlight-card p {
    font-size: 14px;
    line-height: 1.7;
    color: #555;
    margin: 0;
    text-align: left;
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
    text-align: left;
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
    padding: 22px 20px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.06);
    border-left: 5px solid #e94560;
    text-align: left;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
  }
  .fact-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 24px rgba(0,0,0,0.1);
  }
  .fact-card .card-header h3 {
    font-size: 13px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.6px;
    color: #1a1a2e;
  }
  .fact-card .card-header .icon-glyph {
    font-size: 22px;
  }
  .fact-card p {
    font-size: 15px;
    font-weight: 600;
    color: #555;
    margin: 0;
  }

  /* ============ Mobile Responsive ============ */
  @media (max-width: 768px) {
    .hero-flex {
      flex-direction: column;
      text-align: center;
      padding: 28px 20px;
    }
    .cards-grid {
      grid-template-columns: 1fr;
      padding: 0 10px;
    }
  }
</style>

<div class="hero-flex">
  <img src="/assets/images/mohsin.jpg.jpeg" alt="Mohsin Riaz">
  <div>
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
    <div class="card-header">
      <h3>Professional Profile</h3>
      <span class="icon-glyph">🧑‍💻</span>
    </div>
    <p>Welcome to my official academic portfolio. This platform documents my 8-semester journey in Computer Engineering, focusing on technical excellence and structured learning.</p>
  </div>
  <div class="highlight-card">
    <div class="card-header">
      <h3>Current Focus</h3>
      <span class="icon-glyph">🎯</span>
    </div>
    <ul>
      <li>Programming Fundamentals</li>
      <li>Database Management Systems</li>
      <li>Technical Stack: C++, MySQL, GitHub, Jekyll</li>
    </ul>
  </div>
  <div class="highlight-card">
    <div class="card-header">
      <h3>Objective</h3>
      <span class="icon-glyph">🏆</span>
    </div>
    <p>To build a comprehensive repository of academic projects and lab implementations across all 8 semesters of Computer Engineering.</p>
  </div>
</div>

<div class="cards-grid">
  <div class="fact-card">
    <div class="card-header">
      <h3>Degree</h3>
      <span class="icon-glyph">🎓</span>
    </div>
    <p>BS Computer Engineering</p>
  </div>
  <div class="fact-card">
    <div class="card-header">
      <h3>University</h3>
      <span class="icon-glyph">🏛️</span>
    </div>
    <p>UET Faisalabad</p>
  </div>
  <div class="fact-card">
    <div class="card-header">
      <h3>Home City</h3>
      <span class="icon-glyph">🏙️</span>
    </div>
    <p>Lahore</p>
  </div>
</div>
