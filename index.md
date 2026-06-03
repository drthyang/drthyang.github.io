---
layout: single
author_profile: true
classes: wide
---

<style>
  /* Hero Section */
  .hero-summary {
    padding: 2rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    margin-bottom: 3rem;
  }
  .hero-title { font-size: 2.2rem; font-weight: 800; margin-bottom: 0.5rem; color: #fff; }
  .hero-subtitle { font-size: 1.2rem; color: #4facfe; margin-bottom: 1.5rem; font-weight: 400; }
  .proof-strip {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 1.5rem;
  }
  .proof-item {
    border: 1px solid rgba(79, 172, 254, 0.45);
    color: #e8f4ff;
    background: rgba(79, 172, 254, 0.08);
    border-radius: 6px;
    padding: 0.45rem 0.7rem;
    font-size: 0.82rem;
    font-weight: 600;
  }
  .cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin-top: 1.5rem;
  }
  .cta-link {
    border: 1px solid #4facfe;
    border-radius: 5px;
    color: #4facfe;
    padding: 0.55rem 0.85rem;
    text-decoration: none;
    font-weight: 700;
  }
  .cta-link:hover { background: #4facfe; color: #0b0b0b; }

  /* Dual Core Grid */
  .core-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    margin-bottom: 3rem;
  }
  .core-card {
    background: rgba(255, 255, 255, 0.03);
    padding: 2rem;
    border-radius: 12px;
    border: 1px solid rgba(255, 255, 255, 0.05);
    transition: transform 0.2s ease;
  }
  .core-card:hover { transform: translateY(-5px); border-color: #4facfe; }
  .core-card h3 { margin-top: 0; color: #4facfe; }

  /* Quick Stats/Tags */
  .tag-container { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 1rem; }
  .mini-tag {
    font-size: 0.7rem;
    padding: 3px 8px;
    background: rgba(255,255,255,0.1);
    border-radius: 4px;
    color: #ccc;
  }
  .focus-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin: 0 0 3rem 0;
  }
  .focus-card {
    border-left: 3px solid #4facfe;
    padding: 0.9rem 1rem;
    background: rgba(255,255,255,0.025);
  }
  .focus-card strong { color: #fff; display: block; margin-bottom: 0.35rem; }
  .focus-card span { color: #b0b0b0; font-size: 0.92rem; line-height: 1.45; }

  @media (max-width: 768px) {
    .core-grid,
    .focus-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="hero-summary">
  <h1 class="hero-title">Experimental Quantum Materials Scientist</h1>
  <p class="hero-subtitle">Quantum material growth • synchrotron scattering • neutron scattering • local-structure analysis</p>
  
  <p style="font-size: 1.1rem; line-height: 1.6; color: #b0b0b0;">
      I grow, prepare, and characterize quantum materials to understand how local structure,
      magnetism, and lattice dynamics shape anomalous Hall transport, magnetic order,
      local symmetry breaking, and vibrational behavior. My experimental work
      uses <strong>synchrotron X-ray scattering</strong>, <strong>neutron scattering</strong>,
      and <strong>total-scattering/PDF analysis</strong>, supported by Python/C++ tools
      for RMC modeling, data analysis, and atomistic interpretation.
  </p>
  <div class="proof-strip">
    <span class="proof-item">Postdoctoral Researcher @ ORNL</span>
    <span class="proof-item">Ph.D. Physics @ Brown</span>
    <span class="proof-item">Material Growth & Characterization</span>
    <span class="proof-item">Synchrotron / Neutron Scattering</span>
    <span class="proof-item">Python / C++ Analysis Tools</span>
  </div>
  <div class="cta-row">
    <a href="/software/" class="cta-link">Technical Projects</a>
    <a href="/research/" class="cta-link">Research Portfolio</a>
    <a href="/publications/" class="cta-link">Publications</a>
  </div>
</div>

<div class="focus-grid">
  <div class="focus-card">
    <strong>Roles I am building toward</strong>
    <span>Materials scientist, experimental physicist, neutron scattering scientist, and quantum materials R&D roles in advanced characterization, scattering user facilities, and materials informatics-adjacent teams.</span>
  </div>
  <div class="focus-card">
    <strong>Technical strengths</strong>
    <span>Material growth, synchrotron/neutron scattering, local-structure analysis, RMC modeling, numerical methods, and reproducible Python/C++ data workflows.</span>
  </div>
  <div class="focus-card">
    <strong>Industry translation</strong>
    <span>Connect synthesis, characterization, and modeling to explain structure-property relationships in complex materials.</span>
  </div>
</div>

<div class="core-grid">
  <div class="core-card">
    <h3><i class="fas fa-microscope"></i> Quantum Materials</h3>
    <p>Growing, preparing, and characterizing quantum materials to investigate correlated disorder, local symmetry breaking, topology, and phonon dynamics.</p>
    <div class="tag-container">
      <span class="mini-tag">Neutron Scattering</span>
      <span class="mini-tag">Synchrotron Scattering</span>
      <span class="mini-tag">Material Growth</span>
      <span class="mini-tag">Correlated Disorder</span>
      <span class="mini-tag">Topology</span>
    </div>
    <br>
    <a href="/research/" style="text-decoration: none; font-weight: 600; color: #4facfe;">Explore Research Projects →</a>
  </div>

  <div class="core-card">
    <h3><i class="fas fa-code"></i> Computational Analysis</h3>
    <p>Building advanced Python/C++ workflows to analyze scattering data, refine atomistic models, and interpret local structure and dynamics.</p>
    <div class="tag-container">
      <span class="mini-tag">C++17</span>
      <span class="mini-tag">Python (HPC)</span>
      <span class="mini-tag">Scientific Computing</span>
    </div>
    <br>
    <a href="/software/" style="text-decoration: none; font-weight: 600; color: #4facfe;">View Packages & Tools →</a>
  </div>
</div>

<hr style="border: 0; border-top: 1px solid rgba(255,255,255,0.1); margin: 3rem 0;">

### Recent Highlights
* **[Publication]** First-author **Nature Communications (2026)** work linking a magnetostructural transformation to Weyl physics in Mn<sub>3</sub>Sn.
* **[Research]** **JACS (2024)** study revealing coupled antiferromagnetism and local symmetry breaking in kagome (Fe,Co)Sn.
* **[Tools]** Advanced Python/C++ analysis workflows for RMC modeling, local structure, phonon dynamics, and magnetic correlations.

<p align="center" style="margin-top: 4rem;">
  <a href="/assets/resume.pdf" class="btn btn--primary">Download Full CV</a>
</p>
