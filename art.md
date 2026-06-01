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
    max-width: 900px;
    margin: 30px auto;
  }
  .a-header {
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
  .art-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
    gap: 14px;
    margin-top: 16px;
  }
  .art-card {
    background: #161b22;
    border: 1px solid #1e2530;
    border-radius: 8px;
    overflow: hidden;
    transition: border-color 0.2s, transform 0.2s, box-shadow 0.2s;
    cursor: pointer;
  }
  .art-card:hover {
    border-color: #22c55e55;
    transform: translateY(-3px);
    box-shadow: 0 10px 28px rgba(0,0,0,0.5);
  }
  .art-card img {
    width: 100%;
    aspect-ratio: 1;
    object-fit: cover;
    display: block;
  }

  /* Lightbox */
  .lightbox {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.92);
    z-index: 1000;
    align-items: center;
    justify-content: center;
    cursor: zoom-out;
  }
  .lightbox.active { display: flex; }
  .lightbox img {
    max-width: 90vw;
    max-height: 90vh;
    object-fit: contain;
    border-radius: 6px;
    box-shadow: 0 0 60px rgba(0,0,0,0.8);
  }
  .lightbox-close {
    position: absolute;
    top: 20px; right: 28px;
    color: #9ca3af;
    font-size: 2rem;
    cursor: pointer;
    line-height: 1;
  }
  .lightbox-close:hover { color: #22c55e; }
</style>

<div class="art-terminal">
  <div class="a-header">
    <span style="color:#22c55e">iris@brain</span>:<span style="color:#60a5fa">~/chaos/art</span>$ ls -la gallery/
  </div>

  <h1>Art</h1>

  <div class="art-grid">
    <div class="art-card" onclick="openLightbox('/art/IMG_3698.PNG')">
      <img src="/art/IMG_3698.PNG" alt="" loading="lazy">
    </div>
    <div class="art-card" onclick="openLightbox('/art/IMG_4346.jpg')">
      <img src="/art/IMG_4346.jpg" alt="" loading="lazy">
    </div>
    <div class="art-card" onclick="openLightbox('/art/IMG_2766.JPG')">
      <img src="/art/IMG_2766.JPG" alt="" loading="lazy">
    </div>
    <div class="art-card" onclick="openLightbox('/art/IMG_0089.JPG')">
      <img src="/art/IMG_0089.JPG" alt="" loading="lazy">
    </div>
  </div>
</div>

<div class="lightbox" id="lightbox" onclick="closeLightbox()">
  <span class="lightbox-close" onclick="closeLightbox()">&times;</span>
  <img id="lightbox-img" src="" alt="">
</div>

<script>
  function openLightbox(src) {
    document.getElementById("lightbox-img").src = src;
    document.getElementById("lightbox").classList.add("active");
  }
  function closeLightbox() {
    document.getElementById("lightbox").classList.remove("active");
    document.getElementById("lightbox-img").src = "";
  }
  document.addEventListener("keydown", e => { if (e.key === "Escape") closeLightbox(); });
</script>
