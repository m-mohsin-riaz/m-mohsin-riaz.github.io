---
layout: default
title: Home
---

<style>
  /* Hero Section Styling */
  .hero {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 15px;
    padding: 60px 20px;
    text-align: center;
    margin-bottom: 40px;
    overflow: hidden;
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
  }

  .hero h1 { 
    font-size: 32px; 
    margin-bottom: 10px; 
    font-weight: 700;
  }

  .hero p { 
    font-size: 16px; 
    color: #aaa; 
    margin-bottom: 5px; 
  }

  /* Info Cards Grid */
  .info-cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 15px;
    max-width: 1000px;
    margin: 0 auto;
  }

  /* Card Fixes */
  .card {
    background: white;
    border-radius: 12px;
    padding: 25px 15px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.06);
    border-left: 5px solid #e94560;
    display: flex;
    flex-direction: column;
    align-items: center; /* Horizontally center */
    justify-content: center; /* Vertically center */
    text-align: center;
    min-height: 140px;
    transition: transform 0.3s ease;
  }

  .card:hover {
    transform: translateY(-5px);
  }

  /* Icon and Text Alignment */
  .card .icon { 
    font-size: 30px; 
    margin-bottom: 12px; 
    line-height: 1;
  }

  .card h3 { 
    font-size: 13px; 
    color: #888; 
    margin: 0 0 6px 0; 
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .card p { 
    font-size: 14px; 
    font-weight: 700; 
    color: #1a1a2e; 
    margin: 0; 
    line-height: 1.4;
  }

  /* Mobile Responsive Fix */
  @media (max-width: 768px) {
    .info-cards {
      grid-template-columns: 1fr;
      padding: 0 10px;
    }
    .card {
      min-height: auto;
      padding: 20px;
    }
  }
</style>

<div class="hero">
  <img src="/assets/images/mohsin.jpg.jpeg" alt="Mohsin Riaz">
  <h1>Mohsin Riaz</h1>
  <p>Computer Engineering Student</p>
  <p>UET Faisalabad</p>
</div>

<div class="info-cards">
  <div class="card">
    <div class="icon">🎓</div>
    <h3>Degree</h3>
    <p>BS Computer Engineering</p>
  </div>

  <div class="card">
    <div class="icon">🏛️</div>
    <h3>University</h3>
    <p>UET Faisalabad</p>
  </div>

  <div class="card">
    <div class="icon">🏙️</div>
    <h3>Home City</h3>
    <p>Lahore</p>
  </div>
</div>
