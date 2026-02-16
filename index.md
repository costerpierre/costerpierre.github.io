---
layout: single
author_profile: true
---

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;0,700;1,400&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

<style>
  /* --- BASE STYLES --- */
  body { 
    background-color: #faf9f6; 
    color: #34495e; 
    font-family: 'Inter', sans-serif; 
    line-height: 1.6;
  }
  
  h1, h2, h3 { 
    font-family: 'Playfair Display', serif; 
    color: #2c3e50; 
  }

  /* Link Styling */
  a { text-decoration: none; color: #5a7d7c; font-weight: 600; transition: color 0.2s; }
  a:hover { color: #2c3e50; text-decoration: underline; }

  /* --- COPY EMAIL WIDGET (Single Line) --- */
  .copy-container {
    display: inline-flex;
    align-items: center;
    background: #f0f2f1;
    padding: 2px 8px;
    border-radius: 6px;
    border: 1px solid #dcdcdc;
    cursor: pointer;
    transition: all 0.2s ease;
    font-family: 'Inter', sans-serif;
    font-size: 0.9rem;
    color: #34495e;
    margin-left: 5px; /* Spacing from preceding text */
    vertical-align: middle;
  }
  .copy-container:hover { background: #e0e6e3; border-color: #5a7d7c; }
  .copy-container i { margin-left: 6px; font-size: 0.8rem; color: #5a7d7c; }
  
  /* Tooltip logic */
  .copy-container:active:after {
    content: "Copied!";
    position: absolute;
    transform: translateY(-25px);
    background: #2c3e50;
    color: white;
    padding: 2px 6px;
    font-size: 0.7rem;
    border-radius: 4px;
  }

  /* --- SECTION HEADERS --- */
  h2 { 
    font-size: 2rem; 
    border-bottom: 2px solid #dcdcdc; 
    padding-bottom: 10px; 
    margin-top: 50px; 
    margin-bottom: 35px;
  }

  /* --- RESEARCH STYLES --- */
  .working-paper {
    margin-bottom: 45px;
    padding-bottom: 25px;
    border-bottom: 1px dashed #e0e0e0;
  }

  .paper-title-main {
    font-family: 'Playfair Display', serif;
    font-size: 1.5rem;
    font-weight: 700;
    color: #2c3e50;
    display: block;
    margin-bottom: 6px;
    line-height: 1.3;
  }

  /* Work in Progress - Fixed "Heaviness" */
  .wip-item {
    margin-bottom: 30px; 
  }

  .paper-title-wip {
    font-family: 'Playfair Display', serif;
    font-size: 1.25rem; 
    font-weight: 600; 
    color: #2c3e50;
    display: block;
    margin-bottom: 4px;
    line-height: 1.4;
  }

  .coauthors { 
    display: block; 
    margin-top: 4px;
    margin-bottom: 8px;
    font-size: 1rem; 
    color: #7f8c8d; 
    font-style: italic; 
    font-weight: 400;
  }

  .status-badge {
    background-color: #5a7d7c;
    color: #fff;
    font-family: 'Inter', sans-serif;
    font-size: 0.65rem;
    padding: 2px 8px;
    border-radius: 4px;
    vertical-align: middle;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    margin-left: 8px;
  }

  /* --- ABSTRACT TOGGLE --- */
  details { margin-top: 12px; }
  summary { 
    cursor: pointer; 
    color: #5a7d7c; 
    font-family: 'Inter', sans-serif;
    font-size: 0.9rem;
    font-weight: 600;
  }
  summary:hover { color: #2c3e50; }
  
  .abstract-content {
    margin-top: 10px;
    padding: 15px;
    background: #f4f4f4;
    border-left: 3px solid #5a7d7c;
    font-size: 0.95rem;
    text-align: justify;
    color: #444;
    line-height: 1.6;
  }

  /* --- TEACHING GRID --- */
  .teaching-grid {
    display: grid;
    grid-template-columns: 140px 1fr 1fr; 
    gap: 15px;
    align-items: baseline;
    margin-bottom: 15px;
    padding-bottom: 10px;
    border-bottom: 1px solid #eee;
  }
  
  .term { font-weight: bold; color: #5a7d7c; font-size: 0.9rem; }
  .course-name { font-weight: 700; color: #2c3e50; }
  .prof-info { font-size: 0.9rem; color: #666; font-style: italic; text-align: right; }
  
  @media (max-width: 700px) {
    .teaching-grid { grid-template-columns: 1fr; gap: 5px; }
    .prof-info { text-align: left; }
  }
</style>

<div id="about" markdown="1">
# About Me
I am a fourth-year PhD student in Economics at the **University of Southern California**. 

My research explores the dynamics of **International Trade**, **Spatial Economics**, and **Environmental Economics**.

Prior to USC, I studied at **SciencesPo Paris** and **UPF**, and gained professional experience at the **European Central Bank** and the **OECD**. You can view my [CV here](files/CV.pdf){:target="_blank"}. 

<p style="display: flex; align-items: center; gap: 8px; margin-top: 20px;">
  Feel free to reach out at: 
  <span class="copy-container" onclick="copyEmail()" title="Click to copy email">
    <span id="email-text">pcoster@usc.edu</span>
    <i class="fa-regular fa-copy"></i>
  </span>
</p>

<script>
function copyEmail() {
  const email = document.getElementById('email-text').innerText;
  navigator.clipboard.writeText(email);
}
</script>


<script>
function copyEmail() {
  const email = document.getElementById('email-text').innerText;
  navigator.clipboard.writeText(email);
}
</script>
</div>

---

<div id="research" markdown="1">
## Research

### Working Papers

<div class="working-paper">
  <a href="files/CdGM_CBAMleakage.pdf" class="paper-title-main" target="_blank">Firms' Supply Chain Adaptation to Carbon Taxes</a>
  <span class="coauthors">with <a href="https://julian.digiovanni.ca/" target="_blank">Julian di Giovanni</a> and <a href="https://www.isabellemejean.com/" target="_blank">Isabelle Méjean</a></span>
  
  <span style="font-size: 0.9rem;">
  <span class="status-badge">Submitted</span> &nbsp;|&nbsp; 
  <a href="https://cepr.org/publications/dp19644" target="_blank">CEPR Discussion Paper 19644</a> &nbsp;|&nbsp; 
  <a href="https://www.newyorkfed.org/research/staff_reports/sr1136" target="_blank">NY Fed Staff Report 1136</a>
  </span>

  <details>
  <summary>View Abstract</summary>
  <div class="abstract-content">
  This paper studies how firms adjust input sourcing in response to climate policy. Using the EU Emissions Trading System (ETS) as a natural experiment and French product-level import and production data, we show that firms increasingly shifted imports of ETS-regulated inputs to non-EU countries over the 2010s as the policy became more stringent, indicating carbon leakage. This leakage is economically significant: the share of ETS-regulated products sourced from outside the EU rose by 4.3 percentage points after the ETS was implemented. Motivated by these empirical findings, we estimate a heterogeneous firm model using pre-ETS data. Simulating the model under a €100 carbon tax reproduces observed leakage, raises domestic prices and modestly reduces French emissions. Adding a carbon tariff similar to the EU’s Carbon Border Adjustment Mechanism (CBAM) reverses the leakage but further increases prices. The combined ETS+CBAM regime is seven times more effective than the ETS alone in reducing emissions.
  </div>
  </details>
</div>

### Work in Progress

<div class="wip-item">
  <span class="paper-title-wip">Demand for Clean Household Energy: LPG in Rural Ghana</span>
  <span class="coauthors">with <a href="https://sites.google.com/site/bkelseyjack" target="_blank">Kelsey Jack</a>, <a href="https://www.darbyjack.org/" target="_blank">Darby Jack</a>, <a href="https://dornsife.usc.edu/paulina-oliva/" target="_blank">Paulina Oliva</a>, and Georgette Owusu-Amankwah</span>
</div>

<div class="wip-item">
  <span class="paper-title-wip">Carbon Policies and Firm-to-Firm Networks</span>
  <span class="coauthors">with <a href="https://lauriesala.github.io/" target="_blank">Lauri Esala</a> and <a href="https://hubertmassoni.github.io/" target="_blank">Hubert Massoni</a></span>
</div>

<div class="wip-item">
  <span class="paper-title-wip">Climate Change Adaptation and Subsidies in Agriculture: Evidence From France</span>
</div>

<div class="wip-item">
  <span class="paper-title-wip">Firm Upgrading and A New Estimation of Product Quality</span>
</div>
</div>

---

<div id="teaching" markdown="1">
## Teaching

<div class="teaching-grid">
  <div class="term">Fall 2025 & <br>Spring 2026</div>
  <div class="course-name">Intermediate Macroeconomics</div>
  <div class="prof-info">Prof. Robert Dekle (Undergrad)</div>
</div>

<div class="teaching-grid">
  <div class="term">Spring 2025</div>
  <div class="course-name">Macroeconomic Theory II</div>
  <div class="prof-info">Profs. Pablo Kurlat & Andy Neumeyer (PhD)</div>
</div>

<div class="teaching-grid">
  <div class="term">Fall 2024</div>
  <div class="course-name">
    Introduction to Macroeconomics <br>
    <a href="files/evaluations_Fall_2024.pdf" target="_blank" style="font-size: 0.8rem; font-weight: normal;">[View Evaluations]</a>
  </div>
  <div class="prof-info">Prof. Lodovico Pizzati (Undergrad)</div>
</div>

<div class="teaching-grid">
  <div class="term">Spring 2024</div>
  <div class="course-name">Macroeconomic Bootcamp</div>
  <div class="prof-info">Prof. Pablo Kurlat (PhD Core)</div>
</div>

</div>