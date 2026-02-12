---
layout: single
title: "Software & Open Source"
author_profile: true
classes: wide
---

<style>
  /* CSS for the Project Grid */
  .project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
    margin-top: 2rem;
  }

  .project-card {
    background: #fff;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 20px;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  /* Hover Effect for Interactivity */
  .project-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    border-color: #4facfe;
  }

  .project-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 10px;
    border-bottom: 1px solid #f0f0f0;
    padding-bottom: 10px;
  }

  .project-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #333;
  }

  .project-link {
    font-size: 0.85rem;
    color: #4facfe;
    text-decoration: none;
    font-weight: 600;
    border: 1px solid #4facfe;
    padding: 2px 8px;
    border-radius: 4px;
  }

  .project-link:hover {
    background: #4facfe;
    color: #fff;
  }

  .project-description {
    font-size: 0.95rem;
    color: #666;
    line-height: 1.5;
    margin-bottom: 15px;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .tag {
    font-size: 0.75rem;
    background: #f5f7fa;
    color: #555;
    padding: 3px 8px;
    border-radius: 4px;
    border: 1px solid #e1e4e8;
  }
</style>

<div class="project-grid">

  <div class="project-card">
    <div class="project-header">
      <span class="project-title">RMCprofile Post-Processing</span>
      <a href="https://github.com/Tsung-Han-Yang/your-repo-name" class="project-link">GitHub</a>
    </div>
    <p class="project-description">
        A comprehensive post-processing suite for RMCprofile simulations. Automates the visualization of model fits for PDF, S(Q), and Bragg profiles, while tracking simulation convergence diagnostics. Includes an interactive 3D viewer for exploring real-space atomic density distributions.
    </p>
    <div class="project-tags">
      <span class="tag">Python</span><span class="tag">RMCprofile</span><span class="tag">Data Analysis</span>
    </div>
  </div>

  <div class="project-card">
    <div class="project-header">
      <span class="project-title">RMC Phonon Dynamics</span>
      <a href="https://github.com/Tsung-Han-Yang/rmc-phonon-dynamics" class="project-link">GitHub</a>
    </div>
    <p class="project-description">
      Computational framework for extracting phonon density of states (DOS) and vibrational spectra directly from Reverse Monte Carlo structural models. Bridges the gap between static structure and dynamic properties.
    </p>
    <div class="project-tags">
      <span class="tag">Python</span><span class="tag">Lattice Dynamics</span><span class="tag">Scattering</span>
    </div>
  </div>

  <div class="project-card">
    <div class="project-header">
      <span class="project-title">Magnetic Pair Distribution Function Tools</span>
      <a href="https://github.com/Tsung-Han-Yang/mPDF-analysis-visualization" class="project-link">GitHub</a>
    </div>
    <p class="project-description">
      Developed and implemented a rigorous analytical framework to extract short-range magnetic correlations from total neutron scattering data using the magnetic Pair Distribution Function (mPDF) technique. Utilizing Benjamin Frandsen’s mPDF Python package, this project successfully resolved local magnetic structures in quantum materials where traditional Bragg diffraction failed to capture short-range disorder.
    </p>
    <div class="project-tags">
      <span class="tag">Python</span><span class="tag">Pandas</span><span class="tag">Scikit-learn</span>
    </div>
  </div>

  <div class="project-card">
    <div class="project-header">
      <span class="project-title">marketlab</span>
      <a href="https://github.com/Tsung-Han-Yang/marketlab" class="project-link">GitHub</a>
    </div>
    <p class="project-description">
      A Python-based toolkit for financial time-series analysis. Implements technical indicators and visualization for stock market data using modern data science libraries.
    </p>
    <div class="project-tags">
      <span class="tag">Python</span><span class="tag">Pandas</span><span class="tag">Scikit-learn</span>
    </div>
  </div>

</div>