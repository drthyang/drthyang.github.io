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
    margin-top: 2.5rem;
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
    margin-bottom: 1.4rem;
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
    margin: 0.3rem 0 0 0;
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

  /* Highlight specific words */
  .highlight {
    color: #4facfe;
    font-weight: 600;
  }
</style>

<div class="about-container">

  <p>
    I am an experimental and computational materials scientist with <span class="highlight">15+ years of experience</span>, currently a Postdoctoral Researcher at Oak Ridge National Laboratory. I study how structure, disorder, and magnetism control the behavior of quantum materials — designing neutron and synchrotron scattering experiments, building the instruments and sample environments they need, and writing the software that turns noisy measurements into validated physical insight.
  </p>
  <p>
    That full-chain approach — synthesis, instrumentation, measurement, modeling, software — is the thread through my career: I have published <span class="highlight">first-author work in Nature Communications and JACS</span>, authored 10+ successful beamtime proposals as PI or lead contributor, built a high-pressure XRD capability from the ground up, and released three open-source scientific software packages.
  </p>
  <p>
    I am now looking toward industry R&D roles where this mix of hands-on experimentation, prototyping, and data-driven modeling helps develop next-generation technologies — materials R&D, quantum device materials, advanced metrology, and scientific computing for complex physical systems.
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
        Neutron-scattering studies of topological and correlated quantum materials across 9 SNS/HFIR instruments; open-source analysis software and Python/HPC workflows.
      </p>
    </div>
    <div class="timeline-entry">
      <span class="timeline-role">Ph.D. in Physics (Condensed Matter)</span><br>
      <span class="timeline-org">Brown University</span><span class="timeline-dates">2015 – 2023</span>
      <p class="timeline-desc">
        Spin-orbital physics of lacunar spinels; built a high-pressure (&gt;10 GPa), low-temperature XRD capability and crystal-synthesis workflows for a new quantum-materials lab.
      </p>
    </div>
    <div class="timeline-entry">
      <span class="timeline-role">Research Assistant</span><br>
      <span class="timeline-org">Academia Sinica</span><span class="timeline-dates">2013 – 2015</span>
      <p class="timeline-desc">
        DFT and NEGF quantum-transport modeling of metal-organic systems, in collaboration with STM experimental groups.
      </p>
    </div>
    <div class="timeline-entry">
      <span class="timeline-role">M.Sc. in Physics (Condensed Matter)</span><br>
      <span class="timeline-org">National Taiwan University</span><span class="timeline-dates">2010 – 2012</span>
      <p class="timeline-desc">
        MBE thin-film growth under UHV and atomic-scale surface magnetism by spin-polarized STM.
      </p>
    </div>
  </div>

  <div class="about-header">Toolbox</div>
  <div class="skill-grid">
    <span class="skill-tag">Neutron & Synchrotron Scattering</span>
    <span class="skill-tag">PDF / Diffuse / Inelastic</span>
    <span class="skill-tag">Crystal Growth</span>
    <span class="skill-tag">Diamond Anvil Cells</span>
    <span class="skill-tag">MBE / UHV / STM</span>
    <span class="skill-tag">DFT (Quantum ESPRESSO / VASP)</span>
    <span class="skill-tag">Phonopy</span>
    <span class="skill-tag">RMCProfile</span>
    <span class="skill-tag">Python / HPC</span>
    <span class="skill-tag">JAX / GPU Acceleration</span>
    <span class="skill-tag">Machine Learning</span>
  </div>

  <div class="about-header">Recognition</div>
  <ul>
    <li>Invited Speaker, American Crystallographic Association Annual Meeting (2025)</li>
    <li>Representative, ORNL Neutron Science Division DOE Research Highlight (2025)</li>
    <li>Invited Reviewer, <em>Nature Communications</em></li>
  </ul>

</div>
