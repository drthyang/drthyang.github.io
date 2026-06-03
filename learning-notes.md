---
layout: splash
title: "Learning Notes"
author_profile: true
classes: wide
header:
  overlay_image: /assets/images/museum-of-new-zealand-te-papa-tongarewa-S0rMoSd-VyI-unsplash.jpg
  overlay_filter: 0.5 # Darkens image by 50% so white text pops
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
---

<style>
  /* --- Header Styling --- */
  .section-header {
    margin-bottom: 3rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid #333;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .header-title {
    font-size: 2.5rem;
    font-weight: 800;
    color: #ffffff;
    margin: 0 0 0.5rem 0;
    line-height: 1.0;
  }

  .header-subtitle {
    margin-top: 20px;
    font-size: 0.85rem;
    color: #e0e0e0;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 500;
  }

  /* --- Main Container --- */
  .projects-container {
    max-width: 1200px;
    margin: 0 auto;
  }

  /* --- Card Styling (Grid Layout) --- */
  .project-card {
    background: rgba(255,255,255,0.03);
    border: 1px solid #333;
    border-radius: 8px;
    padding: 30px;
    margin-bottom: 40px;
    box-shadow: 0 6px 18px rgba(0,0,0,0.22);
    display: grid;
    grid-template-columns: 1fr 380px; /* Text takes space | Image fixed width */
    gap: 40px;
    align-items: start;
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  }

  .project-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 12px 24px rgba(0,0,0,0.35);
    border-color: #4facfe;
  }

  /* Left Column: Text Content */
  .project-content {
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  .project-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 20px;
    flex-wrap: wrap;
    gap: 10px;
  }

  .project-name {
    font-size: 1.5rem;
    font-weight: 700;
    color: #ffffff;
    margin: 0;
    line-height: 1.3;
  }

  /* Right Column: Figure */
  .project-figure {
    width: 100%;
    border-radius: 6px;
    overflow: hidden;
    border: 1px solid #333;
    background: #090909;
    min-height: 200px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .project-figure img {
    width: 100%;
    height: auto;
    display: block;
    object-fit: contain;
  }

  /* Buttons */
  .project-link {
    font-size: 0.75rem;
    color: #4facfe;
    text-transform: uppercase;
    font-weight: 700;
    letter-spacing: 0.5px;
    text-decoration: none;
    border: 1px solid #4facfe;
    padding: 6px 14px;
    border-radius: 4px;
    transition: all 0.2s ease;
  }

  .project-link:hover {
    background: #4facfe;
    color: #fff;
  }

  /* --- Detailed List Styling --- */
  .project-details {
    margin-bottom: 1.5rem;
  }

  .detail-item {
    margin-bottom: 0.8rem;
    line-height: 1.6;
    color: #b0b0b0;
    font-size: 0.95rem;
    display: flex; /* Aligns label next to text */
  }

  .detail-label {
    font-weight: 700;
    color: #ffffff;
    min-width: 130px; /* Ensures all labels align vertically */
    margin-right: 15px;
    flex-shrink: 0; /* Prevents label from squishing */
  }

  /* Tags */
  .stack-tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-top: auto;
  }

  .tech-tag {
    font-size: 0.75rem;
    background: rgba(79, 172, 254, 0.08);
    color: #d9ecff;
    padding: 4px 12px;
    border-radius: 4px;
    border: 1px solid rgba(79, 172, 254, 0.35);
    font-family: monospace;
    font-weight: 500;
  }

  /* Mobile Responsive */
  @media (max-width: 900px) {
    .project-card {
      grid-template-columns: 1fr;
      gap: 20px;
      padding: 20px;
    }
    .project-figure {
      order: -1; /* Image on top for mobile */
      margin-bottom: 15px;
    }
    .detail-item {
      flex-direction: column; /* Stack label above text on phones */
    }
    .detail-label {
      margin-bottom: 2px;
    }
  }
</style>

<div class="projects-container">

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <h3 class="project-name">Phonon Dynamics in Disordered Systems</h3>
        <a href="https://github.com/drthyang/rmc-phonon-dynamics" class="project-link" target="_blank" rel="noopener noreferrer">View on GitHub</a>
      </div>

      <div class="project-details">
        <div class="detail-item">
          <span class="detail-label">Methodology:</span>
          <span>Developed a high-performance numerical engine to calculate vibrational properties from <strong>Reverse Monte Carlo (RMC)</strong> structural models.</span>
        </div>
        <div class="detail-item">
          <span class="detail-label">Algorithm:</span>
          <span>Implemented <strong>Force Constant Matrix (Hessian)</strong> construction for large-scale disordered supercells, using finite-displacement methods, sparse numerical workflows, and Python/C++ kernels.</span>
        </div>
        <div class="detail-item">
          <span class="detail-label">Challenge:</span>
          <span>Optimized the computation of the <strong>Dynamic Structure Factor</strong> $S(Q, \omega)$ by parallelizing the Fourier transform of atomic trajectories across $10^5+$ coordinates.</span>
        </div>
        <div class="detail-item">
          <span class="detail-label">Impact:</span>
          <span>Enables direct comparison between theoretical atomic models and experimental Inelastic Neutron Scattering (INS) data for non-crystalline materials.</span>
        </div>
      </div>

      <div class="stack-tags">
        <span class="tech-tag">Python</span>
        <span class="tech-tag">NumPy</span>
        <span class="tech-tag">SciPy (Sparse)</span>
        <span class="tech-tag">C++ Kernels</span>
      </div>
    </div>
    
    <div class="project-figure">
      <img src="/assets/images/phonon-concept.svg" alt="Phonon Dynamics Visualization">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <h3 class="project-name">Materials Data & Scattering Workflows</h3>
        <a href="/research/" class="project-link">Research</a>
      </div>

      <div class="project-details">
        <div class="detail-item">
          <span class="detail-label">Overview:</span>
          <span>A learning and project track for building reproducible Python workflows around neutron scattering, PDF analysis, and atomistic model validation.</span>
        </div>
         <div class="detail-item">
          <span class="detail-label">Features:</span>
          <span>Includes fit diagnostics, model-comparison plots, local-structure summaries, and reusable Python analysis patterns for scattering-informed materials research.</span>
        </div>
      </div>

      <div class="stack-tags">
        <span class="tech-tag">Python</span>
        <span class="tech-tag">Neutron Scattering</span>
        <span class="tech-tag">Matplotlib</span>
        <span class="tech-tag">Model Validation</span>
        <span class="tech-tag">Materials Modeling</span>
      </div>
    </div>
    
    <div class="project-figure">
       <img src="/assets/images/rmc-fit-dashboard.svg" alt="Materials data workflow dashboard">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <h3 class="project-name">Physics-Informed Neural Networks</h3>
        <a href="/blog/" class="project-link">Related Notes</a>
      </div>

      <div class="project-details">
        <div class="detail-item">
          <span class="detail-label">Overview:</span>
          <span>A learning track for solving differential-equation and inverse-problem examples with neural networks constrained by physical residuals.</span>
        </div>
         <div class="detail-item">
          <span class="detail-label">Focus:</span>
          <span>Connects scientific modeling habits with modern ML: loss design, parameter inference, uncertainty checks, and physically meaningful validation.</span>
        </div>
      </div>

      <div class="stack-tags">
        <span class="tech-tag">PyTorch</span>
        <span class="tech-tag">Inverse Problems</span>
        <span class="tech-tag">Scientific ML</span>
        <span class="tech-tag">Optimization</span>
      </div>
    </div>
    
    <div class="project-figure">
       <img src="/assets/images/pinn_concept.svg" alt="Physics-informed neural network concept">
    </div>
  </div>

</div>
