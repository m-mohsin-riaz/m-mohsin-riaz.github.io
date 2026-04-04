---
layout: default
title: My Journey
---

<style>
  .blog-header {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 15px;
    padding: 40px;
    margin-bottom: 30px;
    text-align: center;
  }
  .blog-header h1 { font-size: 32px; margin-bottom: 10px; }
  .blog-header p { color: #aaa; font-size: 16px; }
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

<div class="blog-header">
  <h1>My Journey</h1>
  <p>Stories, experiences and learnings from my life</p>
</div>

{% for post in site.posts %}
<div class="post-card">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="post-date">📅 {{ post.date | date: "%B %d, %Y" }}</p>
  <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
  <a class="read-more" href="{{ post.url }}">Read More →</a>
</div>
{% endfor %}
