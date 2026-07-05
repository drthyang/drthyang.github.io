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

  /* Quick links */
  .about-links {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    margin: 1.5rem 0 0.5rem 0;
  }

  .about-link {
    font-size: 0.8rem;
    color: #4facfe;
    text-transform: uppercase;
    font-weight: 600;
    letter-spacing: 0.05em;
    text-decoration: none;
    border: 1px solid #4facfe;
    padding: 5px 14px;
    border-radius: 4px;
    white-space: nowrap;
    transition: all 0.2s ease;
  }

  .about-link:hover {
    background: #4facfe;
    color: #000;
  }

  /* Career timeline */
  .timeline {
    border-left: 2px solid rgba(79, 172, 254, 0.4);
    margin-left: 8px;
    padding-left: 25px;
  }

  .timeline-entry {
    position: relative;
    margin-bottom: 1.8rem;
  }

  .timeline-entry::before {
    content: "";
    position: absolute;
    left: -31px;
    top: 8px;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: #4facfe;
  }

  .timeline-role {
    color: #ffffff;
    font-weight: 700;
    font-size: 1.05rem;
  }

  .timeline-org {
    color: #4facfe;
    font-weight: 600;
    font-size: 0.95rem;
  }

  .timeline-dates {
    color: #777;
    font-size: 0.85rem;
    margin-left: 8px;
  }

  .timeline-desc {
    font-size: 0.98rem;
    line-height: 1.6;
    margin: 0.4rem 0 0 0;
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
    I am an experimental and computational materials scientist with <span class="highlight">15+ years of experience</span>, currently working as a Postdoctoral Researcher at Oak Ridge National Laboratory. My work sits at the intersection of advanced materials R&D, atomic-scale characterization, and physics-based modeling, with a focus on understanding how structure, disorder, magnetism, interfaces, and defects control material behavior.
  </p>
  <p>
    I specialize in designing and executing complex neutron and synchrotron scattering experiments, analyzing high-dimensional experimental datasets, and building computational workflows that translate noisy measurements into validated physical insight. I have published <span class="highlight">first-author research in Nature Communications and JACS</span>, authored 10+ successful peer-reviewed beamtime proposals as PI or lead contributor, and released three open-source scientific software packages. My background spans quantum materials, magnetic and topological systems, thin films, metal-organic interfaces, STM/MBE surface science, crystal synthesis, local-structure analysis, DFT, Reverse Monte Carlo modeling, and Python/HPC-based scientific computing.
  </p>

  <div class="about-links">
    <a href="/research/" class="about-link">Research</a>
    <a href="/software/" class="about-link">Software & Tools</a>
    <a href="/publications/" class="about-link">Publications</a>
    <a href="https://github.com/drthyang" class="about-link">GitHub</a>
  </div>

  <div class="about-header">Career Path</div>

  <div class="timeline">
    <div class="timeline-entry">
      <span class="timeline-role">Postdoctoral Research Fellow</span><br>
      <span class="timeline-org">Oak Ridge National Laboratory</span><span class="timeline-dates">2023 – Present</span>
      <p class="timeline-desc">
        Leading neutron-scattering investigations of topological, magnetic, and strongly correlated quantum materials across 9 SNS and HFIR instruments; building open-source analysis software and reproducible Python/HPC workflows that connect experiment with physics-based modeling.
      </p>
    </div>
    <div class="timeline-entry">
      <span class="timeline-role">Ph.D. Researcher — Condensed Matter Physics</span><br>
      <span class="timeline-org">Brown University</span><span class="timeline-dates">2015 – 2023</span>
      <p class="timeline-desc">
        Established core capabilities for a new quantum-materials laboratory: crystal synthesis, a custom-built high-pressure (&gt;10 GPa), low-temperature XRD capability, and DFT/phonon analysis workflows. Dissertation on spin-orbital fluctuations and unconventional quantum phases in lacunar spinels.
      </p>
    </div>
    <div class="timeline-entry">
      <span class="timeline-role">Research Assistant</span><br>
      <span class="timeline-org">Academia Sinica, Research Center for Applied Sciences</span><span class="timeline-dates">2013 – 2015</span>
      <p class="timeline-desc">
        DFT electronic-structure and NEGF quantum-transport modeling of metal-organic hybrid systems and spin-dependent transport, in close collaboration with STM experimental groups.
      </p>
    </div>
    <div class="timeline-entry">
      <span class="timeline-role">Graduate Research Assistant — M.Sc.</span><br>
      <span class="timeline-org">National Taiwan University</span><span class="timeline-dates">2010 – 2012</span>
      <p class="timeline-desc">
        Epitaxial thin-film growth by MBE and sputter deposition under UHV with in-situ RHEED, and atomic-scale surface magnetism studies by spin-polarized STM at low temperature.
      </p>
    </div>
  </div>

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
      My hands-on experience includes neutron/X-ray diffraction, total scattering/PDF, diffuse scattering, inelastic neutron scattering, STM/SP-STM, MBE thin-film growth, UHV systems, crystal synthesis, inert-atmosphere handling, cryogenic/high-pressure measurements, and custom experimental setup integration — including instrumentation I designed and built myself, from diamond-anvil-cell XRD setups to metal 3D-printed sample fixtures.
    </p>
  </div>

  <div class="strength-card">
    <span class="strength-title">Computational Modeling & Scientific Software</span>
    <p style="margin-bottom: 0;">
      I develop Python/C++ workflows for scientific data analysis, inverse modeling, and materials simulation. My work includes Reverse Monte Carlo analysis, PDF modeling, magnetic refinement, DFT, phonon calculations, symmetry analysis, HPC workflows, and reproducible experiment–simulation comparison — packaged into open-source tools like <a href="https://github.com/drthyang/nebula3d">nebula3d</a>, <a href="https://github.com/drthyang/rmc-toolkits">rmc-toolkits</a>, and <a href="https://github.com/drthyang/rmc-phonon-dynamics">rmc-phonon-dynamics</a>.
    </p>
  </div>

  <div class="about-header">Recognition</div>
  <ul>
    <li>Invited Speaker, American Crystallographic Association Annual Meeting (2025)</li>
    <li>Representative, ORNL Neutron Science Division DOE Research Highlight (2025)</li>
    <li>Invited Reviewer, <em>Nature Communications</em></li>
    <li>Invited Speaker, Argonne National Laboratory Materials Science Division Seminar (2023)</li>
    <li>National Best Master's Thesis Award, Taiwan Association for Magnetic Technology (2012)</li>
  </ul>

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
      <span class="skill-tag">PPMS / VSM / Hall Transport</span>
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
      <span class="skill-tag">In-situ RHEED</span>
      <span class="skill-tag">UHV Systems</span>
      <span class="skill-tag">Diamond Anvil Cells</span>
      <span class="skill-tag">Cryogenic Sample Environments</span>
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
      <span class="skill-tag">DFT (Quantum ESPRESSO / VASP)</span>
      <span class="skill-tag">Phonopy</span>
      <span class="skill-tag">RMCProfile</span>
      <span class="skill-tag">GSAS-II / FullProf / Mantid</span>
      <span class="skill-tag">Monte Carlo Methods</span>
      <span class="skill-tag">Inverse Modeling</span>
      <span class="skill-tag">Numerical Optimization</span>
      <span class="skill-tag">Magnetic / Crystallographic Refinement</span>
      <span class="skill-tag">Symmetry Analysis (ISODISTORT / Bilbao)</span>
      <span class="skill-tag">Model Validation</span>
    </div>
  </div>

  <div class="skill-group">
    <span class="skill-label">Data & Research Workflows</span>
    <div class="skill-grid">
      <span class="skill-tag">HPC / SLURM</span>
      <span class="skill-tag">Linux / Bash</span>
      <span class="skill-tag">Git / GitHub</span>
      <span class="skill-tag">JAX / GPU Acceleration</span>
      <span class="skill-tag">Interactive Dashboards (Flask / React)</span>
      <span class="skill-tag">Reproducible Scientific Workflows</span>
      <span class="skill-tag">Signal Extraction</span>
      <span class="skill-tag">Scientific Visualization</span>
      <span class="skill-tag">Automated Analysis Pipelines</span>
      <span class="skill-tag">Experiment–Simulation Comparison</span>
    </div>
  </div>

  <div class="about-header">Education</div>
  <ul>
    <li><strong>Ph.D. in Physics (Condensed Matter)</strong> — Brown University, 2023<br>
      <span style="font-size: 0.95rem; color: #999;">Dissertation: Spin-orbital Fluctuations and Unconventional Quantum Phases in Lacunar Spinels: Insights from Neutron and X-ray Scattering</span></li>
    <li><strong>M.Sc. in Physics (Condensed Matter)</strong> — National Taiwan University, 2012</li>
    <li><strong>B.Sc. in Physics</strong> — National Chung Hsing University, 2010</li>
    <li><strong>Certificate: Machine Learning Specialization</strong> — DeepLearning.AI & Stanford Online, 2025</li>
  </ul>

</div>
