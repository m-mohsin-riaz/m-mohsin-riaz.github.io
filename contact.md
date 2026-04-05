---
layout: default
title: Contact
---

<style>
  /* Header Styling */
  .contact-header {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 15px;
    padding: 40px;
    margin-bottom: 30px;
    text-align: center;
  }
  .contact-header h1 { font-size: 32px; margin-bottom: 10px; font-weight: 700; }
  .contact-header p { color: #aaa; font-size: 16px; }

  /* Grid Layout */
  .contact-cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* 3 cards per row */
    gap: 20px;
    max-width: 1000px;
    margin: 0 auto;
  }

  /* Individual Card Styling */
  .contact-card {
    background: white;
    border-radius: 15px;
    padding: 35px 15px;
    text-align: center;
    box-shadow: 0 4px 20px rgba(0,0,0,0.06);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 180px; /* Sab cards ka size ek jaisa rahega */
    transition: transform 0.3s ease;
  }

  .contact-card:hover {
    transform: translateY(-5px);
  }

  /* Icon Fix */
  .contact-card .icon { 
    font-size: 45px; 
    margin-bottom: 15px; 
    line-height: 1;
  }

  /* Label Styling (Email, GitHub etc.) */
  .contact-card h3 { 
    font-size: 13px; 
    color: #888; 
    margin: 0 0 10px 0; 
    font-weight: 600;
    text-transform: capitalize;
  }

  /* Content/Link Styling */
  .contact-card p, .contact-card a { 
    font-size: 14px; 
    color: #1a1a2e; 
    font-weight: 700; 
    margin: 0;
    text-decoration: none;
    word-break: break-all; /* Lambe emails ke liye safety */
  }

  .contact-card a { color: #e94560; }

  /* Mobile Responsive */
  @media (max-width: 768px) {
    .contact-cards {
      grid-template-columns: repeat(2, 1fr);
    }
  }
  @media (max-width: 480px) {
    .contact-cards {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="contact-header">
  <h1>Contact Me</h1>
  <p>Feel free to reach out anytime!</p>
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
