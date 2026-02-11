---
layout: home
author_profile: true
title: Home
classes: wide
---

<style>
  .portfolio-section { max-width: 1000px; margin: 2rem auto; }
  
  .research-block { 
    margin-bottom: 4rem; 
    border-left: 3px solid #4facfe; 
    padding-left: 30px; 
  }

  .research-header { margin-bottom: 1.5rem; }
  .research-title { font-size: 1.4rem; font-weight: 800; color: #ffffff; }
  .industry-tag { 
    font-size: 0.75rem; background: #1a3a5a; color: #4facfe; 
    padding: 3px 10px; border-radius: 20px; font-weight: bold; margin-left: 10px;
    vertical-align: middle; border: 1px solid #4facfe;
  }

  .research-summary { color: #b0b0b0; line-height: 1.6; margin-bottom: 1rem; font-size: 1rem; }

  /* Compact Publication List within Research Block */
  .nested-pubs { background: #1a1a1a; padding: 15px; border-radius: 8px; }
  .nested-pub-item { font-size: 0.9rem; margin-bottom: 10px; color: #ccc; }
  .nested-pub-item strong { color: #fff; }
  .nested-pub-link { color: #4facfe; font-size: 0.8rem; text-decoration: none; margin-left: 10px; font-weight: bold; }
</style>

<div class="portfolio-section">

  <div class="research-block">
    <div class="research-header">
      <span class="research-title">Topological States & Correlated Disorder</span>
      <span class="industry-tag">QUANTUM COMPUTING</span>
    </div>
    <div class="research-summary">
      Applied high-dimensional data analysis to characterize <strong>Weyl phase transitions</strong> in Kagome magnets. Developed optimization routines to model magnetostructural coupling, with direct applications in designing robust quantum materials.
    </div>
    
    <div class="nested-pubs">
      <div class="nested-pub-item">
        <strong>Nat. Commun. (2026)</strong>: Intrinsic Topological Weyl Phase Transition...
        <a href="#" class="nested-pub-link">DOI</a>
      </div>
      <div class="nested-pub-item">
        <strong>J. Am. Chem. Soc. (2024)</strong>: Simultaneous Development of Antiferromagnetism...
        <a href="#" class="nested-pub-link">DOI</a>
      </div>
    </div>
  </div>

  <div class="research-block">
    <div class="research-header">
      <span class="research-title">Phonon Spectrum Construction (RMC Dynamics)</span>
      <span class="industry-tag">DATA SCIENCE / OPTIMIZATION</span>
    </div>
    <div class="research-summary">
      Built a Python-based computational framework using <strong>Reverse Monte Carlo (RMC)</strong> to reconstruct vibrational spectra from static scattering data. Solved inverse problems to extract dynamical properties from noisy experimental datasets.
    </div>

    <div class="nested-pubs">
      <div class="nested-pub-item">
        <strong>Phys. Rev. B (2024)</strong>: Jahn-Teller driven quadrupolar ordering...
        <a href="#" class="nested-pub-link">DOI</a>
      </div>
    </div>
  </div>

</div>
