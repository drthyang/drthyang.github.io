---
layout: splash
title: "Materials R&D & Scientific Computing"
author_profile: true
classes: wide
header:
  overlay_image: /assets/images/maria-oleacu-M-TI91UdTxs-unsplash.jpg
  overlay_filter: 0.0
  caption: "Photo by [Maria Oleacu](https://unsplash.com/@mari_oleacu?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/a-black-and-white-photo-of-sand-and-water-M-TI91UdTxs?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)"
---

<style>
  /* Main Container */
  .research-container {
    max-width: 1100px;
    margin: 2rem auto;
    color: #e0e0e0;
  }

  /* The Project Card (Now a wrapper for the grid) */
  .project-card {
    margin-bottom: 4rem; /* More space between projects */
    padding-bottom: 2rem;
    border-bottom: 1px solid #333;
    display: grid;
    grid-template-columns: 1fr 350px; /* Text takes rest, Image is 350px fixed */
    gap: 40px; /* Space between text and image */
    align-items: start;
  }

  /* Left Column: Text Content */
  .project-content {
    display: flex;
    flex-direction: column;
  }

  /* Right Column: Figure Wrapper */
  .project-figure {
    width: 100%;
    border-radius: 8px;
    overflow: hidden;
    background: #000; /* Placeholder background */
    border: 1px solid #333;
    box-shadow: 0 4px 12px rgba(0,0,0,0.5);
  }

  .project-figure img {
    width: 100%;
    height: auto;
    display: block;
    object-fit: cover;
  }

  /* Header Styling */
  .project-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 15px;
    flex-wrap: wrap;
    gap: 15px;
  }

  .project-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #ffffff;
    line-height: 1.2;
    margin: 0;
  }

  /* Link Styling (Kept exactly as you liked) */
  .project-links-wrapper {
    display: flex;
    gap: 10px;
  }

  .project-link {
    font-size: 0.8rem;
    color: #4facfe;
    text-transform: uppercase;
    font-weight: 600;
    letter-spacing: 0.05em;
    text-decoration: none;
    border: 1px solid #4facfe;
    padding: 4px 12px;
    border-radius: 4px;
    white-space: nowrap;
    transition: all 0.2s ease;
  }

  .project-link:hover {
    background: #4facfe;
    color: #000;
  }

  .project-description {
    font-size: 1.05rem;
    color: #b0b0b0;
    line-height: 1.6;
    margin-bottom: 20px;
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

  /* Mobile Responsive: Stack text over image */
  @media (max-width: 900px) {
    .project-card {
      grid-template-columns: 1fr; /* Single column */
      gap: 20px;
    }
    
    .project-figure {
      max-width: 100%;
      margin-top: 10px;
    }
    
    .project-header {
      flex-direction: column;
      align-items: flex-start;
    }
  }
</style>

<div class="research-container">

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Advanced Materials R&D</span>
      </div>
      <p class="project-description">
        Research on quantum materials, magnetic/topological systems, correlated crystals, thin films, and metal-organic interfaces, with a focus on how microscopic structure and interactions control functional material behavior.
      </p>
      <div class="project-tags">
        <span class="tag">Quantum Materials</span>
        <span class="tag">Topological Systems</span>
        <span class="tag">Correlated Crystals</span>
        <span class="tag">Thin Films</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/ToC_JACS.png" alt="Advanced Materials">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Materials Characterization & Metrology</span>
      </div>
      <p class="project-description">
        Advanced neutron/synchrotron scattering, diffraction, PDF, diffuse scattering, inelastic scattering, STM/SP-STM, and surface characterization under low-temperature, high-pressure, UHV, and specialized sample environments.
      </p>
      <div class="project-tags">
        <span class="tag">Neutron Scattering</span>
        <span class="tag">Synchrotron</span>
        <span class="tag">STM/SP-STM</span>
        <span class="tag">Diffuse Scattering</span>
      </div>
    </div>
    <div class="project-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Characterization Image]</span>
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Structure–Property & Defect Analysis</span>
      </div>
      <p class="project-description">
        Analysis of local disorder, lattice distortions, symmetry breaking, interfaces, magnetic order, and short-range correlations to understand performance-relevant material behavior.
      </p>
      <div class="project-tags">
        <span class="tag">Defect Analysis</span>
        <span class="tag">Local Disorder</span>
        <span class="tag">Magnetic Order</span>
        <span class="tag">Symmetry Breaking</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/PRR_GTS.png" alt="Defect Analysis">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Materials Synthesis, Thin Films & Experimental Systems</span>
      </div>
      <p class="project-description">
        Hands-on experience with crystal growth, inert-atmosphere synthesis, MBE thin-film growth, UHV systems, custom sample environments, cryogenic/high-pressure setups, and experimental integration.
      </p>
      <div class="project-tags">
        <span class="tag">MBE</span>
        <span class="tag">Crystal Growth</span>
        <span class="tag">UHV Systems</span>
        <span class="tag">Cryogenics</span>
      </div>
    </div>
    <div class="project-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Experimental Setup Image]</span>
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Scientific Computing & Physics-Based Modeling</span>
      </div>
      <p class="project-description">
        Python-based scientific workflows, RMC/PDF modeling, DFT, phonon calculations, magnetic refinement, symmetry analysis, HPC, and reproducible experiment–simulation comparison.
      </p>
      <div class="project-tags">
        <span class="tag">Python</span>
        <span class="tag">RMC Modeling</span>
        <span class="tag">DFT</span>
        <span class="tag">HPC</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/phonon-concept.svg" alt="Scientific Computing">
    </div>
  </div>

</div>
