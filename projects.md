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
  .p-header {
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
    margin-top: 16px;
  }
  .project-card {
    background: #161b22;
    border: 1px solid #1e2530;
    border-radius: 10px;
    padding: 20px;
    transition: border-color 0.2s, box-shadow 0.2s;
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .project-card:hover {
    border-color: #22c55e55;
    box-shadow: 0 0 16px rgba(34,197,94,0.07);
  }
  .project-card h3 {
    color: #e5e7eb;
    font-size: 0.95rem;
    margin: 0;
  }
  .project-meta {
    color: #6b7280;
    font-size: 0.75rem;
    margin: 0;
  }
  .project-desc {
    color: #9ca3af;
    font-size: 0.82rem;
    margin: 0;
    line-height: 1.7;
    padding-left: 10px;
    border-left: 2px solid #1e2530;
  }
  .project-desc li { margin-bottom: 4px; }
  .project-tags { display: flex; flex-wrap: wrap; gap: 5px; margin-top: 4px; }
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

  <p class="p-section">Software & Web</p>
  <div class="projects-grid">

    <div class="project-card">
      <h3>1-on-1 Scheduling Website</h3>
      <p class="project-meta">Jan 2024 – Apr 2024 &nbsp;·&nbsp; University of Toronto</p>
      <ul class="project-desc">
        <li>Led development of a scheduling website enabling 1:1 meetings between accounts for UofT Music Department, from static design to full implementation.</li>
        <li>Built static front end using HTML/CSS, JavaScript, and Tailwind for consistent, responsive UI.</li>
        <li>Implemented Django back end with RESTful APIs and proper authentication; documented endpoints and payloads via Postman.</li>
        <li>Pre-populated database with 10 registered users and 5 calendars at different states for testing.</li>
      </ul>
      <div class="project-tags">
        <span class="project-tag">Django</span>
        <span class="project-tag">Python</span>
        <span class="project-tag">JavaScript</span>
        <span class="project-tag">Tailwind</span>
        <span class="project-tag">Postman</span>
        <span class="project-tag">REST API</span>
        <span class="project-tag">HTML/CSS</span>
      </div>
    </div>

    <div class="project-card">
      <h3>Memory Matching Card Game</h3>
      <p class="project-meta">Sep 2022 – Dec 2022 &nbsp;·&nbsp; University of Toronto</p>
      <ul class="project-desc">
        <li>Developed a memory matching card game in Java using object-oriented programming principles, with user account management and customizable game modes.</li>
        <li>Implemented GUI allowing users to choose different themes.</li>
        <li>Built leaderboards with user record tracking using SQL.</li>
      </ul>
      <div class="project-tags">
        <span class="project-tag">Java</span>
        <span class="project-tag">OOP</span>
        <span class="project-tag">SQL</span>
        <span class="project-tag">GUI</span>
      </div>
    </div>

  </div>

  <p class="p-section">Statistics & Data Analysis</p>
  <div class="projects-grid">

    <div class="project-card">
      <h3>Canadian Federal Election Popular Vote Analysis</h3>
      <p class="project-meta">Nov 2023 – Dec 2023 &nbsp;·&nbsp; University of Toronto</p>
      <ul class="project-desc">
        <li>Applied multiple regression analysis to examine relationships between voting likelihood and independent variables.</li>
        <li>Enhanced model accuracy using post-stratification techniques.</li>
        <li>Created bar plots to visualize voter distributions across demographic categories.</li>
      </ul>
      <div class="project-tags">
        <span class="project-tag">R</span>
        <span class="project-tag">Regression Analysis</span>
        <span class="project-tag">Post-Stratification</span>
        <span class="project-tag">Data Visualization</span>
      </div>
    </div>

    <div class="project-card">
      <h3>Wine Density Linear Regression</h3>
      <p class="project-meta">Jul 2023 – Aug 2023 &nbsp;·&nbsp; University of Toronto</p>
      <ul class="project-desc">
        <li>Developed and refined predictive models using linear regression on a wine dataset, achieving 88.4% explanation of variance in wine density.</li>
        <li>Applied statistical analysis including variable transformation, outlier handling, and feature selection for robustness and accuracy.</li>
      </ul>
      <div class="project-tags">
        <span class="project-tag">R</span>
        <span class="project-tag">Linear Regression</span>
        <span class="project-tag">Statistical Analysis</span>
        <span class="project-tag">Feature Selection</span>
      </div>
    </div>

  </div>

</div>
