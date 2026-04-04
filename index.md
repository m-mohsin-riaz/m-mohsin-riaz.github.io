---
layout: default
title: Home
---

<style>
  .hero {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 15px;
    padding: 60px 40px;
    text-align: center;
    margin-bottom: 40px;
  }
  .hero img {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid #e94560;
    margin-bottom: 15px;
  }
  .hero h1 { font-size: 36px; margin-bottom: 10px; }
  .hero p { font-size: 18px; color: #aaa; margin-bottom: 5px; }
  .info-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
  }
  .card {
    background: white;
    border-radius: 12px;
    padding: 25px;
    box-shadow: 0 3px 15px rgba(0,0,0,0.08);
    border-left: 4px solid #e94560;
    text-align: center;
  }
  .card .icon { font-size: 30px; margin-bottom: 10px; }
  .card h3 { font-size: 14px; color: #888; margin-bottom: 5px; }
  .card p { font-size: 14px; font-weight: bold; color: #1a1a2e; }
</style>

<div class="hero">
  <img src="/assets/images/WhatsApp Image 2026-04-05 at 2.59.39 AM.jpeg" alt="Mohsin Riaz">
  <h1>Mohsin Riaz</h1>
  <p>Computer Engineering Student</p>
  <p>University of Engineering & Technology (UET) Faisalabad</p>
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
