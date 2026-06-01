---
layout: default
title: Projects
permalink: /projects/
---

<style>
  .projects-terminal {
    background: #0b0f14;
    color: #d1d5db;
    font-family: "JetBrains Mono", "Courier New", monospace;
    padding: 36px;
    border-radius: 12px;
    box-shadow: 0 20px 60px rgba(0,0,0,0.7), 0 0 0 1px #1e2530;
    max-width: 860px;
    margin: 30px auto;
  }
  .projects-terminal .p-header {
    color: #9ca3af;
    margin-bottom: 24px;
    padding-bottom: 14px;
    border-bottom: 1px solid #1e2530;
    font-size: 0.85rem;
  }
  .projects-terminal h1 {
    color: #22c55e;
    font-size: 1.3rem;
    margin-top: 0;
    text-shadow: 0 0 10px rgba(34,197,94,0.2);
  }
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
    gap: 16px;
    margin-top: 20px;
  }
  .project-card {
    background: #161b22;
    border: 1px solid #1e2530;
    border-radius: 10px;
    padding: 20px;
    transition: border-color 0.2s, box-shadow 0.2s;
  }
  .project-card:hover {
    border-color: #22c55e55;
    box-shadow: 0 0 16px rgba(34,197,94,0.07);
  }
  .project-card h3 {
    color: #e5e7eb;
    font-size: 0.95rem;
    margin: 0 0 6px;
  }
  .project-card h3 a { color: #60a5fa; }
  .project-card h3 a:hover { color: #22c55e; }
  .project-desc {
    color: #9ca3af;
    font-size: 0.82rem;
    margin: 0 0 12px;
    line-height: 1.6;
  }
  .project-tags { display: flex; flex-wrap: wrap; gap: 5px; }
  .project-tag {
    background: #0b0f14;
    border: 1px solid #1e2530;
    color: #22c55e;
    padding: 2px 8px;
    border-radius: 4px;
    font-size: 0.72rem;
  }
  .p-section {
    color: #22c55e;
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    margin: 32px 0 14px;
    padding-bottom: 6px;
    border-bottom: 1px solid #1e2530;
  }
  .p-section::before { content: "// "; color: #374151; }
</style>

<div class="projects-terminal">
  <div class="p-header">
    <span style="color:#22c55e">iris@brain</span>:<span style="color:#60a5fa">~/projects</span>$ ls -la
  </div>

  <h1>Projects</h1>

  <p class="p-section">DFIR & Security</p>
  <div class="projects-grid">

    <div class="project-card">
      <h3>[ Project Name ]</h3>
      <p class="project-desc">[ What it does — one or two sentences. What problem it solves or what you learned. ]</p>
      <div class="project-tags">
        <span class="project-tag">Python</span>
        <span class="project-tag">[ Add tool ]</span>
      </div>
    </div>

    <div class="project-card">
      <h3>[ Project Name ]</h3>
      <p class="project-desc">[ Description ]</p>
      <div class="project-tags">
        <span class="project-tag">[ Tag ]</span>
      </div>
    </div>

  </div>

  <p class="p-section">Software & Dev</p>
  <div class="projects-grid">

    <div class="project-card">
      <h3>[ Project Name ]</h3>
      <p class="project-desc">[ Description ]</p>
      <div class="project-tags">
        <span class="project-tag">Java</span>
        <span class="project-tag">[ Tag ]</span>
      </div>
    </div>

  </div>

  <p class="p-section">Other</p>
  <div class="projects-grid">

    <div class="project-card">
      <h3>[ Project Name ]</h3>
      <p class="project-desc">[ Description ]</p>
      <div class="project-tags">
        <span class="project-tag">[ Tag ]</span>
      </div>
    </div>

  </div>

</div>
