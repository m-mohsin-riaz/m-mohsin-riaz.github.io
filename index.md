---
layout: default
title: Home
---

<style>
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
  .hero h1 { font-size: 32px; margin-bottom: 10px; }
  .hero p { font-size: 16px; color: #aaa; margin-bottom: 5px; }
  .info-cards {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 15px;
  }
  .card {
    background: white;
    border-radius: 12px;
    padding: 20px 10px;
    box-shadow: 0 3px 15px rgba(0,0,0,0.08);
    border-left: 4px solid #e94560;
    text-align: center;
  }
  .card .icon { font-size: 26px; margin-bottom: 8px; }
  .card h3 { font-size: 12px; color: #888; margin-bottom: 5px; }
  .card p { font-size: 12px; font-weight: bold; color: #1a1a2e; margin: 0; }
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
