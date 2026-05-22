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

  @media (max-width: 768px) { .core-grid { grid-template-columns: 1fr; } }
</style>

<div class="hero-summary">
  <h1 class="hero-title">Bridging Physics & Computation</h1>
  <!-- <p class="hero-subtitle">Postdoctoral Research Fellow @ Oak Ridge National Laboratory</p> -->
  
  <p style="font-size: 1.1rem; line-height: 1.6; color: #b0b0b0;">
      I bridge the gap between <strong>experimental physics</strong> and <strong>computational engineering</strong>. 
      By leveraging <strong>multi-modal scattering</strong> and <strong>high-performance analytics</strong>, 
      I build frameworks that transform noisy experimental data into predictive physical models.
    
  </p>
</div>

<div class="core-grid">
  <div class="core-card">
    <h3><i class="fas fa-microscope"></i> Quantum Materials</h3>
    <p>Investigating exotic phases, correlated disorder, and phonon dynamics in topological quantum systems through multi-modal scattering.</p>
    <div class="tag-container">
      <span class="mini-tag">Neutron Scattering</span>
      <span class="mini-tag">Correlated Disorder</span>
      <span class="mini-tag">Topology</span>
      <span class="mini-tag">Spin-orbit Coupling</span>
    </div>
    <br>
    <a href="/research/" style="text-decoration: none; font-weight: 600; color: #4facfe;">Explore Research Projects →</a>
  </div>

  <div class="core-card">
    <h3><i class="fas fa-code"></i> Scientific Software</h3>
    <p>Building robust tools for data inversion (RMC), molecular dynamics, and algorithmic modeling.</p>
    <div class="tag-container">
      <span class="mini-tag">C++17</span>
      <span class="mini-tag">Python (HPC)</span>
      <span class="mini-tag">Machine Learning</span>
    </div>
    <br>
    <a href="/software/" style="text-decoration: none; font-weight: 600; color: #4facfe;">View Packages & Tools →</a>
  </div>
</div>

<hr style="border: 0; border-top: 1px solid rgba(255,255,255,0.1); margin: 3rem 0;">

### Recent Highlights
* **[Publication]** *Intrinsic Topological Weyl Phase Transition...* — **Nat. Commun. (2026)**
* **[Software]** Released v2.1 of `rmc-phonon-dynamics` with improved MPI support.
* **[Note]** New learning notes on *Bayesian Optimization for Physics*.

<p align="center" style="margin-top: 4rem;">
  <a href="/assets/resume.pdf" class="btn btn--primary">Download Full CV</a>
</p>