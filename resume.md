---
layout: default
title: Resume
permalink: /resume/
---

<style>
  .resume-terminal {
    background: #0b0f14;
    color: #d1d5db;
    font-family: "JetBrains Mono", "Courier New", monospace;
    padding: 36px;
    border-radius: 12px;
    box-shadow: 0 20px 60px rgba(0,0,0,0.7), 0 0 0 1px #1e2530;
    max-width: 820px;
    margin: 30px auto;
  }
  .resume-terminal .r-header {
    color: #9ca3af;
    margin-bottom: 24px;
    padding-bottom: 14px;
    border-bottom: 1px solid #1e2530;
    font-size: 0.85rem;
  }
  .resume-terminal h2 {
    color: #22c55e;
    font-size: 1rem;
    margin: 28px 0 10px;
    text-transform: uppercase;
    letter-spacing: 2px;
  }
  .resume-terminal h2::before { content: "## "; color: #6b7280; }
  .r-entry {
    margin-bottom: 20px;
    padding-left: 16px;
    border-left: 2px solid #1e2530;
  }
  .r-entry:hover { border-left-color: #22c55e44; }
  .r-role {
    color: #e5e7eb;
    font-size: 1rem;
    font-weight: bold;
    margin: 0;
  }
  .r-company {
    color: #60a5fa;
    font-size: 0.9rem;
    margin: 2px 0;
  }
  .r-dates {
    color: #6b7280;
    font-size: 0.8rem;
    margin: 2px 0 8px;
  }
  .r-entry ul {
    margin: 6px 0;
    padding-left: 20px;
    color: #9ca3af;
    font-size: 0.88rem;
  }
  .r-entry ul li { margin-bottom: 4px; }
  .skills-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 8px;
  }
  .skill-tag {
    background: #161b22;
    border: 1px solid #1e2530;
    color: #22c55e;
    padding: 3px 10px;
    border-radius: 4px;
    font-size: 0.8rem;
  }
  .r-section-note {
    color: #6b7280;
    font-size: 0.8rem;
    margin-top: 4px;
  }
</style>

<div class="resume-terminal">
  <div class="r-header">
    <span style="color:#22c55e">iris@brain</span>:<span style="color:#60a5fa">~</span>$ cat resume.txt
  </div>

  <h2>Experience</h2>

  <div class="r-entry">
    <p class="r-role">[ Role Title ]</p>
    <p class="r-company">[ Company / Organization ]</p>
    <p class="r-dates">[ Start ] — [ End ]  ·  [ Location ]</p>
    <ul>
      <li>[ What you did and what impact it had ]</li>
      <li>[ Another bullet ]</li>
    </ul>
  </div>

  <div class="r-entry">
    <p class="r-role">[ Role Title ]</p>
    <p class="r-company">[ Company / Organization ]</p>
    <p class="r-dates">[ Start ] — [ End ]  ·  [ Location ]</p>
    <ul>
      <li>[ What you did ]</li>
      <li>[ Another bullet ]</li>
    </ul>
  </div>

  <h2>Education</h2>

  <div class="r-entry">
    <p class="r-role">Honours Bachelor of Science — Computer Science</p>
    <p class="r-company">University of Toronto</p>
    <p class="r-dates">[ Year ] — Present  ·  Toronto, ON</p>
    <ul>
      <li>Mathematics & Statistics Minor</li>
      <li>[ Relevant coursework, clubs, or achievements ]</li>
    </ul>
  </div>

  <h2>Skills & Tools</h2>

  <div class="skills-grid">
    <span class="skill-tag">Autopsy</span>
    <span class="skill-tag">Volatility</span>
    <span class="skill-tag">Wireshark</span>
    <span class="skill-tag">Python</span>
    <span class="skill-tag">[ Add more ]</span>
  </div>

  <h2>Certifications & Courses</h2>

  <div class="r-entry">
    <p class="r-role">[ Cert / Course Name ]</p>
    <p class="r-company">[ Issuer ]</p>
    <p class="r-dates">[ Date ]</p>
  </div>

</div>
