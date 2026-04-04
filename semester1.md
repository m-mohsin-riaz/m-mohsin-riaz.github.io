---
layout: default
title: Semester 1
permalink: /semester1/
---

<style>
  .sem-header {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 15px;
    padding: 40px;
    margin-bottom: 30px;
    text-align: center;
  }
  .sem-header h1 { font-size: 32px; margin-bottom: 10px; }
  .sem-header p { color: #aaa; font-size: 16px; }
  .back-btn {
    display: inline-block;
    margin-bottom: 25px;
    background: #e94560;
    color: white;
    padding: 8px 18px;
    border-radius: 20px;
    text-decoration: none;
    font-size: 14px;
  }
  .back-btn:hover { background: #c73652; }
  .info-section {
    background: white;
    border-radius: 12px;
    padding: 30px;
    margin-bottom: 20px;
    box-shadow: 0 3px 15px rgba(0,0,0,0.08);
  }
  .info-section h2 {
    color: #e94560;
    font-size: 20px;
    margin-bottom: 15px;
    border-bottom: 2px solid #f4f6f9;
    padding-bottom: 10px;
  }
  .info-section p { line-height: 1.8; color: #555; font-size: 15px; }
  .subjects-grid {
    display: grid !important;
    grid-template-columns: repeat(3, 1fr) !important;
    gap: 12px !important;
    margin-top: 20px;
  }
  .subject-card {
    background: #f9f9f9;
    border-left: 4px solid #e94560;
    border-radius: 8px;
    padding: 15px 12px;
    text-align: center;
  }
  .subject-card .icon { font-size: 26px; }
  .subject-card .name {
    font-size: 13px;
    font-weight: bold;
    color: #1a1a2e;
    margin-top: 8px;
  }
  .subject-card .type {
    font-size: 11px;
    color: #888;
    margin-top: 3px;
  }
  .post-card {
    background: white;
    border-radius: 12px;
    padding: 25px 30px;
    margin-bottom: 20px;
    box-shadow: 0 3px 15px rgba(0,0,0,0.08);
    border-left: 4px solid #e94560;
  }
  .post-card h2 { font-size: 20px; margin-bottom: 8px; }
  .post-card h2 a { color: #1a1a2e; text-decoration: none; }
  .post-card h2 a:hover { color: #e94560; }
  .post-date { color: #888; font-size: 13px; margin-bottom: 10px; }
  .post-excerpt { color: #555; font-size: 14px; line-height: 1.7; }
  .read-more {
    display: inline-block;
    margin-top: 12px;
    color: #e94560;
    font-size: 14px;
    font-weight: bold;
    text-decoration: none;
  }
</style>

<a class="back-btn" href="/myjourney/">← Back to My Journey</a>

<div class="sem-header">
  <h1>Semester 1</h1>
  <p>My first semester at UET Faisalabad</p>
</div>

<div class="info-section">
  <h2>📖 About This Semester</h2>
  <p>My first semester at UET Faisalabad was a life-changing experience. Moving into the hostel, attending university for the first time, making new friends, and learning new subjects all at once was both exciting and challenging. From struggling with Calculus and Physics to writing my first Python programs, every week taught me something new. I even completed a Machine Learning project in my very first semester, which gave me great confidence and motivation to keep growing.</p>

  <div class="subjects-grid">
    <div class="subject-card">
      <div class="icon">💻</div>
      <div class="name">Programming Fundamentals</div>
      <div class="type">Theory</div>
    </div>
    <div class="subject-card">
      <div class="icon">📐</div>
      <div class="name">Calculus</div>
      <div class="type">Theory</div>
    </div>
    <div class="subject-card">
      <div class="icon">🧮</div>
      <div class="name">Discrete Mathematics</div>
      <div class="type">Theory</div>
    </div>
    <div class="subject-card">
      <div class="icon">🖥️</div>
      <div class="name">AICT</div>
      <div class="type">Theory</div>
    </div>
    <div class="subject-card">
      <div class="icon">⚛️</div>
      <div class="name">Applied Physics</div>
      <div class="type">Theory</div>
    </div>
    <div class="subject-card">
      <div class="icon">📖</div>
      <div class="name">Fahm-e-Quran</div>
      <div class="type">Theory</div>
    </div>
    <div class="subject-card">
      <div class="icon">🔬</div>
      <div class="name">Lab - PF</div>
      <div class="type">Lab</div>
    </div>
    <div class="subject-card">
      <div class="icon">💾</div>
      <div class="name">Lab - AICT</div>
      <div class="type">Lab</div>
    </div>
    <div class="subject-card">
      <div class="icon">🧪</div>
      <div class="name">Lab - Physics</div>
      <div class="type">Lab</div>
    </div>
  </div>
</div>

<div class="info-section">
  <h2>📝 Posts</h2>
  {% assign sem1_posts = site.posts | where_exp: "post", "post.tags contains 'semester1'" %}
  {% if sem1_posts.size > 0 %}
    {% for post in sem1_posts %}
    <div class="post-card">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p class="post-date">📅 {{ post.date | date: "%B %d, %Y" }}</p>
      <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a class="read-more" href="{{ post.url }}">Read More →</a>
    </div>
    {% endfor %}
  {% else %}
    <p style="color:#888;">No posts added yet.</p>
  {% endif %}
</div>
