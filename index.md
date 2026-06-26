---
layout: home
---

<style>
  .site-header, .page-header { display: none !important; }
  .page-content { padding: 0 !important; }
  .wrapper { max-width: 100% !important; padding: 0 !important; }

  .gn-wrap {
    background: #f4f6f9;
    border-radius: 14px;
    overflow: hidden;
    padding: 20px 18px;
    font-family: 'Poppins', sans-serif;
    max-width: 780px;
    margin: 20px auto;
  }

  .gn-hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #fff;
    border-radius: 14px;
    padding: 22px 26px;
    margin-bottom: 24px;
    box-shadow: 0 3px 12px rgba(0,0,0,0.06);
    gap: 20px;
  }

  .gn-left {
    display: flex;
    align-items: center;
    gap: 18px;
    flex: 1;
  }

  .gn-left img {
    width: 78px;
    height: 78px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid #e94560;
    flex-shrink: 0;
  }

  .gn-left h1 {
    font-size: 19px;
    font-weight: 700;
    color: #1a1a2e;
    margin: 0 0 4px;
  }

  .gn-left p {
    font-size: 12px;
    color: #888;
    margin: 0;
  }

  .gn-navgrid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px 24px;
  }

  .gn-link {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 4px;
    text-decoration: none;
    cursor: pointer;
  }

  .gn-ic { font-size: 22px; }

  .gn-link .lbl {
    font-size: 10px;
    color: #1a1a2e;
    font-weight: 700;
    white-space: nowrap;
  }

  .gn-label {
    text-align: center;
    margin: 0 0 16px;
  }

  .gn-label .eyebrow {
    display: block;
    font-size: 11px;
    color: #888;
    margin-bottom: 3px;
    letter-spacing: 1px;
    text-transform: uppercase;
  }

  .gn-label h2 {
    font-size: 18px;
    color: #1a1a2e;
    margin: 0;
    font-weight: 700;
  }

  .gn-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
    margin-bottom: 12px;
  }

  .gn-card {
    background: #fff;
    border-radius: 10px;
    padding: 14px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.06);
    border-left: 4px solid #e94560;
  }

  .gn-card-head {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 6px;
    margin-bottom: 9px;
  }

  .gn-card-head h3 {
    font-size: 12px;
    color: #1a1a2e;
    margin: 0;
    font-weight: 700;
  }

  .gn-card-head .ic { font-size: 15px; }

  .gn-card p {
    font-size: 9.5px;
    line-height: 1.5;
    color: #555;
    margin: 0;
  }

  .gn-card ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .gn-card ul li {
    font-size: 9px;
    line-height: 1.5;
    color: #555;
    padding-left: 10px;
    position: relative;
    margin-bottom: 2px;
  }

  .gn-card ul li::before {
    content: "";
    position: absolute;
    left: 0;
    top: 6px;
    width: 4px;
    height: 4px;
    border-radius: 50%;
    background: #e94560;
  }

  .gn-fact .gn-card-head h3 {
    font-size: 10px;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    color: #aaa;
    font-weight: 600;
  }

  .gn-fact p {
    font-size: 13px !important;
    font-weight: 700;
    color: #1a1a2e !important;
  }

  @media (max-width: 560px) {
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
        <p>Computer Engineering Student</p>
      </div>
    </div>
    <div class="gn-navgrid">
      <a href="/myjourney/" class="gn-link"><span class="gn-ic">📖</span><span class="lbl">My Journey</span></a>
      <a href="/about/" class="gn-link"><span class="gn-ic">👤</span><span class="lbl">About Me</span></a>
      <a href="/contact/" class="gn-link"><span class="gn-ic">✉️</span><span class="lbl">Contact Me</span></a>
      <a href="#" class="gn-link" onclick="document.body.classList.toggle('dark-mode');return false;"><span class="gn-ic">🌙</span><span class="lbl">Theme</span></a>
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

  <div class="gn-grid" style="margin-bottom:0;">
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
