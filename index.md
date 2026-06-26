<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mohsin Riaz – Computer Engineering Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Inter:wght@400;500&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Inter', sans-serif;
      background: #f4f6f9;
      min-height: 100vh;
      display: flex;
      align-items: flex-start;
      justify-content: center;
      padding: 32px 16px;
    }

    .wrapper {
      width: 100%;
      max-width: 780px;
    }

    /* ── Hero Card ── */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: #fff;
      border-radius: 16px;
      padding: 22px 28px;
      margin-bottom: 20px;
      box-shadow: 0 4px 16px rgba(0,0,0,0.07);
      gap: 20px;
    }

    .hero-left {
      display: flex;
      align-items: center;
      gap: 18px;
      flex: 1;
    }

    .hero-left img {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #e94560;
      flex-shrink: 0;
    }

    .hero-left h1 {
      font-family: 'Poppins', sans-serif;
      font-size: 20px;
      font-weight: 700;
      color: #1a1a2e;
      margin-bottom: 3px;
    }

    .hero-left p {
      font-size: 12px;
      color: #888;
    }

    /* 2×2 Nav Grid */
    .nav-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px 24px;
    }

    .nav-item {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 4px;
      cursor: pointer;
      text-decoration: none;
    }

    .nav-item:hover .nav-icon { transform: scale(1.15); }

    .nav-icon {
      font-size: 22px;
      transition: transform 0.2s ease;
    }

    .nav-label {
      font-size: 10px;
      font-weight: 700;
      color: #1a1a2e;
      white-space: nowrap;
    }

    /* ── Section Header ── */
    .section-header {
      text-align: center;
      margin: 8px 0 16px;
    }

    .section-header .eyebrow {
      display: block;
      font-size: 11px;
      letter-spacing: 1px;
      text-transform: uppercase;
      color: #888;
      margin-bottom: 4px;
    }

    .section-header h2 {
      font-family: 'Poppins', sans-serif;
      font-size: 19px;
      font-weight: 700;
      color: #1a1a2e;
    }

    /* ── Card Grid ── */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
      margin-bottom: 12px;
    }

    .card {
      background: #fff;
      border-radius: 12px;
      padding: 16px;
      box-shadow: 0 3px 12px rgba(0,0,0,0.06);
      border-left: 4px solid #e94560;
    }

    .card-head {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 10px;
    }

    .card-head h3 {
      font-family: 'Poppins', sans-serif;
      font-size: 12.5px;
      font-weight: 700;
      color: #1a1a2e;
    }

    .card-head .icon {
      font-size: 16px;
    }

    .card p {
      font-size: 10px;
      line-height: 1.6;
      color: #555;
    }

    .card ul {
      list-style: none;
      padding: 0;
    }

    .card ul li {
      font-size: 10px;
      line-height: 1.6;
      color: #555;
      padding-left: 12px;
      position: relative;
      margin-bottom: 2px;
    }

    .card ul li::before {
      content: '';
      position: absolute;
      left: 0;
      top: 7px;
      width: 5px;
      height: 5px;
      border-radius: 50%;
      background: #e94560;
    }

    /* Fact cards */
    .card.fact .card-head h3 {
      font-size: 10px;
      text-transform: uppercase;
      letter-spacing: 0.6px;
      color: #aaa;
      font-weight: 600;
    }

    .card.fact p {
      font-size: 13px;
      font-weight: 700;
      color: #1a1a2e;
    }

    /* ── Responsive ── */
    @media (max-width: 560px) {
      .hero { flex-direction: column; align-items: flex-start; }
      .nav-grid { width: 100%; }
      .card-grid { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <div class="wrapper">

    <!-- Hero / Nav Bar -->
    <div class="hero">
      <div class="hero-left">
        <img src="https://m-mohsin-riaz.github.io/assets/images/mohsin.jpg.jpeg" alt="Mohsin Riaz">
        <div>
          <h1>Mohsin Riaz</h1>
          <p>Computer Engineering Student</p>
        </div>
      </div>
      <nav class="nav-grid" aria-label="Main navigation">
        <a href="#journey" class="nav-item">
          <span class="nav-icon">📖</span>
          <span class="nav-label">My Journey</span>
        </a>
        <a href="#about" class="nav-item">
          <span class="nav-icon">👤</span>
          <span class="nav-label">About Me</span>
        </a>
        <a href="#contact" class="nav-item">
          <span class="nav-icon">✉️</span>
          <span class="nav-label">Contact Me</span>
        </a>
        <a href="#" class="nav-item" id="theme-toggle" onclick="toggleTheme(event)">
          <span class="nav-icon" id="theme-icon">🌙</span>
          <span class="nav-label">Theme</span>
        </a>
      </nav>
    </div>

    <!-- Section Header -->
    <div class="section-header">
      <span class="eyebrow">Overview</span>
      <h2>Professional Profile</h2>
    </div>

    <!-- Info Cards Row 1 -->
    <div class="card-grid">
      <div class="card">
        <div class="card-head">
          <h3>Professional Profile</h3>
          <span class="icon">🧑‍💻</span>
        </div>
        <p>Welcome to my official academic portfolio documenting my 8-semester journey in Computer Engineering.</p>
      </div>
      <div class="card">
        <div class="card-head">
          <h3>Current Focus</h3>
          <span class="icon">🎯</span>
        </div>
        <ul>
          <li>Programming Fundamentals</li>
          <li>Database Management</li>
          <li>C++, MySQL, GitHub, Jekyll</li>
        </ul>
      </div>
      <div class="card">
        <div class="card-head">
          <h3>Objective</h3>
          <span class="icon">🏆</span>
        </div>
        <p>Build a comprehensive repository of academic projects across all 8 semesters.</p>
      </div>
    </div>

    <!-- Fact Cards Row 2 -->
    <div class="card-grid">
      <div class="card fact">
        <div class="card-head">
          <h3>Degree</h3>
          <span class="icon">🎓</span>
        </div>
        <p>BS Computer Engineering</p>
      </div>
      <div class="card fact">
        <div class="card-head">
          <h3>University</h3>
          <span class="icon">🏛️</span>
        </div>
        <p>UET Faisalabad</p>
      </div>
      <div class="card fact">
        <div class="card-head">
          <h3>Home City</h3>
          <span class="icon">🏙️</span>
        </div>
        <p>Lahore</p>
      </div>
    </div>

  </div>

  <script>
    function toggleTheme(e) {
      e.preventDefault();
      const isDark = document.body.classList.toggle('dark');
      document.getElementById('theme-icon').textContent = isDark ? '☀️' : '🌙';
    }

    // Dark mode styles injected via JS to keep HTML clean
    const darkCSS = `
      body.dark { background: #12111a; }
      body.dark .hero,
      body.dark .card { background: #1e1d2e; box-shadow: 0 3px 12px rgba(0,0,0,0.3); }
      body.dark .hero-left h1,
      body.dark .card-head h3,
      body.dark .card.fact p,
      body.dark .nav-label,
      body.dark .section-header h2 { color: #f0f0f0; }
      body.dark .card p,
      body.dark .card ul li { color: #aaa; }
      body.dark .section-header .eyebrow { color: #666; }
      body.dark .card.fact .card-head h3 { color: #666; }
    `;
    const style = document.createElement('style');
    style.textContent = darkCSS;
    document.head.appendChild(style);
  </script>
</body>
</html>
