---
layout: default
title: About
permalink: /about/
---

<style>
  .aligned > div {
  display: grid;
  grid-template-columns: 160px 20px auto;
  margin-bottom: 6px;
}

.key {
  text-align: right;
  color: #9ca3af;
}

.sep {
  text-align: center;
}

.val {
  color: #e5e7eb;
}
  .terminal {
    background: #0b0f14;
    color: #d1d5db;
    font-family: "Courier New", monospace;
    padding: 40px;
    border-radius: 12px;
    box-shadow: 0 20px 60px rgba(0,0,0,0.6);
    max-width: 800px;
    margin: 60px auto;
  }

  .terminal-header {
    color: #9ca3af;
    margin-bottom: 20px;
  }

  .terminal-line {
    margin: 10px 0;
  }

  .prompt {
    color: #22c55e;
  }

  .input-line {
    display: flex;
    align-items: center;
  }

  input {
    background: transparent;
    border: none;
    color: #e5e7eb;
    font-family: inherit;
    font-size: 1rem;
    outline: none;
    margin-left: 8px;
    width: 100%;
  }

  .cursor {
    display: inline-block;
    width: 10px;
    height: 18px;
    background: #22c55e;
    margin-left: 4px;
    animation: blink 1s infinite;
  }

  @keyframes blink {
    50% { opacity: 0; }
  }

  .error {
    color: #ef4444;
  }

  .hint {
    color: #60a5fa;
    font-size: 0.9rem;
  }
</style>

<div class="terminal">
  <div class="terminal-header">
    $cd human/iris/basic_info<br>
    $cat about.txt
  </div>

<div class="terminal-line aligned">
  <div><span class="key">Name</span><span class="sep">:</span><span class="val">Iris (Hyelim) Myung</span></div>
  <div><span class="key">Education</span><span class="sep">:</span><span class="val">University of Toronto</span></div>
  <div><span class="key">Degree</span><span class="sep">:</span><span class="val">Computer Science Major, Mathematics & Statistics Minor</span></div>
  <div><span class="key">Career goals</span><span class="sep">:</span><span class="val">Work for the government in crime scenes with DFIR</span></div>
  <div><span class="key">Other goals</span><span class="sep">:</span><span class="val">
    Getting Permanent Residency in Canada, Building my own house,
    Holding a small concert, Ballroom dancing competition
  </span></div>
</div>

