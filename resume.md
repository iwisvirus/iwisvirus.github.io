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
    max-width: 860px;
    margin: 30px auto;
  }
  .resume-terminal .r-header {
    color: #9ca3af;
    margin-bottom: 24px;
    padding-bottom: 14px;
    border-bottom: 1px solid #1e2530;
    font-size: 0.85rem;
  }
  .r-name {
    color: #22c55e;
    font-size: 1.6rem;
    margin: 0 0 4px;
    text-shadow: 0 0 12px rgba(34,197,94,0.2);
  }
  .r-contact {
    color: #6b7280;
    font-size: 0.78rem;
    margin: 0 0 28px;
    line-height: 1.8;
  }
  .r-contact a { color: #60a5fa; }
  .r-section {
    color: #22c55e;
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    margin: 32px 0 14px;
    padding-bottom: 6px;
    border-bottom: 1px solid #1e2530;
  }
  .r-section::before { content: "// "; color: #374151; }
  .r-entry {
    margin-bottom: 24px;
    padding-left: 14px;
    border-left: 2px solid #1e2530;
    transition: border-color 0.2s;
  }
  .r-entry:hover { border-left-color: #22c55e55; }
  .r-role {
    color: #e5e7eb;
    font-size: 0.95rem;
    font-weight: bold;
    margin: 0 0 2px;
  }
  .r-company { color: #60a5fa; font-size: 0.85rem; margin: 0 0 2px; }
  .r-dates { color: #6b7280; font-size: 0.78rem; margin: 0 0 10px; }
  .r-entry ul {
    margin: 6px 0 0;
    padding-left: 18px;
    color: #9ca3af;
    font-size: 0.82rem;
    line-height: 1.7;
  }
  .r-entry ul li { margin-bottom: 5px; }
  .r-entry ul li strong { color: #d1d5db; }
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 16px;
    margin-top: 8px;
  }
  .skill-group-title {
    color: #60a5fa;
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin: 0 0 6px;
  }
  .skill-tags { display: flex; flex-wrap: wrap; gap: 5px; }
  .skill-tag {
    background: #161b22;
    border: 1px solid #1e2530;
    color: #22c55e;
    padding: 2px 8px;
    border-radius: 4px;
    font-size: 0.75rem;
  }
  .r-about {
    color: #9ca3af;
    font-size: 0.85rem;
    line-height: 1.8;
    margin: 0;
    border-left: 2px solid #22c55e33;
    padding-left: 14px;
  }
</style>

<div class="resume-terminal">
  <div class="r-header">
    <span style="color:#22c55e">iris@brain</span>:<span style="color:#60a5fa">~</span>$ cat resume.txt
  </div>

  <h1 class="r-name">Iris Myung</h1>
  <p class="r-contact">
    iris.myung00@gmail.com &nbsp;·&nbsp; (647)-289-4575 &nbsp;·&nbsp; Toronto, Ontario<br>
    <a href="https://www.linkedin.com/in/irismyung">linkedin/irismyung</a> &nbsp;·&nbsp;
    <a href="https://github.com/iwisvirus">github/iwisvirus</a> &nbsp;·&nbsp;
    <a href="https://iwisvirus.github.io">iwisvirus.github.io</a>
  </p>

  <p class="r-section">About</p>
  <p class="r-about">
    UofT Computer Science graduate and Google-certified cybersecurity professional with hands-on DFIR experience
    across mobile forensics, email eDiscovery, deleted data recovery, and storage media imaging.
    Passionate about digital investigations — experienced in extracting forensic artifacts from damaged devices,
    analyzing structured and unstructured data, querying forensic databases, and supporting legal teams
    through detailed, court-ready investigative reporting. Strong foundation in cybersecurity,
    incident response, and forensic methodologies with a deep interest in evidence recovery and artifact analysis.
  </p>

  <p class="r-section">Education & Certifications</p>

  <div class="r-entry">
    <p class="r-role">B.Sc. Computer Science</p>
    <p class="r-company">University of Toronto</p>
    <p class="r-dates">September 2019 – June 2024</p>
    <ul><li>Mathematics & Statistics Minor</li></ul>
  </div>

  <div class="r-entry">
    <p class="r-role">Google Cybersecurity Certificate</p>
    <p class="r-company">Google</p>
    <p class="r-dates">August 2025</p>
  </div>

  <p class="r-section">Experience</p>

  <div class="r-entry">
    <p class="r-role">Digital Forensics Analyst</p>
    <p class="r-company">Data Rescue Labs</p>
    <p class="r-dates">May 2026 – Present &nbsp;·&nbsp; Toronto, ON</p>
    <ul>
      <li><strong>Mobile Forensics & Device Acquisition:</strong> Perform iOS and Android extractions using Cellebrite Physical Analyzer and Magnet AXIOM on active criminal and civil cases; execute brute-force acquisitions on locked iPhones and Samsung devices using Cellebrite and Inseyets; document acquisition failures and manage full case lifecycle through internal ticketing system.</li>
      <li><strong>Email Evidence Extraction & eDiscovery:</strong> Process AD1 image files in Magnet AXIOM with keyword filters and date-range scoping; produce PST output via ForensicEmail Extractor for ingestion into Relativity eDiscovery platform; authored step-by-step SOPs for repeatable export workflows.</li>
      <li><strong>Database & Deleted Data Recovery:</strong> Query SQLite databases (bugle_db for RCS messages, Telegram db_sqlite for crypto/chat recovery) using DB Browser and direct SQL; trace artifacts across chat history, timestamps, and media to reconstruct investigative timelines; produce multi-page forensic reports for legal teams.</li>
      <li><strong>Storage Media Forensics:</strong> Image physically damaged SSDs, HDDs, and NVMe chips using PC-3000 and FTK Imager; mount and process E01/E02 image files in Magnet AXIOM; apply SSD safe-mode techniques and thermostat analysis to assess hardware recoverability.</li>
      <li><strong>Registry & USB Artifact Analysis:</strong> Extract and analyze SOFTWARE/SYSTEM registry hives via Registry Explorer to determine USB device connection timestamps on BitLocker-encrypted NVMe devices; recover BitLocker keys via admin escalation.</li>
      <li><strong>Filesystem Timeline Analysis:</strong> Identify file deletion and overwrite history using $UsnJrnl (MFTECmd.exe), $MFT, and $LogFile; applied to cases involving cleared recycle bins and deleted email recovery scoping.</li>
      <li><strong>Cross-Artifact Investigation:</strong> Conduct keyword, image, and chat history investigations across Cellebrite PA databases; trace findings across linked artifacts (messages→contacts→media) to build complete investigative narratives for civil cases.</li>
    </ul>
  </div>

  <div class="r-entry">
    <p class="r-role">IT Systems & Security Analyst</p>
    <p class="r-company">University of Toronto – Law Department</p>
    <p class="r-dates">September 2025 – Present &nbsp;·&nbsp; Toronto, ON</p>
    <ul>
      <li><strong>Incident Response & Forensics:</strong> Perform forensic-level macOS recovery (DFU mode) and file recovery using PhotoRec; conduct endpoint patching and firmware recovery across Windows and macOS device fleets.</li>
      <li><strong>Access Control & Compliance:</strong> Enforce MFA/2FA policies and verify compliance during onboarding; lead endpoint security audits and conduct periodic user account access reviews aligned to PIPEDA.</li>
      <li><strong>Vulnerability Management & Documentation:</strong> Diagnose and remediate endpoint, network, and printer vulnerabilities; author runbooks and SOPs to maintain audit-ready records for Threat Risk Assessments (TRAs).</li>
      <li><strong>AI & Automation:</strong> Deployed a Model Context Protocol (MCP) server integrated with Claude AI to support AI-assisted workflow automation for a professor; engineered an AI-assisted diagnostic workflow to eliminate a recurring printer configuration conflict.</li>
      <li>Deliver Tier 1–2 technical support to lawyers, faculty, and staff across macOS, Windows 10/11, printers, AV/Zoom systems, and campus hardware.</li>
    </ul>
  </div>

  <div class="r-entry">
    <p class="r-role">Bartender</p>
    <p class="r-company">Watson's</p>
    <p class="r-dates">September 2025 – Present &nbsp;·&nbsp; Toronto, ON</p>
    <ul>
      <li>Craft a full range of cocktails — classics, signature, and seasonal menus — maintaining consistency and presentation standards.</li>
      <li>Deliver bar and floor service in a fast-paced environment; manage bar prep including batching, juicing, garnishes, and restocking.</li>
      <li>Lead service during private events, producing continuous rounds of cocktails while maintaining quality and workflow coordination.</li>
    </ul>
  </div>

  <div class="r-entry">
    <p class="r-role">Bartender</p>
    <p class="r-company">IDK Social Bar</p>
    <p class="r-dates">May 2025 – December 2025 &nbsp;·&nbsp; Toronto, ON</p>
    <ul>
      <li>Prepared and served cocktails, premade drinks, and beer on tap in a high-volume nightlife setting.</li>
      <li>Provided personalized and attentive guest service with precision and consistency under pressure.</li>
    </ul>
  </div>

  <div class="r-entry">
    <p class="r-role">Software Developer</p>
    <p class="r-company">Moneris</p>
    <p class="r-dates">May 2022 – April 2023 &nbsp;·&nbsp; Toronto, ON</p>
    <ul>
      <li><strong>Fee Disclosure API:</strong> Designed and implemented end-to-end — pricing logic, request validation, authentication middleware, downstream service orchestration, and release.</li>
      <li><strong>Access Control Engineering:</strong> Built API key authentication and request-validation layers (Spring Boot / Java) to enforce secure access control across internal and external consumers; addressed OWASP Top 10 risks including broken authentication, injection, and CORS misconfiguration.</li>
      <li><strong>Secure Cloud Migration:</strong> Migrated legacy databases to Microsoft Azure; integrated analytics pipeline via Synapse and Power BI; validated schema changes and data integrity throughout.</li>
      <li>Deployed and managed containerized microservices on Kubernetes; optimized API response times using EhCache; wrote JUnit tests covering validation logic and service contracts.</li>
    </ul>
  </div>

  <div class="r-entry">
    <p class="r-role">Server</p>
    <p class="r-company">Daldongnae Korean BBQ</p>
    <p class="r-dates">July 2021 – August 2025 &nbsp;·&nbsp; Toronto, ON</p>
    <ul>
      <li>Progressed from Hostess/Busser to Server within 2 months through strong performance.</li>
      <li>Managed a 20-table section serving up to 80 guests per shift; exceeded 120 tables during peak hours.</li>
      <li>Trained and mentored new staff; assisted with cash handling, register closing, and till balancing.</li>
    </ul>
  </div>

  <div class="r-entry">
    <p class="r-role">Server</p>
    <p class="r-company">Soos / Fat Choi Fine Dining</p>
    <p class="r-dates">May 2022 – March 2023 &nbsp;·&nbsp; Toronto, ON</p>
    <ul>
      <li>Provided personalized fine dining service accommodating guest preferences, allergies, and dietary requirements.</li>
      <li>Managed assigned sections serving parties from two to sixteen guests.</li>
    </ul>
  </div>

  <p class="r-section">Independent Research</p>
  <div class="r-entry">
    <p class="r-role">Self-directed DFIR Research</p>
    <p class="r-company"><a href="https://iwisvirus.github.io">iwisvirus.github.io</a></p>
    <ul>
      <li><strong>HackTheBox & TryHackMe:</strong> Sherlock/Brutus (log analysis, attacker attribution), Volatility (memory forensics, RAM artifact extraction), Autopsy (disk imaging, timeline analysis), Windows Forensics 1 & 2 (registry, prefetch, LNK files, shellbags, browser artifacts) — mapped to MITRE ATT&CK.</li>
      <li><strong>Academic Modules:</strong> Linux for Digital Forensics, Windows CLI forensics, number systems, and forensic timestamp interpretation.</li>
      <li><strong>Scripting & Tooling:</strong> Bash/Python for log parsing, timestamp normalization, and artifact triage.</li>
    </ul>
  </div>

  <p class="r-section">Technical Skills</p>
  <div class="skills-grid">
    <div>
      <p class="skill-group-title">Forensic Tools</p>
      <div class="skill-tags">
        <span class="skill-tag">Cellebrite PA</span>
        <span class="skill-tag">Magnet AXIOM</span>
        <span class="skill-tag">FTK Imager</span>
        <span class="skill-tag">PC-3000</span>
        <span class="skill-tag">Autopsy</span>
        <span class="skill-tag">Volatility</span>
        <span class="skill-tag">Registry Explorer</span>
        <span class="skill-tag">PhotoRec</span>
        <span class="skill-tag">ForensicEmail Extractor</span>
        <span class="skill-tag">Inseyets</span>
      </div>
    </div>
    <div>
      <p class="skill-group-title">Artifact Analysis</p>
      <div class="skill-tags">
        <span class="skill-tag">SQLite / DB Browser</span>
        <span class="skill-tag">bugle_db (RCS)</span>
        <span class="skill-tag">AD1 / PST / E01</span>
        <span class="skill-tag">Mobile Extractions</span>
        <span class="skill-tag">Memory Forensics</span>
        <span class="skill-tag">Windows Registry</span>
        <span class="skill-tag">$MFT / $UsnJrnl</span>
        <span class="skill-tag">NVMe / SSD / HDD Recovery</span>
      </div>
    </div>
    <div>
      <p class="skill-group-title">Security</p>
      <div class="skill-tags">
        <span class="skill-tag">Incident Response</span>
        <span class="skill-tag">MITRE ATT&CK</span>
        <span class="skill-tag">OWASP Top 10</span>
        <span class="skill-tag">MFA / 2FA</span>
        <span class="skill-tag">Chain of Custody</span>
        <span class="skill-tag">eDiscovery (Relativity)</span>
        <span class="skill-tag">Wireshark</span>
        <span class="skill-tag">Nmap</span>
      </div>
    </div>
    <div>
      <p class="skill-group-title">Programming</p>
      <div class="skill-tags">
        <span class="skill-tag">Python</span>
        <span class="skill-tag">SQL</span>
        <span class="skill-tag">Java</span>
        <span class="skill-tag">Bash</span>
        <span class="skill-tag">HTML / CSS</span>
        <span class="skill-tag">Spring Boot</span>
      </div>
    </div>
    <div>
      <p class="skill-group-title">Cloud & Infrastructure</p>
      <div class="skill-tags">
        <span class="skill-tag">Microsoft Azure</span>
        <span class="skill-tag">Kubernetes</span>
        <span class="skill-tag">CI/CD</span>
        <span class="skill-tag">Active Directory</span>
        <span class="skill-tag">Git</span>
      </div>
    </div>
    <div>
      <p class="skill-group-title">Languages</p>
      <div class="skill-tags">
        <span class="skill-tag">English</span>
        <span class="skill-tag">Korean</span>
        <span class="skill-tag">French</span>
      </div>
    </div>
  </div>

</div>
