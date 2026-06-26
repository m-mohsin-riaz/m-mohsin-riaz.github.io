---
layout: default
title: Contact
---
<style>
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

  .contact-cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    max-width: 1100px;
    margin: 0 auto 50px auto;
    padding: 10px;
  }
  .contact-card {
    background: white;
    border-radius: 12px;
    padding: 40px 14px 30px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.06);
    border-bottom: 4px solid transparent;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    min-height: 200px;
    transition: all 0.3s ease;
    box-sizing: border-box;
  }
  .contact-card:hover {
    transform: translateY(-8px);
    border-bottom: 4px solid #e94560;
  }
  .contact-card .icon {
    font-size: 45px;
    margin-bottom: 15px;
    display: block;
    line-height: 1;
  }
  .contact-card h3 {
    font-size: 13px;
    color: #888;
    margin: 0 0 8px 0;
    font-weight: 500;
    letter-spacing: 0.5px;
  }
  .contact-card p,
  .contact-card a {
    font-size: 14px;
    font-weight: 700;
    margin: 0 0 8px 0;
    color: #1a1a2e;
    text-decoration: none;
    line-height: 1.2;
    word-wrap: break-word;
    max-width: 100%;
  }
  .contact-card a { color: #e94560; }
  .contact-card .card-desc {
    font-size: 12px;
    font-weight: 400;
    color: #999;
    margin: 0;
    line-height: 1.5;
  }

  @media (max-width: 800px) {
    .contact-cards { grid-template-columns: repeat(2, 1fr); }
  }
  @media (max-width: 500px) {
    .contact-cards { grid-template-columns: 1fr; }
  }

  /* Message Form */
  .message-section {
    max-width: 1100px;
    margin: 0 auto;
    padding: 10px;
  }
  .message-box {
    background: white;
    border-radius: 15px;
    padding: 40px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.07);
  }
  .message-box h2 {
    font-size: 26px;
    margin: 0 0 6px 0;
    color: #1a1a2e;
  }
  .message-box .reply-note {
    font-size: 14px;
    color: #888;
    margin: 0 0 30px 0;
    font-weight: 400;
  }
  .form-field { margin-bottom: 20px; }
  .form-field label {
    display: block;
    font-size: 14px;
    font-weight: 600;
    color: #1a1a2e;
    margin-bottom: 8px;
  }
  .form-field input,
  .form-field textarea {
    width: 100%;
    box-sizing: border-box;
    padding: 12px 16px;
    border-radius: 10px;
    border: 1.5px solid #e0e0e0;
    font-size: 14px;
    font-family: inherit;
    color: #1a1a2e;
    outline: none;
    transition: border 0.2s;
    background: #fff;
  }
  .form-field input:focus,
  .form-field textarea:focus {
    border-color: #7c6cf5;
    box-shadow: 0 0 0 3px rgba(124,108,245,0.1);
  }
  .form-field textarea { resize: vertical; min-height: 140px; }
  .form-buttons {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 14px;
    margin-top: 10px;
  }
  .btn-whatsapp {
    background: #25D366;
    color: white;
    border: none;
    border-radius: 10px;
    padding: 15px;
    font-size: 15px;
    font-weight: 600;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    transition: opacity 0.2s;
    font-family: inherit;
  }
  .btn-email {
    background: #4F46E5;
    color: white;
    border: none;
    border-radius: 10px;
    padding: 15px;
    font-size: 15px;
    font-weight: 600;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    transition: opacity 0.2s;
    font-family: inherit;
  }
  .btn-whatsapp:hover { opacity: 0.88; }
  .btn-email:hover { opacity: 0.88; }

  @media (max-width: 500px) {
    .form-buttons { grid-template-columns: 1fr; }
    .message-box { padding: 24px 18px; }
  }
</style>

<div class="contact-header">
  <h1>Contact Me</h1>
  <p>I'm always open to discussing new projects or opportunities.</p>
</div>

<div class="contact-cards">
  <div class="contact-card">
    <span class="icon">📧</span>
    <h3>Email</h3>
    <a href="mailto:wmohsinriaz@gmail.com">wmohsinriaz@gmail.com</a>
    <p class="card-desc">Best way to reach me for professional queries and collaborations.</p>
  </div>
  <div class="contact-card">
    <span class="icon">🐙</span>
    <h3>GitHub</h3>
    <a href="https://github.com/m-mohsin-riaz" target="_blank">m-mohsin-riaz</a>
    <p class="card-desc">Explore my open-source projects and code contributions.</p>
  </div>
  <div class="contact-card">
    <span class="icon">💬</span>
    <h3>WhatsApp</h3>
    <a href="https://wa.me/923014144869" target="_blank">+92 301 4144869</a>
    <p class="card-desc">Drop a quick message — I usually reply within a few hours.</p>
  </div>
  <div class="contact-card">
    <span class="icon">📸</span>
    <h3>Instagram</h3>
    <a href="https://instagram.com/itz_mohsin_riaz" target="_blank">itz_mohsin_riaz</a>
    <p class="card-desc">Follow along for updates, creative work, and daily life.</p>
  </div>
  <div class="contact-card">
    <span class="icon">🏙️</span>
    <h3>Home City</h3>
    <p>Lahore, Pakistan</p>
    <p class="card-desc">Based in the cultural heart of Punjab — open to remote opportunities worldwide.</p>
  </div>
  <div class="contact-card">
    <span class="icon">🎓</span>
    <h3>University</h3>
    <p>UET Faisalabad</p>
    <p class="card-desc">Studying engineering with a passion for software development and problem-solving.</p>
  </div>
</div>

<div class="message-section">
  <div class="message-box">
    <h2>💌 Send a Message</h2>
    <p class="reply-note">I usually reply within 24 hours!</p>

    <div class="form-field">
      <label>👤 Your Name</label>
      <input type="text" id="contact-name" placeholder="John Doe" />
    </div>
    <div class="form-field">
      <label>📧 Email</label>
      <input type="email" id="contact-email" placeholder="john@example.com" />
    </div>
    <div class="form-field">
      <label>💬 Message</label>
      <textarea id="contact-msg" placeholder="Your message..."></textarea>
    </div>

    <div class="form-buttons">
      <button class="btn-whatsapp" onclick="sendWhatsApp()">💬 Message on WhatsApp</button>
      <button class="btn-email" onclick="sendEmail()">📧 Send Email</button>
    </div>
  </div>
</div>

<script>
function getFormData() {
  return {
    name: document.getElementById('contact-name').value.trim(),
    email: document.getElementById('contact-email').value.trim(),
    msg: document.getElementById('contact-msg').value.trim()
  };
}
function sendWhatsApp() {
  var d = getFormData();
  var text = "Hi! I'm " + (d.name || 'a visitor') + " (" + (d.email || 'no email provided') + ").\n\n" + (d.msg || '...');
  window.open('https://wa.me/923014144869?text=' + encodeURIComponent(text), '_blank');
}
function sendEmail() {
  var d = getFormData();
  var subject = encodeURIComponent('Message from ' + (d.name || 'Website Visitor'));
  var body = encodeURIComponent('Name: ' + d.name + '\nEmail: ' + d.email + '\n\nMessage:\n' + d.msg);
  window.location.href = 'mailto:wmohsinriaz@gmail.com?subject=' + subject + '&body=' + body;
}
</script>
