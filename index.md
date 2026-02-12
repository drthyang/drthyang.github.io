---
layout: single
author_profile: true
#title: "Home"
classes: wide
---

<style>
  /* Container for the main content */
  .portfolio-container {
    max-width: 900px;
    margin: 0 auto;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  }

  /* The Research Card */
  .research-card {
    margin-bottom: 3.5rem;
    position: relative;
    padding-left: 20px; /* Space for the accent line */
  }

  /* The Sleek Accent Line */
  .research-card::before {
    content: "";
    position: absolute;
    left: 0;
    top: 5px;
    bottom: 5px;
    width: 2px;
    background: linear-gradient(to bottom, #4facfe, #00f2fe);
    border-radius: 2px;
    opacity: 0.7;
  }

  /* Header Section */
  .card-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    flex-wrap: wrap;
    margin-bottom: 1rem;
    gap: 10px;
  }

  .project-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: #f0f0f0; /* Soft White */
    margin: 0;
    letter-spacing: -0.5px;
  }

  /* Modern Pill Tag */
  .tech-tag {
    font-size: 0.7rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    color: #4facfe;
    background: rgba(79, 172, 254, 0.1);
    padding: 6px 12px;
    border-radius: 100px; /* Full pill shape */
    font-weight: 600;
    border: 1px solid rgba(79, 172, 254, 0.2);
  }

  /* Summary Text */
  .project-summary {
    color: #a0a0a0; /* Softer gray for readability */
    line-height: 1.7;
    font-size: 1.05rem;
    margin-bottom: 1.5rem;
    max-width: 95%;
  }

  .project-summary strong {
    color: #e0e0e0;
    font-weight: 600;
  }

  /* Publication List - Clean & Minimal */
  .pub-list {
    display: flex;
    flex-direction: column;
    gap: 12px;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    padding-top: 15px;
  }

  .pub-item {
    font-size: 0.95rem;
    color: #b0b0b0;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .pub-journal {
    color: #4facfe;
    font-weight: 700;
    white-space: nowrap;
    font-size: 0.9rem;
  }

  .pub-link {
    font-size: 0.75rem;
    text-transform: uppercase;
    color: #666;
    text-decoration: none;
    border: 1px solid #444;
    padding: 2px 8px;
    border-radius: 4px;
    transition: all 0.2s ease;
  }

  .pub-link:hover {
    color: #fff;
    border-color: #fff;
  }

  /* Responsive Mobile Tweak */
  @media (max-width: 600px) {
    .card-header { flex-direction: column; }
    .research-card::before { display: none; }
    .research-card { padding-left: 0; border-top: 2px solid #333; padding-top: 20px; }
  }

/* Figure Styling */
  .project-figure {
    width: 100%;
    max-width: 600px; /* Limits size on big screens */
    border-radius: 8px; /* Soft rounded corners */
    box-shadow: 0 4px 12px rgba(0,0,0,0.3); /* Subtle depth */
    margin: 1.5rem 0;
    border: 1px solid rgba(255,255,255,0.1);
  }
  
  .figure-caption {
    font-size: 0.85rem;
    color: #888;
    text-align: left;
    margin-top: -10px;
    margin-bottom: 2rem;
    font-style: italic;
  }  
</style>

<div class="portfolio-container">

  <div class="research-card">
    <div class="card-header">
      <h2 class="project-title">Topological States & Correlated Disorder</h2>
      <span class="tech-tag">Quantum Materials</span>
    </div>
    
    <img src="/assets/images/ToC_JACS.png" alt="Local Symmetry Breaking Plot" class="project-figure">
    <div class="figure-caption">Figure 1: Local symmetry breaking driven by a magnetic transition in Fe-doped CoSn.</div>

    <div class="project-summary">
      Applied high-dimensional data analysis to characterize <strong>Weyl phase transitions</strong> in Kagome magnets. Developed optimization routines to model magnetostructural coupling, with direct applications in designing robust quantum materials.
    </div>
    
    <div class="pub-list">
      <div class="pub-item">
        <span class="pub-journal">Nat. Commun. (2026)</span>
        <span>Intrinsic Topological Weyl Phase Transition in Kagome magnet...</span>
        <a href="https://doi.org/" class="pub-link">DOI</a>
      </div>
      <div class="pub-item">
        <span class="pub-journal">JACS (2024)</span>
        <span>Simultaneous Development of Antiferromagnetism...</span>
        <a href="https://doi.org/10.1021/jacs.4c09387" class="pub-link">DOI</a>
      </div>
    </div>
  </div>

  <div class="research-card">
    <div class="card-header">
      <h2 class="project-title">Phonon Spectrum Construction</h2>
      <span class="tech-tag">Data Science / Optimization</span>
    </div>
    
    <div class="project-summary">
      Built a Python-based computational framework using <strong>Reverse Monte Carlo (RMC)</strong> to reconstruct vibrational spectra from static scattering data. Solved inverse problems to extract dynamical properties from noisy experimental datasets.
    </div>

    <div class="pub-list">
      <div class="pub-item">
        <span class="pub-journal">Phys. Rev. Res. (2022)</span>
        <span>Bond Ordering and Molecular Spin-orbital Fluctuations...</span>
        <a href="https://doi.org/10.1103/PhysRevResearch.4.033123" class="pub-link">DOI</a>
      </div>
      <div class="pub-item">
        <span class="pub-journal">Phys. Rev. B (2024)</span>
        <span>Jahn-Teller driven quadrupolar ordering...</span>
        <a href="https://doi.org/10.1103/PhysRevB.109.144101" class="pub-link">DOI</a>
      </div>
    </div>
  </div>

  <div class="research-card">
    <div class="card-header">
      <h2 class="project-title">Exotic Quantum Phase in Lacunar Spinels</h2>
      <span class="tech-tag">Quantum Materials</span>
    </div>
    <img src="/assets/images/PRR_GTS.png" alt="Disorder-order transition" class="project-figure">
    <div class="figure-caption">Figure 3: Disorder-order transition in GaTa<sub>4</sub>Se<sub>8</sub>.</div>

    <div class="project-summary">
      Built a Python-based computational framework using <strong>Reverse Monte Carlo (RMC)</strong> to reconstruct vibrational spectra from static scattering data. Solved inverse problems to extract dynamical properties from noisy experimental datasets.
    </div>

    <div class="pub-list">
      <div class="pub-item">
        <span class="pub-journal">Phys. Rev. Res. (2022)</span>
        <span>Bond Ordering and Molecular Spin-orbital Fluctuations...</span>
        <a href="https://doi.org/10.1103/PhysRevResearch.4.033123" class="pub-link">DOI</a>
      </div>
      <div class="pub-item">
        <span class="pub-journal">Phys. Rev. B (2024)</span>
        <span>Jahn-Teller driven quadrupolar ordering...</span>
        <a href="https://doi.org/10.1103/PhysRevB.109.144101" class="pub-link">DOI</a>
      </div>
    </div>
  </div>


</div>