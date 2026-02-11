---
layout: single
title: "Research"
author_profile: true
classes: wide
---

<style>
  .research-container {
    max-width: 1000px;
    margin: 2rem auto;
    color: #e0e0e0;
  }

  .project-card {
    margin-bottom: 3rem;
    padding-bottom: 2rem;
    border-bottom: 1px solid #333;
  }

  .project-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 10px;
    flex-wrap: wrap;
    gap: 10px;
  }

  .project-title {
    font-size: 1.25rem;
    font-weight: 700;
    color: #ffffff;
    line-height: 1.2;
  }

  .project-link {
    font-size: 0.8rem;
    color: #4facfe;
    text-transform: uppercase;
    font-weight: 600;
    letter-spacing: 0.05em;
    text-decoration: none;
    border: 1px solid #4facfe;
    padding: 3px 10px;
    border-radius: 4px;
    transition: all 0.2s ease;
  }

  .project-link:hover {
    background: #4facfe;
    color: #000;
  }

  .project-description {
    font-size: 1.0rem;
    color: #b0b0b0;
    line-height: 1.5;
    margin-bottom: 15px;
  }

  .project-tags {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }

  .tag {
    font-size: 0.75rem;
    background: #222;
    color: #888;
    padding: 2px 8px;
    border-radius: 3px;
    border: 1px solid #444;
  }

  @media (max-width: 768px) {
    .project-header { flex-direction: column; align-items: flex-start; }
    .project-title { font-size: 1.1rem; }
  }
</style>

<div class="research-container">

  <div class="project-card">
    <div class="project-header">
      <span class="project-title">Emergent Topological Phenomena in Correlated Disordered Systems</span>
      <a href="/publications/" class="project-link">View Papers</a>
    </div>
    <p class="project-description">
      Investigating magnetostructural transformations in Mn<sub>3</sub>Sn and Mn<sub>3</sub>Ga to induce intrinsic Weyl phase transitions and anomalous Hall effects.
    </p>
    <div class="project-tags">
      <span class="tag">Neutron Scattering</span>
      <span class="tag">Topological Physics</span>
      <span class="tag">ORNL</span>
    </div>
  </div>
<div class="project-card">
  <div class="project-header">
    <span class="project-title">Constructing Phonon Spectra from Total Scattering Measurements</span>
    <div class="project-links">
      <a href="https://github.com/Tsung-Han-Yang/rmc-phonon-dynamics" class="project-link" target="_blank">View Code</a>
      <a href="/publications/" class="project-link">Related Papers</a>
    </div>
  </div>
  
  <p class="project-description">
    Extracting dynamic information from static total scattering data using <strong>Reverse Monte Carlo (RMC)</strong> and <strong>Phonon Dynamics</strong> modeling. This framework allows for the reconstruction of the phonon density of states (DOS) and dispersion relations by refining atomic configurations against pair distribution function (PDF) and structure factor $S(Q)$ data.
  </p>

  <div class="project-tags">
    <span class="tag">RMC Modeling</span>
    <span class="tag">Lattice Dynamics</span>
    <span class="tag">Neutron Scattering</span>
    <span class="tag">Python/C++</span>
  </div>
</div>

<div class="project-card">
    <div class="project-header">
      <span class="project-title">High-Order Spin-Orbit Quantum States in Lacunar Spinels</span>
      <a href="/publications/" class="project-link">View Papers</a>
    </div>

    

    <p class="project-description">
      Investigating molecular spin-orbital fluctuations and Jahn-Teller driven ordering in cluster Mott insulators. This work focuses on identifying local symmetry breaking and quadrupolar ordering in GaTa<sub>4</sub>Se<sub>8</sub> and GaNb<sub>4</sub>Se<sub>8</sub> using total scattering techniques.
    </p>
    
    <div class="project-tags">
      <span class="tag">Molecular Clusters</span>
      <span class="tag">Jahn-Teller Effect</span>
      <span class="tag">PDF Analysis</span>
      <span class="tag">Neutron Scattering</span>
    </div>
  </div>

</div>