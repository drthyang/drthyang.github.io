---
layout: single
author_profile: true
classes: wide
---

<style>
  /* Hero Section */
  .hero-summary {
    padding: 2rem 0 1.5rem;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    margin-bottom: 2rem;
  }
  .hero-title {
    font-size: 1.8rem;
    font-weight: 800;
    margin-bottom: 0.5rem;
    color: #fff;
    line-height: 1.15;
  }
  .hero-subtitle {
    font-size: 1.15rem;
    color: #4facfe;
    margin-bottom: 1.5rem;
    font-weight: 400;
    line-height: 1.4;
  }
  .hero-lede {
    font-size: 1.08rem;
    line-height: 1.75;
    color: #b0b0b0;
    margin-bottom: 1rem;
    max-width: 62rem;
  }

  /* Target Roles Banner */
  .target-roles-banner {
    display: flex;
    align-items: center;
    gap: 12px;
    background: rgba(79, 172, 254, 0.05);
    border-left: 4px solid #4facfe;
    padding: 0.85rem 1.25rem;
    border-radius: 4px;
    margin: 1.5rem 0 1.2rem;
    font-size: 1.02rem;
    line-height: 1.6;
    color: #d8eaff;
  }
  .target-roles-banner strong {
    color: #ffffff;
    font-weight: 700;
  }

  /* Proof Strip */
  .proof-strip {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 1.2rem;
  }
  .proof-item {
    border: 1px solid rgba(79, 172, 254, 0.3);
    color: #e2f1ff;
    background: rgba(79, 172, 254, 0.06);
    border-radius: 6px;
    padding: 0.45rem 0.75rem;
    font-size: 0.88rem;
    font-weight: 600;
  }
  a.proof-item {
    text-decoration: none;
    transition: background 0.2s ease, border-color 0.2s ease;
  }
  a.proof-item:hover {
    background: rgba(79, 172, 254, 0.2);
    border-color: rgba(79, 172, 254, 0.7);
    color: #ffffff;
  }

  /* Section headers */
  .home-section-title {
    color: #fff;
    font-size: 1.35rem;
    font-weight: 700;
    margin: 0 0 0.3rem;
  }
  .home-section-sub {
    color: #8fa8bd;
    font-size: 0.95rem;
    margin: 0 0 1.3rem;
  }

  /* Pillar Strip */
  .pillar-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    grid-auto-rows: 1fr;
    gap: 1rem;
    margin-bottom: 2.5rem;
  }
  .pillar-card {
    background: rgba(255, 255, 255, 0.02);
    border: 1px solid rgba(255, 255, 255, 0.07);
    border-left: 3px solid rgba(79, 172, 254, 0.55);
    border-radius: 6px;
    padding: 1rem 1.1rem;
  }
  .pillar-card h4 {
    margin: 0 0 0.45rem;
    color: #fff;
    font-size: 0.98rem;
    font-weight: 700;
  }
  .pillar-card p {
    margin: 0;
    color: #a8b6c2;
    font-size: 0.9rem;
    line-height: 1.65;
  }
  .pillar-card .pillar-proof {
    margin-top: 0.75rem;
    color: #d2e7ff;
    font-size: 0.82rem;
    line-height: 1.5;
  }
  .pillar-proof strong {
    color: #ffffff;
  }
  .pillar-card {
    display: flex;
    flex-direction: column;
  }
  .pillar-link {
    margin-top: auto;
    padding-top: 0.7rem;
    font-size: 0.82rem;
    font-weight: 600;
    color: #4facfe;
    text-decoration: none;
  }
  .pillar-link:hover { text-decoration: underline; }

  /* App Card Grid */
  .app-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    grid-auto-rows: 1fr;
    gap: 1.2rem;
    margin-bottom: 2.5rem;
  }
  .core-card {
    background: rgba(255, 255, 255, 0.02);
    padding: 1.4rem 1.5rem;
    border-radius: 8px;
    border: 1px solid rgba(255, 255, 255, 0.07);
    display: flex;
    flex-direction: column;
    height: 100%;
    transition: transform 0.25s ease, border-color 0.25s ease;
  }
  .core-card:hover {
    transform: translateY(-4px);
    border-color: rgba(79, 172, 254, 0.5);
  }
  .core-card h3 {
    margin: 0 0 0.6rem;
    color: #ffffff;
    font-size: 1.12rem;
    font-weight: 700;
    font-family: 'SF Mono', Menlo, monospace;
  }
  .core-card p {
    font-size: 0.95rem;
    color: #b0b0b0;
    line-height: 1.6;
    margin-bottom: 1.1rem;
  }
  .card-footer { margin-top: auto; }
  .tag-container {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    margin-bottom: 1rem;
  }
  .mini-tag {
    background: rgba(79, 172, 254, 0.1);
    border: 1px solid rgba(79, 172, 254, 0.2);
    color: #d2e7ff;
    border-radius: 4px;
    font-family: 'SF Mono', Menlo, monospace;
    font-size: 0.72rem;
    padding: 3px 8px;
  }
  .card-links {
    display: flex;
    gap: 14px;
    align-items: center;
  }
  .card-links a {
    text-decoration: none;
    font-weight: 600;
    font-size: 0.9rem;
    color: #4facfe;
  }
  .card-links a.launch {
    background: rgba(79, 172, 254, 0.12);
    border: 1px solid rgba(79, 172, 254, 0.35);
    border-radius: 6px;
    padding: 0.35rem 0.8rem;
  }
  .card-links a.launch:hover { background: rgba(79, 172, 254, 0.25); }

  /* CTA row */
  .cta-row {
    display: flex;
    justify-content: center;
    gap: 14px;
    flex-wrap: wrap;
    margin-top: 3rem;
  }

  @media (max-width: 900px) {
    .app-grid {
      grid-template-columns: 1fr;
    }
  }
  @media (max-width: 768px) {
    .pillar-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="hero-summary">
  <h1 class="hero-title">AI for Science &times; Materials Physics</h1>
  <p class="hero-subtitle">Physics-Grounded ML & LLM Agents &middot; Scattering Data &middot; Disorder Modeling &middot; Scientific Software</p>

  <p class="hero-lede">
      I build ML and LLM tools that turn complex scattering data into discovery — grounded in real materials physics, from sample preparation and neutron/synchrotron/STM measurements to physics-based modeling. My niche is owning the path from material and measurement design to reproducible Python/browser/LLM workflows that produce defensible, structure-property insight rather than black-box predictions.
  </p>

  <div class="target-roles-banner">
    <span style="font-size: 1.15rem;">🎯</span>
    <span><strong>Target Roles:</strong> AI for Science / Materials Informatics &middot; Experimental/Computational Materials Scientist &middot; Materials R&D / Metrology Scientist</span>
  </div>

  <div class="proof-strip">
    <span class="proof-item">Postdoc @ ORNL (Spallation Neutron Source)</span>
    <a class="proof-item" href="/publications/">First-author: Nature Communications &middot; JACS →</a>
    <span class="proof-item">Neutron, synchrotron & STM measurements</span>
    <span class="proof-item">Open-source Python/WebGPU tools</span>
    <span class="proof-item">Local-first LLM analysis workflows</span>
  </div>
</div>

<h2 class="home-section-title">Capability map</h2>
<p class="home-section-sub">Sample → signal → model → software: a connected toolkit for turning hard materials data into decisions.</p>

<div class="pillar-grid">
  <div class="pillar-card">
    <h4>Synthesis & Sample Prep</h4>
    <p>Prepare crystals, polycrystalline samples, and thin films; tune synthesis routes; handle air-sensitive workflows; and screen sample quality before beamtime or surface measurements.</p>
    <p class="pillar-proof"><strong>Proof:</strong> Flux/CVT growth, glovebox synthesis, MBE prep.</p>
    <a class="pillar-link" href="/research/">Research projects →</a>
  </div>
  <div class="pillar-card">
    <h4>Scattering & Metrology</h4>
    <p>Design neutron, synchrotron, and STM measurements, then convert diffraction, PDF, diffuse, inelastic, low-temperature, and high-pressure data into structure-property constraints.</p>
    <p class="pillar-proof"><strong>Proof:</strong> ORNL/SNS; neutron, synchrotron, STM studies.</p>
    <a class="pillar-link" href="/publications/">Publications →</a>
  </div>
  <div class="pillar-card">
    <h4>Modeling & Interpretation</h4>
    <p>Use DFT, phonons, Reverse Monte Carlo, Rietveld/magnetic refinement, and symmetry analysis to test mechanisms for disorder, magnetism, topology, and lattice dynamics.</p>
    <p class="pillar-proof"><strong>Proof:</strong> Nature Communications, JACS, PRB/PRR studies.</p>
    <a class="pillar-link" href="/publications/">Publications →</a>
  </div>
  <div class="pillar-card">
    <h4>Scientific Software & AI</h4>
    <p>Build Python/HPC and browser-first tools with Pyodide/WebGPU/React, plus LLM agents for analysis review, retrieval-grounded reasoning, local inference, and evaluation.</p>
    <p class="pillar-proof"><strong>Proof:</strong> MATERIA, NEBULA3D, RMCProfile Monitor, rmc-phonon-dynamics.</p>
    <a class="pillar-link" href="/software/">Packages & tools →</a>
  </div>
</div>

<h2 class="home-section-title">Scientific software I ship</h2>
<p class="home-section-sub">Browser-first research tools for structure refinement and neutron/RMC/phonon analysis: local data, inspectable workflows, and reproducible outputs.</p>

<div class="app-grid">
  <div class="core-card">
    <h3>MATERIA</h3>
    <p>An AI-native workbench for crystal &amp; magnetic structure refinement in the browser — single-crystal + powder, X-ray + neutron, nuclear + magnetic on one engine, with the pure core exposed to LLM agents as MCP tools that assess fits and suggest next steps.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">Rietveld</span>
        <span class="mini-tag">Magnetic Symmetry</span>
        <span class="mini-tag">MCP Agents</span>
      </div>
      <div class="card-links">
        <a class="launch" href="https://drthyang.github.io/web-refinement/">Launch ▶</a>
        <a href="https://github.com/drthyang/web-refinement">GitHub</a>
      </div>
    </div>
  </div>

  <div class="core-card">
    <h3>NEBULA3D</h3>
    <p>Cleans 3D reciprocal-space neutron diffuse-scattering volumes and computes 3D-&Delta;PDF maps — the complete Python pipeline runs client-side via Pyodide, with an optional AI reasoning review where a local or cloud LLM grades the reduction quality.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">Pyodide</span>
        <span class="mini-tag">3D-&Delta;PDF</span>
        <span class="mini-tag">LLM Review</span>
      </div>
      <div class="card-links">
        <a class="launch" href="https://drthyang.github.io/nebula3d/">Launch ▶</a>
        <a href="https://github.com/drthyang/nebula3d">GitHub</a>
      </div>
    </div>
  </div>

  <div class="core-card">
    <h3>RMCProfile Monitor</h3>
    <p>Dashboard for RMCProfile/STOG refinements — live monitoring, space-group detection, WebGPU KDE slices, plus a built-in LLM assistant (local via Ollama/LM Studio or cloud) that reasons over your run and watches convergence.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">Local LLM</span>
        <span class="mini-tag">WebGPU</span>
        <span class="mini-tag">RMCProfile</span>
      </div>
      <div class="card-links">
        <a class="launch" href="https://drthyang.github.io/rmc-toolkits/">Launch ▶</a>
        <a href="https://github.com/drthyang/rmc-toolkits">GitHub</a>
      </div>
    </div>
  </div>

  <div class="core-card">
    <h3>rmc-phonon-dynamics</h3>
    <p>Phonon band structures, DOS, animated 3D modes, and simulated INS spectra extracted directly from RMC ensembles — with WebGPU compute shaders delivering the main ~100&times; speedup for phonon analysis.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">WebGPU</span>
        <span class="mini-tag">Phonons</span>
        <span class="mini-tag">INS</span>
      </div>
      <div class="card-links">
        <a class="launch" href="https://drthyang.github.io/rmc-phonon-dynamics/">Launch ▶</a>
        <a href="https://github.com/drthyang/rmc-phonon-dynamics">GitHub</a>
      </div>
    </div>
  </div>
</div>

<h2 class="home-section-title">📌 Recent highlights</h2>

* [**[Software]**](/software/) **MATERIA Workbench (public beta):** a browser-native, AI-native workbench for crystal & magnetic structure refinement — single-crystal and powder, X-ray and neutron, nuclear and magnetic on one engine — with MCP agent tools that let LLMs assess fits and drive the expert refinement loop.
* [**[Publication]**](/publications/) First-author **Nature Communications (2026)** study on Mn<sub>3</sub>Ga, revealing an intrinsic topological phase transition at room temperature driven by a magnetostructural transformation.
* [**[Software]**](/software/) **scattering-ai-sdk (early development):** an agentic AI layer for scattering science — modular agent skills, retrieval-grounded LLM reasoning, and evaluation harnesses, running fully offline with local models.
* [**[Software]**](/software/) **matdiscover (exploratory):** a closed-loop prototype testing whether an LLM agent can help drive materials screening with physics-grounded surrogates, benchmarked against non-LLM baselines — an early direction I am actively exploring.
* [**[Software]**](/software/) **Neutron diffuse scattering tools for 3D-ΔPDF analysis released:** Developed a Python-based workflow for 3D-ΔPDF reconstruction and visualization, supporting analysis of local disorder and short-range correlations in complex materials.
* [**[Publication]**](/publications/) First-author **JACS (2024)** study on kagome (Fe,Co)Sn, revealing coupling between short-range local disorder and a long-range antiferromagnetic transition.
* [**[Software]**](/software/) **Released rmcph:** a data-processing pipeline and GUI for calculating phonon spectra from total scattering measurements and RMC model ensembles, with integrated tools for phonon processing and visualization.

<div class="cta-row">
  <a href="/publications/" class="btn btn--primary">View Publications</a>
</div>
