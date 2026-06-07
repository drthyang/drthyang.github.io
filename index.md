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
    margin-bottom: 2.5rem;
  }
  .hero-title { 
    font-size: 1.8rem; 
    font-weight: 800; 
    margin-bottom: 0.5rem; 
    color: #fff; 
    line-height: 1.15;
  }
  .hero-subtitle { 
    font-size: 1.15rem; 
    color: #4facfe; 
    margin-bottom: 1.5rem; 
    font-weight: 400; 
    line-height: 1.4;
  }
  
  /* Target Roles Banner */
  .target-roles-banner {
    display: flex;
    align-items: center;
    gap: 12px;
    background: rgba(79, 172, 254, 0.05);
    border-left: 4px solid #4facfe;
    padding: 0.85rem 1.25rem;
    border-radius: 4px;
    margin: 1.8rem 0;
    font-size: 1.05rem;
    line-height: 1.6;
    color: #d8eaff;
  }
  .target-roles-banner strong {
    color: #ffffff;
    font-weight: 700;
  }

  .proof-strip {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 1.5rem;
  }
  .proof-item {
    border: 1px solid rgba(79, 172, 254, 0.3);
    color: #e2f1ff;
    background: rgba(79, 172, 254, 0.06);
    border-radius: 6px;
    padding: 0.45rem 0.75rem;
    font-size: 0.9rem;
    font-weight: 600;
  }

  /* Single-Column Core Grid */
  .core-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    margin-bottom: 3rem;
  }
  .core-card {
    background: rgba(255, 255, 255, 0.02);
    padding: 1.8rem;
    border-radius: 8px;
    border: 1px solid rgba(255, 255, 255, 0.05);
    display: flex;
    flex-direction: column;
    height: 100%;
    transition: transform 0.3s ease, border-color 0.3s ease;
  }
  .core-card:hover {
    transform: translateY(-4px);
    border-color: rgba(79, 172, 254, 0.5);
  }
  .core-card h3 { 
    margin-top: 0; 
    color: #ffffff; 
    font-size: 1.4rem;
    font-weight: 700;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .core-card h3 i {
    color: #4facfe;
    font-size: 1.1rem;
  }
  .core-card p {
    font-size: 1.05rem;
    color: #b0b0b0;
    line-height: 1.6;
    margin-bottom: 1.5rem;
  }

  /* Tag/Link Container alignment */
  .card-footer {
    margin-top: auto;
  }
  .tag-container {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    margin-bottom: 1.2rem;
  }
  .mini-tag {
    background: rgba(79, 172, 254, 0.1);
    border: 1px solid rgba(79, 172, 254, 0.2);
    color: #d2e7ff;
    border-radius: 4px;
    font-family: 'SF Mono', Menlo, monospace;
    font-size: 0.75rem;
    padding: 3px 8px;
  }

  /* Responsive */
  @media (max-width: 900px) {
    .core-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="hero-summary">
  <h1 class="hero-title">Experimental & Computational Materials Scientist</h1>
  <p class="hero-subtitle">Quantum Materials &middot; Characterization & Metrology &middot; Structure&ndash;Property Analysis &middot; Scientific Computing</p>
  
  <p style="font-size: 1.1rem; line-height: 1.8; color: #b0b0b0; margin-bottom: 1rem;">
      I am an experimental and computational materials scientist specializing in quantum and functional materials. My work combines neutron and synchrotron scattering, advanced characterization, surface/interface science, and physics-based modeling to understand how structure, disorder, magnetism, interfaces, and defects control material behavior.
  </p>
  <p style="font-size: 1.1rem; line-height: 1.8; color: #b0b0b0; margin-bottom: 0;">
      I bring hands-on experience in national-lab experiments, crystal synthesis, STM/MBE surface science, local-structure analysis, Reverse Monte Carlo modeling, DFT, phonon calculations, and Python-based scientific workflows for complex materials data.
  </p>

  <div class="target-roles-banner">
    <span style="font-size: 1.15rem;">🎯</span>
    <span><strong>Target Roles:</strong> Materials Scientist &middot; R&D Engineer &middot; Metrology Scientist &middot; Data Scientist &middot; Applied Scientist</span>
  </div>
  
  {% comment %}
  <div class="proof-strip">
    <span class="proof-item">Postdoctoral Researcher @ ORNL</span>
    <span class="proof-item">Ph.D. Physics @ Brown</span>
    <span class="proof-item">Scientific Computing & Modeling</span>
    <span class="proof-item">Synchrotron & Neutron Scattering</span>
    <span class="proof-item">Python / C++ (HPC & Sparse Methods)</span>
  </div>
  {% endcomment %}
</div>

{% comment %}
<div class="core-grid">
  <!-- Pillar 1: Research -->
  <div class="core-card">
    <h3><i class="fas fa-atom"></i> Physics & Materials R&D</h3>
    <p>Leading experimental design, material growth, and high-throughput data collection runs at synchrotron and neutron user facilities.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">Neutron Scattering</span>
        <span class="mini-tag">Synchrotron X-ray</span>
        <span class="mini-tag">Crystal Growth</span>
        <span class="mini-tag">Correlated Disorder</span>
      </div>
      <a href="/research/" style="text-decoration: none; font-weight: 600; color: #4facfe; font-size: 0.92rem;">Explore Research Projects →</a>
    </div>
  </div>

  <!-- Pillar 2: Software -->
  <div class="core-card">
    <h3><i class="fas fa-code"></i> Computational Modeling</h3>
    <p>Building high-performance Python/C++ software to solve inverse problems, accelerate calculations, and model complex physical systems.</p>
    <div class="card-footer">
      <div class="tag-container">
        <span class="mini-tag">C++17</span>
        <span class="mini-tag">Python (HPC)</span>
        <span class="mini-tag">Inverse Problems</span>
        <span class="mini-tag">Sparse Methods</span>
      </div>
      <a href="/software/" style="text-decoration: none; font-weight: 600; color: #4facfe; font-size: 0.92rem;">View Packages & Tools →</a>
    </div>
  </div>
</div>
{% endcomment %}



### Recent Highlights
* [**[Software]**](/software/) **Neutron diffuse scattering tools for 3D-ΔPDF analysis released:** Developed a Python-based workflow for 3D-ΔPDF reconstruction and visualization, supporting analysis of local disorder and short-range correlations in complex materials.
* [**[Publication]**](/publications/) First-author **Nature Communications (2026)** study on Mn<sub>3</sub>Ga, revealing an intrinsic topological phase transition at room temperature driven by a magnetostructural transformation.
* [**[Software]**](/software/) **Released rmcph:** a data-processing pipeline and GUI for calculating phonon spectra from total scattering measurements and RMC model ensembles, with integrated tools for phonon processing and visualization.
* [**[Publication]**](/publications/) First-author **JACS (2024)** study on kagome (Fe,Co)Sn, revealing coupling between short-range local disorder and a long-range antiferromagnetic transition.

<p align="center" style="margin-top: 3.5rem;">
  <a href="/assets/resume.pdf" class="btn btn--primary">Download Full CV</a>
</p>

