---
layout: default
title: About
permalink: /about/
---

Hi, I'm Iris(Hyelim) Myung. I was born in South Korea and came to Canada in grade 10 by myself. I graduated University of Toronto in 2024 with a Computer Science Major and Mathematics and Statistics Minor. I am currently working on pursuing a career in DFIR and getting my Permanent Residency in Canada. 

<style>
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
    $cd human/iris/brain<br>
  </div>

  <div class="terminal-line">
    > Analyzing...
  </div>

  <div class="terminal-line">
    > Welcome. <br>
    > What would you like to explore?<br>
    <br>
       [1] DFIR journey<br>
       [2] Creative chaos
  </div>

  <div class="input-line">
    <span class="prompt">$</span>
    <input id="terminalInput" type="text" autofocus />
    <span class="cursor"></span>
  </div>

  <div id="terminalOutput"></div>
</div>

<script>
  const input = document.getElementById("terminalInput");
  const output = document.getElementById("terminalOutput");

  input.addEventListener("keydown", function(e) {
    if (e.key === "Enter") {
      const value = input.value.trim().toLowerCase();
      input.value = "";

      if (value === "1" || value === "[1]") {
        output.innerHTML += `
          <div class="terminal-line">> Access granted.</div>
          <div class="terminal-line hint">Redirecting to DFIR Journey...</div>
        `;
        setTimeout(() => {
          window.location.href = "{{ site.baseurl }}/category/DFIR/";
        }, 1200);

      } else if (value === "2" || value === "[2]") {
        output.innerHTML += `
          <div class="terminal-line">> Access granted.</div>
          <div class="terminal-line hint">Redirecting to creative chaos...</div>
        `;
        setTimeout(() => {
          window.location.href = "{{ site.baseurl }}/category/other-interests/";
        }, 1200);

      } else {
        output.innerHTML += `
          <div class="terminal-line error">
            > Command not recognized. Type yes or no.
          </div>
        `;
      }

      output.scrollTop = output.scrollHeight;
    }
  });
</script>
