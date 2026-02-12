---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
classes: wide
---

<div class="section-header">
  <!-- <h1 class="header">Projects</h1> -->
  <span class="header-subtitle">Machine Learning • Data Science • Quantum Computing</span>
</div>

<style>
  /* --- Header Styling --- */
  .section-header {
    margin-bottom: 3rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid #e0e0e0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .header-title {
    font-size: 2.5rem;
    font-weight: 800;
    color: #222;
    margin: 0 0 0.5rem 0;
    line-height: 1.0;
  }

  .header-subtitle {
    font-size: 0.85rem;
    color: #666;
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
    background: #fff;
    border: 1px solid #e1e4e8;
    border-radius: 12px;
    padding: 30px;
    margin-bottom: 40px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.04);
    display: grid;
    grid-template-columns: 1fr 380px; /* Text takes space | Image fixed width */
    gap: 40px;
    align-items: start;
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  }

  .project-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 12px 24px rgba(0,0,0,0.08);
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
    color: #2c3e50;
    margin: 0;
    line-height: 1.3;
  }

  /* Right Column: Figure */
  .project-figure {
    width: 100%;
    border-radius: 6px;
    overflow: hidden;
    border: 1px solid #eee;
    background: #fafafa;
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
    border-radius: 20px;
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
    color: #555;
    font-size: 0.95rem;
    display: flex; /* Aligns label next to text */
  }

  .detail-label {
    font-weight: 700;
    color: #333;
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
    background: #f1f8ff;
    color: #0366d6;
    padding: 4px 12px;
    border-radius: 12px;
    border: 1px solid #c8e1ff;
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
        <a href="https://github.com/rmc-phonon-dynamics" class="project-link" target="_blank">View on GitHub</a>
      </div>

      <div class="project-details">
        <div class="detail-item">
          <span class="detail-label">Methodology:</span>
          <span>Developed a high-performance numerical engine to calculate vibrational properties from <strong>Reverse Monte Carlo (RMC)</strong> structural models.</span>
        </div>
        <div class="detail-item">
          <span class="detail-label">Algorithm:</span>
          <span>Implemented <strong>Force Constant Matrix (Hessian)</strong> construction for large-scale disordered supercells, utilizing Finite Displacement Methods to derive the dynamical matrix.</span>
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
      <img src="/assets/images/placeholder_phonon.png" alt="Phonon Dynamics Visualization">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <h3 class="project-name">MarketLab: Quantitative Finance Toolkit</h3>
        <a href="https://github.com/Tsung-Han-Yang/marketlab" class="project-link" target="_blank">View on GitHub</a>
      </div>

      <div class="project-details">
        <div class="detail-item">
          <span class="detail-label">Overview:</span>
          <span>A modular Python framework for backtesting technical trading strategies and visualizing financial time-series data.</span>
        </div>
         <div class="detail-item">
          <span class="detail-label">Features:</span>
          <span>Includes automated calculating of technical indicators (SMA, RSI, MACD) and an extensible pipeline for testing algorithmic trading signals against historical market data.</span>
        </div>
      </div>

      <div class="stack-tags">
        <span class="tech-tag">Pandas</span>
        <span class="tech-tag">Matplotlib</span>
        <span class="tech-tag">Technical Analysis</span>
      </div>
    </div>
    
    <div class="project-figure">
       <img src="/assets/images/placeholder_market.png" alt="Market Analysis Dashboard">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <h3 class="project-name">Physics-informed Neural Network</h3>
        <a href="https://github.com/Tsung-Han-Yang/marketlab" class="project-link" target="_blank">View on GitHub</a>
      </div>

      <div class="project-details">
        <div class="detail-item">
          <span class="detail-label">Overview:</span>
          <span>A modular Python framework for backtesting technical trading strategies and visualizing financial time-series data.</span>
        </div>
         <div class="detail-item">
          <span class="detail-label">Features:</span>
          <span>Includes automated calculating of technical indicators (SMA, RSI, MACD) and an extensible pipeline for testing algorithmic trading signals against historical market data.</span>
        </div>
      </div>

      <div class="stack-tags">
        <span class="tech-tag">Pandas</span>
        <span class="tech-tag">Matplotlib</span>
        <span class="tech-tag">Technical Analysis</span>
      </div>
    </div>
    
    <div class="project-figure">
       <img src="/assets/images/placeholder_market.png" alt="Market Analysis Dashboard">
    </div>
  </div>

</div>