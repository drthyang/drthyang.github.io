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
    grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
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
    font-size: 0.86rem;
    line-height: 1.55;
  }

  /* App Card Grid */
  .app-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
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
</style>

<div class="hero-summary">
  <h1 class="hero-title">Experimental & Computational Materials Scientist</h1>
  <p class="hero-subtitle">Quantum Materials &middot; Synthesis & Crystal Growth &middot; Characterization & Metrology &middot; Scientific Computing</p>

  <p class="hero-lede">
      I study how structure, disorder, magnetism, interfaces, and defects control the behavior of quantum and functional materials — working across the full chain from crystal growth and solid-state synthesis, through neutron/synchrotron scattering and STM/MBE surface science, to DFT and phonon modeling, Reverse Monte Carlo analysis, and Python-based scientific workflows.
  </p>

  <div class="target-roles-banner">
    <span style="font-size: 1.15rem;">🎯</span>
    <span><strong>Target Roles:</strong> Materials Scientist &middot; R&D Engineer &middot; Metrology Scientist &middot; Data Scientist &middot; Applied Scientist</span>
  </div>

  <div class="proof-strip">
    <span class="proof-item">Postdoc @ ORNL (Spallation Neutron Source)</span>
    <span class="proof-item">Ph.D. Physics @ Brown</span>
    <span class="proof-item">First-author: Nat. Commun. &middot; JACS</span>
    <span class="proof-item">10+ beamtime proposals as PI</span>
    <span class="proof-item">Open-source scientific software</span>
  </div>
</div>

<h2 class="home-section-title">⚗️ From synthesis to software</h2>
<p class="home-section-sub">I work across the full materials pipeline — the same person who grows the crystal can model it, measure it, and ship the analysis tools.</p>

<div class="pillar-grid">
  <div class="pillar-card">
    <h4>Synthesis & Growth</h4>
    <p>Single-crystal growth (flux/CVT), polycrystalline synthesis, multi-zone furnaces, inert-atmosphere glovebox, high-pressure sample prep, MBE thin films with in-situ RHEED.</p>
  </div>
  <div class="pillar-card">
    <h4>Characterization</h4>
    <p>Neutron & synchrotron diffraction, total scattering/PDF, diffuse & inelastic scattering, STM/SP-STM, AFM, low-temperature & high-pressure environments.</p>
  </div>
  <div class="pillar-card">
    <h4>Modeling</h4>
    <p>DFT (Quantum ESPRESSO, VASP), Phonopy phonon calculations, Reverse Monte Carlo, Rietveld & magnetic refinement, symmetry analysis.</p>
  </div>
  <div class="pillar-card">
    <h4>Scientific Software</h4>
    <p>Python/HPC analysis pipelines, reproducible workflows, and browser-based tools (Pyodide, WebGPU, React) — see the live apps below.</p>
  </div>
</div>

<h2 class="home-section-title">🔬 Live scientific web apps</h2>
<p class="home-section-sub">Zero install — each app runs its full analysis pipeline in your browser. Your data never leaves your device.</p>

<div class="app-grid">
  <div class="core-card">
    <h3>nebula3d</h3>
    <p>Cleans 3D reciprocal-space neutron diffuse-scattering volumes and computes 3D-&Delta;PDF maps — the complete Python pipeline runs client-side via Pyodide at full float64 resolution.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">Pyodide</span>
        <span class="mini-tag">3D-&Delta;PDF</span>
        <span class="mini-tag">Diffuse Scattering</span>
      </div>
      <div class="card-links">
        <a class="launch" href="https://drthyang.github.io/nebula3d/">Launch ▶</a>
        <a href="https://github.com/drthyang/nebula3d">GitHub</a>
      </div>
    </div>
  </div>

  <div class="core-card">
    <h3>rmc-toolkits</h3>
    <p>Dashboard for RMCProfile/STOG refinements — live run monitoring, interactive charts, space-group detection, a 3D structure view, and a WebGPU-accelerated KDE up to ~100&times; faster.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">WebGPU</span>
        <span class="mini-tag">RMCProfile</span>
        <span class="mini-tag">React</span>
      </div>
      <div class="card-links">
        <a class="launch" href="https://drthyang.github.io/rmc-toolkits/">Launch ▶</a>
        <a href="https://github.com/drthyang/rmc-toolkits">GitHub</a>
      </div>
    </div>
  </div>

  <div class="core-card">
    <h3>rmc-phonon-dynamics</h3>
    <p>Phonon band structures, DOS, animated 3D modes, and simulated INS spectra extracted directly from RMC ensembles — computed on your GPU via WebGPU compute shaders.</p>
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

* [**[Publication]**](/publications/) First-author **Nature Communications (2026)** study on Mn<sub>3</sub>Ga, revealing an intrinsic topological phase transition at room temperature driven by a magnetostructural transformation.
* [**[Software]**](/software/) **Neutron diffuse scattering tools for 3D-ΔPDF analysis released:** Developed a Python-based workflow for 3D-ΔPDF reconstruction and visualization, supporting analysis of local disorder and short-range correlations in complex materials.
* [**[Publication]**](/publications/) First-author **JACS (2024)** study on kagome (Fe,Co)Sn, revealing coupling between short-range local disorder and a long-range antiferromagnetic transition.
* [**[Software]**](/software/) **Released rmcph:** a data-processing pipeline and GUI for calculating phonon spectra from total scattering measurements and RMC model ensembles, with integrated tools for phonon processing and visualization.

<div class="cta-row">
  <a href="/publications/" class="btn btn--primary">View Publications</a>
</div>
