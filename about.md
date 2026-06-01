---
layout: default
title: About
permalink: /about/
---

<style>
  .aligned > div {
    display: grid;
    grid-template-columns: 170px 16px auto;
    margin-bottom: 6px;
  }
  .key { text-align: left; color: #9ca3af; }
  .sep { text-align: center; color: #6b7280; }
  .val { color: #e5e7eb; }

  .terminal {
    background: #0b0f14;
    color: #d1d5db;
    font-family: "JetBrains Mono", "Courier New", monospace;
    padding: 36px;
    border-radius: 12px;
    box-shadow: 0 20px 60px rgba(0,0,0,0.7), 0 0 0 1px #1e2530;
    max-width: 820px;
    margin: 30px auto;
    animation: fadeInUp 0.6s ease both;
  }

  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(20px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  .terminal-header {
    color: #9ca3af;
    margin-bottom: 20px;
    padding-bottom: 14px;
    border-bottom: 1px solid #1e2530;
    font-size: 0.85rem;
  }
  .terminal-line { margin: 10px 0; }
  .prompt { color: #22c55e; }

  .section-divider {
    border: none;
    border-top: 1px solid #1e2530;
    margin: 28px 0;
  }

  .section-label {
    color: #22c55e;
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin: 0 0 14px;
  }
  .section-label::before { content: "## "; color: #6b7280; }

  .motto {
    border-left: 2px solid #22c55e;
    padding: 10px 16px;
    margin: 0 0 20px;
    color: #e5e7eb;
    font-size: 0.95rem;
    font-style: italic;
    background: #0d1117;
    border-radius: 0 6px 6px 0;
  }
  .motto span { color: #6b7280; font-size: 0.75rem; font-style: normal; display: block; margin-top: 4px; }

  .goals-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .goals-list li {
    color: #9ca3af;
    font-size: 0.88rem;
    margin-bottom: 10px;
    display: flex;
    align-items: flex-start;
    gap: 10px;
    transition: color 0.2s;
  }
  .goals-list li:hover { color: #d1d5db; }
  .goals-list li::before {
    content: "[ ]";
    color: #6b7280;
    flex-shrink: 0;
  }
  .goals-list li.done::before {
    content: "[x]";
    color: #22c55e;
  }
  .goals-list li.done { color: #6b7280; text-decoration: line-through; }

  .goal-category {
    color: #60a5fa;
    font-size: 0.78rem;
    margin: 20px 0 6px;
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  .story-link {
    display: inline-block;
    margin-top: 16px;
    color: #60a5fa;
    font-size: 0.85rem;
    border: 1px solid #1e2530;
    padding: 6px 14px;
    border-radius: 6px;
    transition: border-color 0.2s, color 0.2s, box-shadow 0.2s;
  }
  .story-link:hover {
    border-color: #22c55e55;
    color: #22c55e;
    box-shadow: 0 0 10px rgba(34,197,94,0.15);
  }
</style>

<div class="terminal">
  <div class="terminal-header">
    <span style="color:#22c55e">iris@brain</span>:<span style="color:#60a5fa">~/human/iris</span>$ cat about.txt
  </div>

  <div class="terminal-line aligned">
    <div><span class="key">Name</span><span class="sep">:</span><span class="val">Iris (Hyelim) Myung</span></div>
    <div><span class="key">Education</span><span class="sep">:</span><span class="val">University of Toronto</span></div>
    <div><span class="key">Degree</span><span class="sep">:</span><span class="val">Computer Science · Math & Statistics Minor</span></div>
    <div><span class="key">Career goal</span><span class="sep">:</span><span class="val">Top digital forensics examiner & tool builder</span></div>
    <div><span class="key">Based in</span><span class="sep">:</span><span class="val">Toronto, ON</span></div>
  </div>

  <hr class="section-divider">

  <p class="section-label">Goals</p>

  <div class="motto">
    "Learn from mistakes, but never regret."
    <span>— life motto</span>
  </div>

  <p class="goal-category">// life</p>
  <ul class="goals-list">
    <li>Get Permanent Residency in Canada</li>
    <li>Build my own house</li>
    <li>Own and build my own business</li>
    <li>Write my own book</li>
    <li>Hold a small concert</li>
    <li>Compete in a ballroom dancing competition</li>
  </ul>

  <p class="goal-category">// career</p>
  <ul class="goals-list">
    <li>Become a top digital forensics examiner</li>
    <li>Build forensics tools used in real investigations</li>
  </ul>

  <p class="goal-category">// personal growth</p>
  <ul class="goals-list">
    <li>Learn carpentry</li>
    <li>Learn 1–2 new languages</li>
  </ul>

  <hr class="section-divider">

  <p class="section-label">Origin</p>
  <p style="color:#9ca3af; font-size:0.88rem; margin:0 0 10px;">
    Came to Canada alone in high school. Figured it out. Made it to UofT.
    Still figuring it out — just with better tools.
  </p>
  <a class="story-link" href="/story/">$ cat origin.txt →</a>

</div>
