---
layout: splash
title: "Packages & Tools"
author_profile: true
classes: wide
header:
  overlay_image: /assets/images/josh-redd-u_RiRTA_TtY-unsplash.jpg
  overlay_filter: 0.0
  caption: "Photo by [Josh Redd](https://unsplash.com/@joshredd?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/gold-and-black-leather-textile-u_RiRTA_TtY?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)"
---

<style>
  /* Single Column Layout */
  .software-container {
    display: flex;
    flex-direction: column;
    gap: 30px; /* Space between projects */
    margin-top: 2rem;
  }

  .software-card {
    /* background: #fff; */
    border: 1px solid #333;
    border-radius: 8px;
    padding: 25px;
    display: flex; /* Makes content side-by-side */
    gap: 25px;
    align-items: flex-start;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  .software-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.08);
    border-color: #4facfe;
  }

  /* Left Side: Text Content */
  .software-content {
    flex: 1; /* Takes up remaining space */
  }

  /* Right Side: Figure/Image */
  .software-figure {
    flex: 0 0 300px; /* Fixed width of 300px for images */
    height: 180px;   /* Fixed height to keep it uniform */
    background-color: #f5f7fa; /* Placeholder gray background */
    border-radius: 6px;
    border: 1px solid #eee;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .software-figure img {
    width: 100%;
    height: 100%;
    object-fit: cover; /* Ensures image fills the box without stretching */
  }

  /* Header & Title */
  .software-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 12px;
    border-bottom: 1px solid #f0f0f0;
    padding-bottom: 10px;
  }

  .software-title {
    font-size: 1.3rem;
    font-weight: 700;
    color: #ffffff;
  }

  .software-link {
    font-size: 0.85rem;
    color: #4facfe;
    text-decoration: none;
    font-weight: 600;
    border: 1px solid #4facfe;
    padding: 4px 10px;
    border-radius: 4px;
    transition: all 0.2s;
  }

  .software-link:hover {
    background: #4facfe;
    color: #fff;
  }

  .software-description {
    font-size: 1rem;
    color: #b0b0b0;
    line-height: 1.6;
    margin-bottom: 15px;
  }

  /* Tag Styling (Kept exactly as you liked) */
  .project-tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-top: auto; /* Pushes tags to bottom if needed */
  }

  .tag {
    font-size: 0.75rem;
    background: #222;
    color: #888;
    padding: 4px 10px;
    border-radius: 4px;
    border: 1px solid #444;
  }

  /* Mobile Responsive: Stack them vertically on small screens */
  @media (max-width: 768px) {
    .software-card { flex-direction: column-reverse; } /* Image on top */
    .software-figure { flex: none; width: 100%; height: 200px; }
  }
</style>

<div class="software-container">

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">RMC Phonon Dynamics</span>
        <a href="https://github.com/Tsung-Han-Yang/rmc-phonon-dynamics" class="software-link">GitHub</a>
      </div>
      <p class="software-description">
        A computational framework for extracting phonon density of states (DOS) and vibrational spectra directly from Reverse Monte Carlo structural models. By operating without symmetry constraints, this algorithm robustly characterizes dynamics in disordered systems where traditional lattice methods fail.
      </p>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">Lattice Dynamics</span><span class="tag">Scattering</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/phonon_dos_placeholder.png" alt="Phonon DOS">
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">RMCprofile Atomic Density</span>
        <a href="https://github.com/Tsung-Han-Yang/your-repo-name" class="software-link">GitHub</a>
      </div>
      <p class="software-description">
        A comprehensive post-processing suite for RMCprofile simulations. Automates the visualization of model fits for PDF, S(Q), and Bragg profiles, while tracking simulation convergence diagnostics. Includes an interactive 3D viewer for exploring real-space atomic density distributions.
      </p>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">RMCprofile</span><span class="tag">Data Analysis</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/rmc_plot_placeholder.png" alt="RMC Fits">
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">Magnetic Pair Distribution Function</span>
        <a href="https://github.com/Tsung-Han-Yang/mPDF-analysis-visualization" class="software-link">GitHub</a>
      </div>
      <p class="software-description">
        Rigorous analytical framework for extracting short-range magnetic correlations from total neutron scattering data using mPDF. Successfully resolves local magnetic structures in quantum materials where traditional Bragg diffraction fails to capture disorder.
      </p>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">mPDF</span><span class="tag">Magnetism</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/mpdf_placeholder.png" alt="Magnetic PDF">
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">marketlab</span>
        <a href="https://github.com/Tsung-Han-Yang/marketlab" class="software-link">GitHub</a>
      </div>
      <p class="software-description">
        A Python-based toolkit for financial time-series analysis. Implements technical indicators and visualization for stock market data using modern data science libraries.
      </p>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">Pandas</span><span class="tag">Scikit-learn</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/stock_plot_placeholder.png" alt="Market Analysis">
    </div>
  </div>

</div>