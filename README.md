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

- <b>Safeguarding Sip: Drinking Water Quality Regulation, Monitoring and Surveillance in Latin America and the Caribbean</b> (forthcoming, IDB)  
  Measures how utilities oversample clean sites to avoid contamination penalties; efficiency and compliance patterns.

- <b>Knowledge in Every Drop: The Educational Costs of Drinking Water Contamination</b> (in progress, IDB)  
  Access to safe and reliable water is essential for human development, yet its broader educational implications remain poorly understood. This study investigates how variations in water quality affect learning outcomes in Brazil, where most households are connected to piped networks but contamination and service disparities persist. Using integrated administrative and survey data, we quantify the educational burden of water contamination—capturing both its direct health impacts and indirect effects on attendance and performance. By focusing on quality rather than mere access, the study reveals that lapses in water safety within “improved” systems impose significant and unequal costs on children’s learning, underscoring the need to view water governance as a cornerstone of human capital formation.

- <b> Strategic Oversampling and Regulatory Evasion in Brazil’s Water Sector /b> (in progress, IDB)  
  Water quality regulation in Brazil faces a persistent gap between formal standards and effective enforcement. Although national laws require regular monitoring, weak oversight and reliance on self-reporting allow providers to understate or omit violations, leading to systematic underreporting. This study investigates how these distortions bias official water quality data and obscure the true extent of contamination. Using a Heckman selection model and oversampling methods to correct for selection bias, we estimate the real incidence of water quality violations and identify socioeconomic and institutional factors associated with higher risks, showing that the burden of unsafe water is disproportionately borne by poorer communities.

- <b>Electoral Accountability and Deforestation: Investigating the connection between electoral incentives and deforestation in the Amazon Biome </b> (Master Dissetation, LSE)  
 Using a two-way fixed-effect strategy, we examine the influence of electoral incentives on deforestation within the Amazon biome, specifically focusing on mayoral re-election eligibility. Our focus is on the effects of the blacklist policy introduced in 2008 through a presidential decree. This policy socialises the cost of deforestation, allowing penalties at the municipal level. We hypothesised that the introduction of the blacklist policy resulted in deforestation becoming less appealing electorally. Using Brazil’s electoral rule, which allows a mayor to serve for only two consecutive terms, we identified mayors eligible for re-election. Our findings suggest that before 2008, mayors tended to deforest more during their initial term. However, the blacklist policy changed this dynamic, leading mayors to focus more on deforestation during their final term. We also explored scenarios where the blacklist policy might not serve as a credible threat, such as mayoral alignment with the federal government or deforestation happening in areas that are blind spots in Brazil’s monitoring system. Our findings do not provide any evidence that the blacklist policy changed the behaviour of mayors aligned with the federal government. We found evidence that the blacklist policy is ineffective in shifting mayoral behaviour in municipalities with dry forests, where monitoring tends to underestimate deforestation.

  </div>

</section>

<!-- CV TAB -->
<section id="cv" class="tab">
  <div class="card">
    <h3>Curriculum Vitae</h3>
    <p>
      Download the latest CV (PDF): <a href="./POLI_ACADEMIC_CV.pdf"><b>POLI_ACADEMIC_CV.pdf</b></a>
    </p>

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
