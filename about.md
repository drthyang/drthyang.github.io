---
layout: single
title: "About Me"
permalink: /about/
author_profile: true
classes: wide
---

<style>
  /* Container to prevent text from getting too wide */
  .about-container {
    max-width: 800px;
    font-size: 1.1rem;
    line-height: 1.8;
    color: #b0b0b0;
  }



  /* Section Headings */
  .about-header {
    font-size: 1.5rem;
    font-weight: 700;
    color: #b0b0b0;
    margin-top: 2rem;
    margin-bottom: 1rem;
    border-left: 4px solid #4facfe;
    padding-left: 15px;
  }

  /* Skill Pills */
  .skill-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-bottom: 2rem;
  }
  
  .skill-tag {
    background: rgba(79, 172, 254, 0.08);
    border: 1px solid rgba(79, 172, 254, 0.35);
    padding: 5px 12px;
    border-radius: 6px;
    font-size: 0.9rem;
    color: #d9ecff;
    font-weight: 500;
  }
  .skill-group {
    margin-bottom: 1.2rem;
  }
  .skill-label {
    display: block;
    color: #ffffff;
    font-size: 0.95rem;
    font-weight: 700;
    margin-bottom: 0.55rem;
  }

  /* Strength Cards */
  .strength-card {
    background: rgba(255, 255, 255, 0.03);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    padding: 20px 25px;
    margin-bottom: 1.5rem;
    transition: transform 0.2s ease, border-color 0.2s ease;
  }
  .strength-card:hover {
    transform: translateY(-2px);
    border-color: rgba(79, 172, 254, 0.5);
    background: rgba(255, 255, 255, 0.05);
  }
  .strength-title {
    display: flex;
    align-items: center;
    color: #ffffff;
    font-size: 1.05rem;
    font-weight: 700;
    margin-bottom: 0.8rem;
    gap: 10px;
  }
  .strength-title::before {
    content: "▹";
    color: #4facfe;
    font-size: 1.2rem;
  }

  /* Highlight specific words */
  .highlight {
    color: #4facfe;
    font-weight: 600;
  }
</style>

<div class="about-container">

  <p>
    I am an experimental and computational materials scientist currently working as a Postdoctoral Researcher at Oak Ridge National Laboratory. My work sits at the intersection of advanced materials R&D, atomic-scale characterization, and physics-based modeling, with a focus on understanding how structure, disorder, magnetism, interfaces, and defects control material behavior.
  </p>
  <p>
    I specialize in designing and executing complex neutron and synchrotron scattering experiments, analyzing high-dimensional experimental datasets, and building computational workflows that translate noisy measurements into validated physical insight. My background spans quantum materials, magnetic and topological systems, thin films, metal-organic interfaces, STM/MBE surface science, crystal synthesis, local-structure analysis, DFT, Reverse Monte Carlo modeling, and Python/HPC-based scientific computing.
  </p>

  <div class="about-header">Industry Direction</div>
  <p>
    I am interested in industry roles where materials expertise, experimental problem-solving, and data-driven modeling support the development of next-generation technologies. My strongest fit is in materials R&D, quantum device materials, semiconductor-adjacent materials, advanced metrology, and scientific computing for complex physical systems.
  </p>
  <p>
    My goal is to translate deep research experience into practical R&D impact: connecting atomic-scale structure, disorder, interfaces, and defects to device-relevant material behavior, while building reproducible workflows that make complex characterization data more actionable for research and engineering teams.
  </p>

  <div class="about-header">Technical Strengths</div>
  
  <div class="strength-card">
    <span class="strength-title">Experimental Materials Research & Project Execution</span>
    <p style="margin-bottom: 0;">
      I design and execute neutron and synchrotron scattering experiments on quantum, magnetic, topological, and strongly correlated materials. My work includes proposal development, beamline execution, sample-environment planning, data-quality troubleshooting, and coordination with facility scientists and collaborators under time-sensitive experimental conditions.
    </p>
  </div>

  <div class="strength-card">
    <span class="strength-title">Materials Characterization, Synthesis & Experimental Systems</span>
    <p style="margin-bottom: 0;">
      My hands-on experience includes neutron/X-ray diffraction, total scattering/PDF, diffuse scattering, inelastic neutron scattering, STM/SP-STM, MBE thin-film growth, UHV systems, crystal synthesis, inert-atmosphere handling, cryogenic/high-pressure measurements, and custom experimental setup integration. I use these methods to connect structure, disorder, interfaces, magnetism, and defects to material behavior.
    </p>
  </div>

  <div class="strength-card">
    <span class="strength-title">Computational Modeling & Scientific Software</span>
    <p style="margin-bottom: 0;">
      I develop Python/C++ workflows for scientific data analysis, inverse modeling, and materials simulation. My work includes Reverse Monte Carlo analysis, PDF modeling, magnetic refinement, DFT, phonon calculations, symmetry analysis, HPC workflows, and reproducible experiment–simulation comparison.
    </p>
  </div>

  <div class="about-header">Technical Stack</div>
  
  <div class="skill-group">
    <span class="skill-label">Materials Characterization & Metrology</span>
    <div class="skill-grid">
      <span class="skill-tag">Neutron Scattering</span>
      <span class="skill-tag">Synchrotron X-ray Scattering</span>
      <span class="skill-tag">X-ray Diffraction</span>
      <span class="skill-tag">Total Scattering / PDF</span>
      <span class="skill-tag">Diffuse Scattering</span>
      <span class="skill-tag">Inelastic Neutron Scattering</span>
      <span class="skill-tag">STM / SP-STM</span>
      <span class="skill-tag">Surface Characterization</span>
      <span class="skill-tag">Low-Temperature / High-Pressure Measurements</span>
    </div>
  </div>

  <div class="skill-group">
    <span class="skill-label">Materials Synthesis & Experimental Systems</span>
    <div class="skill-grid">
      <span class="skill-tag">Crystal Growth</span>
      <span class="skill-tag">Solid-State Synthesis</span>
      <span class="skill-tag">Inert-Atmosphere Handling</span>
      <span class="skill-tag">MBE Thin-Film Growth</span>
      <span class="skill-tag">UHV Systems</span>
      <span class="skill-tag">Cryogenic Sample Environments</span>
      <span class="skill-tag">High-Pressure Sample Environments</span>
      <span class="skill-tag">Custom Experimental Setup Integration</span>
      <span class="skill-tag">National-Lab Beamtime Execution</span>
    </div>
  </div>

  <div class="skill-group">
    <span class="skill-label">Scientific Computing & Modeling</span>
    <div class="skill-grid">
      <span class="skill-tag">Python</span>
      <span class="skill-tag">C/C++</span>
      <span class="skill-tag">NumPy / SciPy / Pandas</span>
      <span class="skill-tag">scikit-learn</span>
      <span class="skill-tag">RMC / PDF Modeling</span>
      <span class="skill-tag">Monte Carlo Methods</span>
      <span class="skill-tag">Inverse Modeling</span>
      <span class="skill-tag">Numerical Optimization</span>
      <span class="skill-tag">DFT</span>
      <span class="skill-tag">Phonon Calculations</span>
      <span class="skill-tag">Magnetic / Crystallographic Refinement</span>
      <span class="skill-tag">Model Validation</span>
    </div>
  </div>

  <div class="skill-group">
    <span class="skill-label">Data & Research Workflows</span>
    <div class="skill-grid">
      <span class="skill-tag">HPC / SLURM</span>
      <span class="skill-tag">Linux / Bash</span>
      <span class="skill-tag">Git / GitHub</span>
      <span class="skill-tag">Reproducible Scientific Workflows</span>
      <span class="skill-tag">Signal Extraction</span>
      <span class="skill-tag">Scientific Visualization</span>
      <span class="skill-tag">Automated Analysis Pipelines</span>
      <span class="skill-tag">Experiment–Simulation Comparison</span>
    </div>
  </div>

  <div class="about-header">Education</div>
  <ul>
    <li><strong>Ph.D. in Physics</strong> — Brown University (Providence, RI)</li>
  </ul>

</div>
