---
layout: default
title: Contact
---

<style>
  /* Header Section */
  .contact-header {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 15px;
    padding: 50px 20px;
    margin-bottom: 40px;
    text-align: center;
  }
  .contact-header h1 { font-size: 32px; margin: 0 0 10px 0; }
  .contact-header p { color: #aaa; font-size: 16px; margin: 0; }

  /* Grid Layout Fix */
  .contact-cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* Computer par 3 cards barabar */
    gap: 20px;
    max-width: 1100px;
    margin: 0 auto;
    padding: 10px;
  }

  /* Card Styling - Perfect Alignment */
  .contact-card {
    background: white;
    border-radius: 12px;
    padding: 40px 10px; /* Top/Bottom padding zyada ki hai */
    box-shadow: 0 4px 15px rgba(0,0,0,0.06);
    border-bottom: 4px solid transparent;
    display: flex;
    flex-direction: column;
    align-items: center; /* Horizontally center */
    justify-content: center; /* Vertically center */
    text-align: center;
    min-height: 200px; /* Height fix kar di taaki sab ek line mein hon */
    transition: all 0.3s ease;
    box-sizing: border-box;
  }

  .contact-card:hover {
    transform: translateY(-8px);
    border-bottom: 4px solid #e94560;
  }

  /* Icon Style */
  .contact-card .icon { 
    font-size: 45px; 
    margin-bottom: 15px; 
    display: block;
    line-height: 1;
  }

  /* Heading (Email, GitHub etc) */
  .contact-card h3 { 
    font-size: 13px; 
    color: #888; 
    margin: 0 0 12px 0; 
    font-weight: 500;
    letter-spacing: 0.5px;
  }

  /* Text & Links Style */
  .contact-card p, .contact-card a { 
    font-size: 14px; 
    font-weight: 700; 
    margin: 0; 
    color: #1a1a2e;
    text-decoration: none;
    line-height: 1.2;
    word-wrap: break-word;
    max-width: 100%;
  }

  /* Link Color */
  .contact-card a { color: #e94560; }

  /* Mobile Responsive - 1 Card per row */
  @media (max-width: 800px) {
    .contact-cards {
      grid-template-columns: repeat(2, 1fr);
    }
  }
  @media (max-width: 500px) {
    .contact-cards {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="contact-header">
  <h1>Contact Me</h1>
  <p>I'm always open to discussing new projects or opportunities.</p>
</div>

<div class="contact-cards">
  <div class="contact-card">
    <div class="icon">📧</div>
    <h3>Email</h3>
    <p><a href="mailto:wmohsinriaz@gmail.com">wmohsinriaz@gmail.com</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">🐙</div>
    <h3>GitHub</h3>
    <p><a href="https://github.com/m-mohsin-riaz" target="_blank">m-mohsin-riaz</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">💬</div>
    <h3>WhatsApp</h3>
    <p><a href="https://wa.me/923014144869" target="_blank">+92 301 4144869</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">📸</div>
    <h3>Instagram</h3>
    <p><a href="https://instagram.com/itz_mohsin_riaz" target="_blank">itz_mohsin_riaz</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">🏙️</div>
    <h3>Home City</h3>
    <p>Lahore, Pakistan</p>
  </div>

  <div class="contact-card">
    <div class="icon">🎓</div>
    <h3>University</h3>
    <p>UET Faisalabad</p>
  </div>
</div>
