---
layout: splash
title: "Research"
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
        <span class="project-title">Topological Transport Driven by Correlated Disorder</span>
        <div class="project-links-wrapper">
          <a href="/publications/" class="project-link">View Papers</a>
        </div>
      </div>
      <p class="project-description">
        Demonstrating that short-range magnetic correlations significantly influence the topological properties and anomalous Hall effect in Mn<sub>3</sub>Sn. We resolve this physics by combining neutron total scattering with Reverse Monte Carlo (RMC) modeling and magnetic PDF (mPDF) analysis.
      </p>
      <div class="project-tags">
        <span class="tag">Neutron Scattering</span>
        <span class="tag">Short-range Disorder</span>
        <span class="tag">Topological Physics</span>
        <span class="tag">ORNL</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/PRL_Mn3Sn.png" alt="Weyl Semimetal Structure">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Emergent Topological Phenomena</span>
        <div class="project-links-wrapper">
          <a href="/publications/" class="project-link">View Papers</a>
        </div>
      </div>
      <p class="project-description">
        Investigating magnetostructural transformations in Mn<sub>3</sub>Sn and Mn<sub>3</sub>Ga to induce intrinsic Weyl phase transitions and anomalous Hall effects. We utilize advanced neutron scattering to map magnetic domains under strain.
      </p>
      <div class="project-tags">
        <span class="tag">Neutron Scattering</span>
        <span class="tag">Topological Physics</span>
        <span class="tag">ORNL</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/ToC_JACS.png" alt="Weyl Semimetal Structure">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Phonon Spectra from Total Scattering</span>
        <div class="project-links-wrapper">
          <a href="https://github.com/Tsung-Han-Yang/rmc-phonon-dynamics" class="project-link" target="_blank">View Code</a>
          <a href="/publications/" class="project-link">Related Papers</a>
        </div>
      </div>
      <p class="project-description">
        Extracting dynamic information from static total scattering data using <strong>Reverse Monte Carlo (RMC)</strong>. This framework reconstructs the phonon density of states (DOS) by refining atomic configurations against PDF and $S(Q)$ data.
      </p>
      <div class="project-tags">
        <span class="tag">RMC Modeling</span>
        <span class="tag">Lattice Dynamics</span>
        <span class="tag">Neutron Scattering</span>
        <span class="tag">Python/C++</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/placeholder_phonon.png" alt="Phonon DOS Plot">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">High-Order Spin-Orbit States</span>
        <div class="project-links-wrapper">
          <a href="/publications/" class="project-link">View Papers</a>
        </div>
      </div>
      <p class="project-description">
        Investigating molecular spin-orbital fluctuations and Jahn-Teller driven ordering in cluster Mott insulators. This work identifies local symmetry breaking in GaTa<sub>4</sub>Se<sub>8</sub> using total scattering techniques.
      </p>
      <div class="project-tags">
        <span class="tag">Molecular Clusters</span>
        <span class="tag">Jahn-Teller Effect</span>
        <span class="tag">PDF Analysis</span>
        <span class="tag">Neutron Scattering</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/PRR_GTS.png" alt="Cluster Mott Insulator">
    </div>
  </div>

</div>