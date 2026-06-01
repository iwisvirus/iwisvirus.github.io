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
  .r-header {
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
    margin: 0 0 24px;
    line-height: 1.8;
  }
  .r-contact a { color: #60a5fa; }

  /* Tab buttons */
  .resume-tabs {
    display: flex;
    gap: 10px;
    margin-bottom: 28px;
    border-bottom: 1px solid #1e2530;
    padding-bottom: 0;
  }
  .tab-btn {
    background: none;
    border: 1px solid #1e2530;
    border-bottom: none;
    color: #6b7280;
    font-family: "JetBrains Mono", "Courier New", monospace;
    font-size: 0.8rem;
    padding: 8px 18px;
    cursor: pointer;
    border-radius: 6px 6px 0 0;
    transition: color 0.2s, border-color 0.2s, background 0.2s;
    margin-bottom: -1px;
  }
  .tab-btn:hover { color: #d1d5db; border-color: #374151; }
  .tab-btn.active {
    color: #22c55e;
    border-color: #22c55e44;
    background: #0d1117;
    text-shadow: 0 0 8px rgba(34,197,94,0.3);
  }

  .tab-content { display: none; }
  .tab-content.active { display: block; }

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
  .r-role { color: #e5e7eb; font-size: 0.95rem; font-weight: bold; margin: 0 0 2px; }
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
  .r-about {
    color: #9ca3af;
    font-size: 0.85rem;
    line-height: 1.8;
    margin: 0;
    border-left: 2px solid #22c55e33;
    padding-left: 14px;
  }
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
    transition: border-color 0.2s, box-shadow 0.2s;
  }
  .skill-tag:hover {
    border-color: #22c55e88;
    box-shadow: 0 0 8px rgba(34,197,94,0.3);
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

  <div class="resume-tabs">
    <button class="tab-btn active" onclick="switchTab('it')">IT &amp; Digital Forensics</button>
    <button class="tab-btn" onclick="switchTab('hospitality')">Hospitality</button>
    <button class="tab-btn" onclick="switchTab('other')">Other</button>
  </div>

  <!-- ==================== IT & DFIR TAB ==================== -->
  <div id="tab-it" class="tab-content active">

    <p class="r-section">About</p>
    <p class="r-about">
      UofT Computer Science graduate and Google-certified cybersecurity professional with hands-on DFIR experience
      across mobile forensics, email eDiscovery, deleted data recovery, and storage media imaging.
      Passionate about digital investigations — experienced in extracting forensic artifacts from damaged devices,
      analyzing structured and unstructured data, querying forensic databases, and supporting legal teams
      through detailed, court-ready investigative reporting.
    </p>

    <p class="r-section">Education & Certifications</p>

    <div class="r-entry">
      <p class="r-role">B.Sc. Computer Science</p>
      <p class="r-company">University of Toronto</p>
      <p class="r-dates">September 2019 – June 2024</p>
      <ul>
        <li>Mathematics & Statistics Minor</li>
        <li><strong>CS:</strong> Software Design, Software Tools & System Programming, Computer Organization, Data Structures & Analysis, Introduction to Databases, Programming on the Web, Algorithm Design & Analysis, Introduction to Image Understanding, Computers & Society</li>
        <li><strong>Math:</strong> Abstract Mathematics, Introduction to Combinatorics, Multivariable Calculus, Introduction to Number Theory</li>
        <li><strong>Stats:</strong> Methods of Data Analysis, Survey Sampling & Observational Data</li>
      </ul>
    </div>

    <div class="r-entry">
      <p class="r-role">Google Cybersecurity Certificate</p>
      <p class="r-company">Google &nbsp;·&nbsp; <a href="https://github.com/iwisvirus/Google-cybersecurity-certificate" target="_blank" style="color:#60a5fa;">↗ github</a></p>
      <p class="r-dates">August 2025</p>
      <ul>
        <li>Completed hands-on labs covering secure system design, risk analysis, incident response, SIEM tools, and security practices.</li>
      </ul>
    </div>

    <p class="r-section">Experience</p>

    <div class="r-entry">
      <p class="r-role">Digital Forensics Analyst</p>
      <p class="r-company">Data Rescue Labs</p>
      <p class="r-dates">May 2026 – Present &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li><strong>Mobile Forensics & Device Acquisition:</strong> Perform iOS and Android extractions using Cellebrite Physical Analyzer and Magnet AXIOM on active criminal and civil cases; execute brute-force acquisitions on locked iPhones and Samsung devices using Cellebrite and Inseyets.</li>
        <li><strong>Email Evidence Extraction & eDiscovery:</strong> Process AD1 image files in Magnet AXIOM with keyword filters and date-range scoping; produce PST output via ForensicEmail Extractor for ingestion into Relativity eDiscovery platform; authored SOPs for repeatable export workflows.</li>
        <li><strong>Database & Deleted Data Recovery:</strong> Query SQLite databases (bugle_db for RCS messages, Telegram db_sqlite for crypto/chat recovery) using DB Browser and direct SQL; reconstruct investigative timelines; produce multi-page forensic reports for legal teams.</li>
        <li><strong>Storage Media Forensics:</strong> Image physically damaged SSDs, HDDs, and NVMe chips using PC-3000 and FTK Imager; apply SSD safe-mode techniques and thermostat analysis to assess hardware recoverability.</li>
        <li><strong>Registry & USB Artifact Analysis:</strong> Extract and analyze SOFTWARE/SYSTEM registry hives via Registry Explorer to determine USB device connection timestamps on BitLocker-encrypted NVMe devices.</li>
        <li><strong>Filesystem Timeline Analysis:</strong> Identify file deletion and overwrite history using $UsnJrnl (MFTECmd.exe), $MFT, and $LogFile.</li>
        <li><strong>Cross-Artifact Investigation:</strong> Trace findings across linked artifacts (messages→contacts→media) to build complete investigative narratives for civil cases.</li>
      </ul>
    </div>

    <div class="r-entry">
      <p class="r-role">IT Systems & Security Analyst</p>
      <p class="r-company">University of Toronto – Law Department</p>
      <p class="r-dates">September 2025 – Present &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li><strong>Incident Response & Forensics:</strong> Perform forensic-level macOS recovery (DFU mode) and file recovery using PhotoRec; conduct endpoint patching and firmware recovery across Windows and macOS device fleets.</li>
        <li><strong>Access Control & Compliance:</strong> Enforce MFA/2FA policies; lead endpoint security audits and account access reviews aligned to PIPEDA.</li>
        <li><strong>Vulnerability Management & Documentation:</strong> Diagnose and remediate endpoint, network, and printer vulnerabilities; author runbooks and SOPs for Threat Risk Assessments (TRAs).</li>
        <li><strong>AI & Automation:</strong> Deployed an MCP server integrated with Claude AI for workflow automation; engineered AI-assisted diagnostic workflow to eliminate a recurring printer configuration conflict.</li>
        <li>Deliver Tier 1–2 technical support to lawyers, faculty, and staff across macOS, Windows 10/11, printers, AV/Zoom systems, and campus hardware.</li>
      </ul>
    </div>

    <div class="r-entry">
      <p class="r-role">Software Developer</p>
      <p class="r-company">Moneris</p>
      <p class="r-dates">May 2022 – April 2023 &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li><strong>Fee Disclosure API:</strong> Designed and implemented end-to-end — pricing logic, request validation, authentication middleware, and release.</li>
        <li><strong>Access Control Engineering:</strong> Built API key authentication and request-validation layers (Spring Boot / Java); addressed OWASP Top 10 risks.</li>
        <li><strong>Secure Cloud Migration:</strong> Migrated legacy databases to Microsoft Azure; integrated analytics via Synapse and Power BI.</li>
        <li>Deployed containerized microservices on Kubernetes; optimized API response times with EhCache; wrote JUnit tests.</li>
      </ul>
    </div>

    <p class="r-section">Projects</p>
    <div class="r-entry">
      <p class="r-role" style="color:#60a5fa;"><a href="/projects/" style="color:#60a5fa;">→ See full projects page</a></p>
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

  <!-- ==================== HOSPITALITY TAB ==================== -->
  <div id="tab-hospitality" class="tab-content">

    <p class="r-section">About</p>
    <p class="r-about">
      Dedicated hospitality professional with 4+ years of experience across high-volume cocktail bars,
      nightlife venues, and fine dining. Currently bartending at Watson's with a strong background in
      bar operations, floor service, and team coordination. Experienced in staff training, cash handling,
      inventory management, and event service. Quick learner with a focus on guest experience and smooth operations.
    </p>

    <p class="r-section">Experience</p>

    <div class="r-entry">
      <p class="r-role">Bartender</p>
      <p class="r-company">Watson's</p>
      <p class="r-dates">September 2025 – Present &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li>Craft a full range of cocktails — classics, signature, and seasonal menus — maintaining consistency and presentation standards.</li>
        <li>Deliver bar and floor service in a fast-paced, service-focused environment ensuring exceptional guest experience.</li>
        <li>Manage bar prep including batching cocktails, juicing fresh citrus, preparing garnishes, and restocking supplies.</li>
        <li>Lead service during private events, producing continuous rounds while maintaining quality, speed, and workflow coordination.</li>
      </ul>
    </div>

    <div class="r-entry">
      <p class="r-role">Bartender</p>
      <p class="r-company">IDK Social Bar</p>
      <p class="r-dates">May 2025 – December 2025 &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li>Greeted and engaged guests in a high-volume nightlife setting, providing personalized and attentive service.</li>
        <li>Prepared and served cocktails, premade drinks, and beer on tap with precision and consistency.</li>
      </ul>
    </div>

    <div class="r-entry">
      <p class="r-role">Server</p>
      <p class="r-company">Daldongnae Korean BBQ</p>
      <p class="r-dates">July 2021 – August 2025 &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li>Progressed from Hostess/Busser to Server within 2 months through strong performance and dedication.</li>
        <li>Managed a 20-table section serving up to 80 guests per shift; exceeded 120 tables during peak hours.</li>
        <li>Trained and mentored new staff, ensuring consistent service standards and efficient onboarding.</li>
        <li>Assisted with cash handling, register closing, and balancing tills accurately.</li>
        <li>Independently managed morning shifts and collaborated with team during busy periods.</li>
      </ul>
    </div>

    <div class="r-entry">
      <p class="r-role">Server</p>
      <p class="r-company">Soos / Fat Choi Fine Dining</p>
      <p class="r-dates">May 2022 – March 2023 &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li>Maintained immaculate table settings and linens; reviewed reservations and guest notes prior to each shift.</li>
        <li>Provided personalized service accommodating guest preferences, allergies, and dietary requirements.</li>
        <li>Managed assigned sections serving parties from two to sixteen guests.</li>
      </ul>
    </div>

    <p class="r-section">Skills</p>
    <div class="skills-grid">
      <div>
        <p class="skill-group-title">Bar</p>
        <div class="skill-tags">
          <span class="skill-tag">Cocktail Crafting</span>
          <span class="skill-tag">Mixology</span>
          <span class="skill-tag">Batch Preparation</span>
          <span class="skill-tag">Beer on Tap</span>
          <span class="skill-tag">Bar Maintenance</span>
          <span class="skill-tag">Inventory Management</span>
        </div>
      </div>
      <div>
        <p class="skill-group-title">Service</p>
        <div class="skill-tags">
          <span class="skill-tag">Customer Service</span>
          <span class="skill-tag">Upselling</span>
          <span class="skill-tag">POS & Cash Handling</span>
          <span class="skill-tag">Fine Dining</span>
          <span class="skill-tag">Event Service</span>
          <span class="skill-tag">Staff Training</span>
        </div>
      </div>
      <div>
        <p class="skill-group-title">Strengths</p>
        <div class="skill-tags">
          <span class="skill-tag">Multitasking</span>
          <span class="skill-tag">Calm Under Pressure</span>
          <span class="skill-tag">Attention to Detail</span>
          <span class="skill-tag">Teamwork</span>
          <span class="skill-tag">Time Management</span>
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

  <!-- ==================== OTHER TAB ==================== -->
  <div id="tab-other" class="tab-content">

    <p class="r-section">Experience</p>

    <div class="r-entry">
      <p class="r-role">Mail Services Associate (Intern)</p>
      <p class="r-company">Foresters Financial</p>
      <p class="r-dates">May 2021 – August 2021 &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li>Performed data entry and documentation in Excel and PowerPoint, preparing progress reports for management.</li>
        <li>Printed, sorted, and organized confidential client insurance records with discretion.</li>
        <li>Supported office equipment setup and maintenance.</li>
      </ul>
    </div>

    <div class="r-entry">
      <p class="r-role">Pharmacy Assistant</p>
      <p class="r-company">Haber's Compounding Pharmacy &amp; Shoppers Drug Mart</p>
      <p class="r-dates">2019 – 2020 &nbsp;·&nbsp; Toronto, ON</p>
      <ul>
        <li>Created and updated patient records with accuracy, handling personal health information with discretion.</li>
        <li>Assisted pharmacists in preparing and dispensing medications per pharmacy protocols.</li>
        <li>Provided clear, courteous service in a regulated healthcare setting.</li>
      </ul>
    </div>

    <p class="r-section">Awards & Recognition</p>

    <div class="r-entry">
      <p class="r-role">High School Honour Roll</p>
      <p class="r-company">High School</p>
      <p class="r-dates">2016, 2017, 2018, 2019</p>
    </div>
    <div class="r-entry">
      <p class="r-role">Canadian Team Mathematics Contest — 3rd Place</p>
      <p class="r-company">CEMC</p>
      <p class="r-dates">Dec 2018</p>
    </div>
    <div class="r-entry">
      <p class="r-role">Euclid Contest — Group 2 &nbsp;/&nbsp; Canadian Senior Mathematics Contest — Group 2</p>
      <p class="r-company">CEMC</p>
      <p class="r-dates">2018</p>
    </div>
    <div class="r-entry">
      <p class="r-role">Cayley Contest — Group 4 &nbsp;/&nbsp; Canadian Senior Math Contest — Group 3 &nbsp;/&nbsp; Avogadro Exam — 73rd Percentile</p>
      <p class="r-company">CEMC / University of Waterloo</p>
      <p class="r-dates">2017</p>
    </div>
    <div class="r-entry">
      <p class="r-role">COMC Honour Roll &nbsp;/&nbsp; Canadian Intermediate Mathematics Contest — Group 3</p>
      <p class="r-company">CEMC</p>
      <p class="r-dates">2016 &amp; 2017</p>
    </div>

    <p class="r-section">Activities & Involvement</p>

    <div class="r-entry">
      <p class="r-role">Risk Management Chair</p>
      <p class="r-company">Alpha Kappa Delta Phi (aKDPhi) — University of Toronto</p>
      <p class="r-dates">Jan 2021 – Present</p>
      <ul>
        <li>Educated the Chapter on risk management through workshops covering Risk Management Policy, Criminal Liability, Alcohol & Drug Abuse, Fire Prevention, and Sexual Abuse & Harassment programs.</li>
      </ul>
    </div>
    <div class="r-entry">
      <p class="r-role">Fundraising Chair</p>
      <p class="r-company">Alpha Kappa Delta Phi (aKDPhi) — University of Toronto</p>
      <p class="r-dates">Jan 2021 – Present</p>
      <ul>
        <li>Organized Bubble Tea and Krispy Kreme fundraising events; created promotional materials and coordinated with stakeholders.</li>
      </ul>
    </div>
    <div class="r-entry">
      <p class="r-role">Manager</p>
      <p class="r-company">Korean Canadian University & Toronto Students' Association (KCUTSA)</p>
      <p class="r-dates">Sep 2019 – Present</p>
      <ul>
        <li>Streamlined event planning; designed event posters and managed electronic databases using Excel.</li>
      </ul>
    </div>

  </div>

</div>

<script>
  function switchTab(tab) {
    document.querySelectorAll(".tab-content").forEach(el => el.classList.remove("active"));
    document.querySelectorAll(".tab-btn").forEach(el => el.classList.remove("active"));
    document.getElementById("tab-" + tab).classList.add("active");
    event.target.classList.add("active");
  }
</script>
