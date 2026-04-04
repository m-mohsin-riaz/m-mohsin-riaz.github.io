---
layout: default
title: My Journey
permalink: /myjourney/
---

<style>
  .journey-header {
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: white;
    border-radius: 15px;
    padding: 40px;
    margin-bottom: 30px;
    text-align: center;
  }
  .journey-header h1 { font-size: 32px; margin-bottom: 10px; }
  .journey-header p { color: #aaa; font-size: 16px; }
  .semester-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
  }
  .semester-card {
    background: white;
    border-radius: 12px;
    padding: 30px;
    text-align: center;
    box-shadow: 0 3px 15px rgba(0,0,0,0.08);
    border-left: 4px solid #e94560;
    text-decoration: none;
    color: #1a1a2e;
    display: block;
    transition: transform 0.2s;
  }
  .semester-card:hover { transform: translateY(-5px); }
  .semester-card .icon { font-size: 40px; margin-bottom: 15px; }
  .semester-card h2 { font-size: 20px; margin-bottom: 8px; color: #1a1a2e; }
  .semester-card p { font-size: 14px; color: #888; }
</style>

<div class="journey-header">
  <h1>My Journey</h1>
  <p>My university life semester by semester</p>
</div>

<div class="semester-cards">
  <a class="semester-card" href="/semester1/">
    <div class="icon">📚</div>
    <h2>Semester 1</h2>
    <p>My first semester experience</p>
  </a>
  <a class="semester-card" href="/semester2/">
    <div class="icon">🎯</div>
    <h2>Semester 2</h2>
    <p>My second semester experience</p>
  </a>
</div>
