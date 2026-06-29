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
    align-items: flex-start;
    margin-bottom: 12px;
    border-bottom: 1px solid #f0f0f0;
    padding-bottom: 10px;
    flex-wrap: wrap;
    gap: 10px;
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
  .case-list {
    margin: 0 0 16px 0;
    padding: 0;
    list-style: none;
  }
  .case-list li {
    color: #b0b0b0;
    font-size: 0.92rem;
    line-height: 1.5;
    margin-bottom: 0.45rem;
  }
  .case-list strong {
    color: #ffffff;
    margin-right: 4px;
  }

  /* Tag Styling */
  .software-tags {
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
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/rmc-phonon-dynamics/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/rmc-phonon-dynamics" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-description">
        A computational framework for calculating phonon bands, eigenvectors, and inelastic neutron scattering spectra directly from Reverse Monte Carlo model ensembles.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Static total-scattering models capture local structural disorder but do not directly provide lattice-dynamical information. The goal is to extract physically meaningful phonon behavior from disordered atomistic configurations constrained by experimental scattering data.</li>
        <li><strong>Approach:</strong> The framework combines Python/C++ numerical workflows for large-supercell calculations, GPU acceleration with JAX, real/imaginary kernel decomposition, and sparse-matrix-based operations to improve computational efficiency.</li>
        <li><strong>Value:</strong> It connects total-scattering-derived structural models with phonon dynamics and INS observables, enabling comparison between disordered atomistic models and experimental vibrational spectra with substantially improved computational throughput.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">C++</span><span class="tag">GUI</span><span class="tag">RMC Modeling</span><span class="tag">Phonons</span><span class="tag">INS</span><span class="tag">GPU Acceleration</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Phonon DOS Image]</span>
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">Diffuse Scattering & 3D-ΔPDF</span>
        <a href="https://github.com/drthyang/neutron-diffuse" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
      </div>
      <p class="software-description">
        A comprehensive Python suite for advanced 3D reciprocal-space neutron diffuse scattering data processing, featuring background removal, Bragg punch/backfill, 3D-ΔPDF generation, and inverse 3D-FFT for robust consistency checks.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Weak diffuse signals are often obscured by powder-ring backgrounds, Bragg peaks, and other artifacts in raw volumetric scattering data.</li>
        <li><strong>Approach:</strong> The toolkit uses multi-stage processing workflows, Bragg peak removal and backfilling, reciprocal-space masking, background cleaning, and interactive GUI-based quality checks.</li>
        <li><strong>Value:</strong> It converts raw diffuse scattering volumes into cleaner 3D-ΔPDF-ready datasets, enabling more reliable analysis of local structural disorder, short-range magnetic correlations, and structure&ndash;property relationships in complex materials.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">Neutron Scattering</span><span class="tag">Diffuse Scattering</span><span class="tag">3D-ΔPDF</span><span class="tag">Data Processing</span><span class="tag">GUI</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[3D Diffuse Viewer]</span>
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">RMC Toolkits</span>
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/rmc-toolkits/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/rmc-toolkits" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-description">
        A comprehensive post-processing suite and web dashboard for RMCProfile and STOG outputs, featuring interactive plots, live data monitoring, and 3D atomic density visualization.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Interpreting RMC outputs is traditionally a fragmented and manual process. Researchers must juggle disconnected static plots, text logs, and external 3D viewers, creating a major bottleneck in validating structural models of complex materials.</li>
        <li><strong>Approach:</strong> The framework pairs a Python backend with a React/Vite frontend to deliver live folder monitoring, browser-native SVG charting, and a Three.js-powered interactive KDE slice viewer.</li>
        <li><strong>Value:</strong> It turns expert-level RMC post-processing into a faster, highly visual, and reproducible workflow for analyzing local structure, disorder, and atomistic correlations.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">React/Vite</span><span class="tag">Flask</span><span class="tag">Three.js</span><span class="tag">RMCProfile</span><span class="tag">KDE</span><span class="tag">Dashboard</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[RMC Fits Image]</span>
    </div>
  </div>

  {% comment %}
  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">Magnetic Pair Distribution Function</span>
        <a href="https://github.com/drthyang/mPDF-analysis-visualization" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
      </div>
      <p class="software-description">
        An analytical workflow for extracting short-range magnetic correlations from total neutron scattering data. This project extends the <code>diffpy.mpdf</code> package (developed by 
        <a href="https://doi.org/10.1107/S1600576722007257" target="_blank" rel="noopener noreferrer">Dr. Benjamin Frandsen</a>) 
        into a modular system for streamlined calculations.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> interpret diffuse magnetic signals that are not captured by average-structure diffraction alone.</li>
        <li><strong>Engineering:</strong> modular analysis scripts, parameterized calculations, model comparison, and visualization of short-range spin correlations.</li>
        <li><strong>Value:</strong> supports model comparison for complex magnetic disorder in quantum materials.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">mPDF</span><span class="tag">Signal Extraction</span><span class="tag">Model Validation</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Magnetic PDF Image]</span>
    </div>
  </div>
  {% endcomment %}

</div>
