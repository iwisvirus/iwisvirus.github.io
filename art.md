---
layout: default
title: Art
permalink: /art/
---

<style>
  .art-terminal {
    background: #0b0f14;
    color: #d1d5db;
    font-family: "JetBrains Mono", "Courier New", monospace;
    padding: 36px;
    border-radius: 12px;
    box-shadow: 0 20px 60px rgba(0,0,0,0.7), 0 0 0 1px #1e2530;
    max-width: 860px;
    margin: 30px auto;
  }
  .art-terminal .a-header {
    color: #9ca3af;
    margin-bottom: 24px;
    padding-bottom: 14px;
    border-bottom: 1px solid #1e2530;
    font-size: 0.85rem;
  }
  .art-terminal h1 {
    color: #22c55e;
    font-size: 1.3rem;
    margin-top: 0;
    text-shadow: 0 0 10px rgba(34,197,94,0.2);
  }
  .art-terminal p.subtitle {
    color: #6b7280;
    font-size: 0.85rem;
    margin-top: -10px;
    margin-bottom: 28px;
  }
  .art-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: 14px;
    margin-top: 16px;
  }
  .art-card {
    background: #161b22;
    border: 1px solid #1e2530;
    border-radius: 8px;
    overflow: hidden;
    transition: border-color 0.2s, transform 0.2s;
    cursor: pointer;
  }
  .art-card:hover {
    border-color: #22c55e55;
    transform: translateY(-2px);
    box-shadow: 0 8px 24px rgba(0,0,0,0.4);
  }
  .art-card img {
    width: 100%;
    aspect-ratio: 1;
    object-fit: cover;
    display: block;
    border-bottom: 1px solid #1e2530;
  }
  .art-placeholder {
    width: 100%;
    aspect-ratio: 1;
    background: #0d1117;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #374151;
    font-size: 2rem;
    border-bottom: 1px solid #1e2530;
  }
  .art-card-info {
    padding: 10px 12px;
  }
  .art-card-title {
    color: #e5e7eb;
    font-size: 0.82rem;
    margin: 0 0 2px;
  }
  .art-card-meta {
    color: #6b7280;
    font-size: 0.75rem;
    margin: 0;
  }
  .art-section-label {
    color: #22c55e;
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin: 28px 0 12px;
  }
  .art-section-label::before { content: "// "; color: #6b7280; }
</style>

<div class="art-terminal">
  <div class="a-header">
    <span style="color:#22c55e">iris@brain</span>:<span style="color:#60a5fa">~/chaos/art</span>$ ls -la gallery/
  </div>

  <h1>Art</h1>
  <p class="subtitle">[ Add a one-liner about your art here — medium, vibe, whatever ]</p>

  <p class="art-section-label">[ Category — e.g. Drawings / Digital / Photography ]</p>

  <div class="art-grid">

    <!-- Copy this block for each piece and replace the placeholder with an <img> tag -->
    <div class="art-card">
      <div class="art-placeholder">+</div>
      <div class="art-card-info">
        <p class="art-card-title">[ Title ]</p>
        <p class="art-card-meta">[ Medium ] · [ Year ]</p>
      </div>
    </div>

    <div class="art-card">
      <div class="art-placeholder">+</div>
      <div class="art-card-info">
        <p class="art-card-title">[ Title ]</p>
        <p class="art-card-meta">[ Medium ] · [ Year ]</p>
      </div>
    </div>

    <div class="art-card">
      <div class="art-placeholder">+</div>
      <div class="art-card-info">
        <p class="art-card-title">[ Title ]</p>
        <p class="art-card-meta">[ Medium ] · [ Year ]</p>
      </div>
    </div>

  </div>

  <p class="art-section-label">[ Another Category ]</p>

  <div class="art-grid">

    <div class="art-card">
      <div class="art-placeholder">+</div>
      <div class="art-card-info">
        <p class="art-card-title">[ Title ]</p>
        <p class="art-card-meta">[ Medium ] · [ Year ]</p>
      </div>
    </div>

  </div>

</div>
