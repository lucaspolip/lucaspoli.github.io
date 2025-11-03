# lucaspoli.github.io

<!-- README for lucaspoli.github.io -->
<!-- CSS-only tabbed layout that works on GitHub Pages/Markdown -->

<style>
  /* Container */
  .tabs { max-width: 900px; margin: 0 auto; font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif; }
  .tabs h1 { text-align: center; margin-bottom: 0.25rem; }
  .subtitle { text-align: center; color: #555; margin: 0 0 1.25rem 0; }

  /* Top nav */
  .tab-nav { display: flex; gap: .5rem; justify-content: center; margin: 1rem 0 1.25rem; flex-wrap: wrap; }
  .tab-nav a {
    padding: .5rem .9rem; border: 1px solid #e1e4e8; border-radius: .6rem; text-decoration: none; color: #24292e;
    background: #fff;
  }
  .tab-nav a.active { background: #0969da; border-color: #0969da; color: #fff; }

  /* Sections */
  .tab { display: none; }
  .tab:target { display: block; }
  /* Default (no hash) -> show summary */
  .tab.default { display: block; }
  /* Card-ish bits */
  .card { border: 1px solid #e1e4e8; border-radius: .8rem; padding: 1rem; margin: 1rem 0; background: #fff; }
  .center { text-align: center; }
  .avatar { width: 160px; height: 160px; border-radius: 50%; object-fit: cover; border: 1px solid #e1e4e8; }
  .badges a { margin-right: .5rem; text-decoration: none; }
  .muted { color: #666; font-size: .95rem; }
</style>

<div class="tabs">

<h1>Lucas Poli</h1>
<p class="subtitle"><b>Research Consultant · Inter-American Development Bank</b><br>
Specializing in Water, Sanitation & Solid Waste Policy</p>

<p class="center badges">
  <a href="mailto:poli.lucasluiz@gmail.com">poli.lucasluiz@gmail.com</a> ·
  <a href="https://www.linkedin.com/in/lucas-poli">LinkedIn</a> ·
  <a href="https://scholar.google.com/">Google Scholar</a> ·
  <a href="https://github.com/lucaspoli">GitHub</a>
</p>

<!-- Nav uses :target; JS-free -->
<div class="tab-nav">
  <a href="#summary" id="link-summary">Summary</a>
  <a href="#research" id="link-research">Research</a>
  <a href="#cv" id="link-cv">CV</a>
</div>

<!-- SUMMARY TAB -->
<section id="summary" class="tab default">
  <div class="card center">
    <img src="./image.jpeg" alt="Portrait of Lucas Poli" class="avatar"><br>
    <p class="muted">Washington, DC · Portuguese · English · Spanish · German</p>
  </div>
  <div class="card">
    <h3>Summary</h3>
    <p>
      I am a political economist focused on <b>resilient infrastructure for water quality and sanitation</b> in Latin America and the Caribbean.
      My work examines how <b>institutional design, regulatory incentives, and behavioral factors</b> shape service continuity and environmental outcomes.
      At the Inter-American Development Bank, I co-author research on water contamination, utility efficiency, and strategic compliance.
    </p>
    <ul>
      <li><b>Focus:</b> Water quality, sanitation continuity, resilient infrastructure</li>
      <li><b>Methods:</b> Causal inference, policy synthesis, monitoring & data systems</li>
      <li><b>Current interests:</b> Last-mile sewer connections, continuity metrics, equity in WASH</li>
    </ul>
  </div>
</section>

<!-- RESEARCH TAB -->
<section id="research" class="tab">
  <div class="card">
    <h3>Selected Research</h3>

- <b>Strategic Oversampling and Regulatory Evasion in Brazil’s Water Sector</b> (forthcoming, IDB)  
  Measures how utilities oversample clean sites to avoid contamination penalties; efficiency and compliance patterns.

- <b>Water Contamination and Learning Outcomes in Brazil</b> (in progress, IDB)  
  Education impacts of contamination using administrative and assessment data.

- <b>Regulating Water Quality in Latin America and the Caribbean</b> (2024, IDB Flagship)  
  Regional assessment of standards vs. WHO guidelines; built an index for regulatory alignment.

- <b>Forecasting Urban Crime with Machine Learning</b> (Centre for Economic Performance, LSE)  
  > Reduced prediction MAPE from 25% to 3% using >1M observations.

  </div>

  <div class="card">
    <h4>Data & Code</h4>
    <ul>
      <li>Selected analysis and reproducible code will be linked here as public repos.</li>
    </ul>
  </div>
</section>

<!-- CV TAB -->
<section id="cv" class="tab">
  <div class="card">
    <h3>Curriculum Vitae</h3>
    <p>
      Download the latest CV (PDF): <a href="./LUCAS_POLI_ACADEMIC_CV.pdf"><b>LUCAS_POLI_ACADEMIC_CV.pdf</b></a>
    </p>
    <h4>Highlights</h4>
    <ul>
      <li><b>Current role:</b> Research Consultant – Inter-American Development Bank (Water, Sanitation & Solid Waste)</li>
      <li><b>Education:</b> MSc Political Economy (LSE, Distinction); BA Economics (PUC-SP); BA Social Science (USP)</li>
      <li><b>Skills:</b> R, Python, QGIS, SQL, LaTeX, Power BI, Tableau</li>
      <li><b>Languages:</b> Portuguese (Native), English (Fluent), Spanish (Intermediate), German (Basic)</li>
    </ul>
  </div>
</section>

</div>

<!-- Small helper so the active tab link looks highlighted without JS -->
<style>
  :target ~ .tab-nav a { /* reset */ }
  #summary:target ~ .tab-nav #link-summary,
  #research:target ~ .tab-nav #link-research,
  #cv:target ~ .tab-nav #link-cv { background:#0969da; border-color:#0969da; color:#fff; }
  /* When no hash, pretend Summary is active */
  .tab.default ~ .tab-nav #link-summary { background:#0969da; border-color:#0969da; color:#fff; }
</style>
