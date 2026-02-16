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

.about-container p {
    text-align: justify;
    text-justify: inter-word;
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
    background: #f8f9fa;
    border: 1px solid #e9ecef;
    padding: 5px 12px;
    border-radius: 6px;
    font-size: 0.9rem;
    color: #555;
    font-weight: 500;
  }

  /* Highlight specific words */
  .highlight {
    color: #0366d6;
    font-weight: 600;
  }
</style>

<div class="about-container">

  <p>
    I am a <strong>Computational Physicist</strong> and <strong>Data Scientist</strong> currently working as a Postdoctoral Researcher at <span class="highlight">Oak Ridge National Laboratory (ORNL)</span>.
  </p>
  
  <p>
    My expertise lies in extracting signals from noise. Whether analyzing terabytes of neutron scattering data or modeling stochastic market trends, I build <strong>high-performance numerical tools</strong> to uncover hidden structures in complex systems.
  </p>

  <div class="about-header">Research & Technology</div>
  <p>
    My academic work focuses on <strong>Quantum Materials</strong>—specifically, how local disorder drives emergent phenomena like topological phase transitions. To solve these problems, standard software wasn't enough, so I built my own.
  </p>
  <p>
    I specialize in <strong>Reverse Monte Carlo (RMC)</strong> modeling and have developed open-source Python/C++ frameworks to reconstruct phonon dynamics from static experimental data.
  </p>

  <div class="about-header">Current Focus: Quantitative Finance & ML</div>
  <p>
    I am actively expanding my toolkit into <strong>Machine Learning</strong>, <strong>Data Science</strong>, and <strong>Quantum Computing</strong>. I am fascinated by the parallels between statistical mechanics and financial markets—both are governed by stochastic processes, correlations, and large-scale data analysis.
  </p>
  <p>
    I am currently developing <strong>MarketLab</strong>, a Python library for algorithmic trading strategy backtesting, applying the same rigor I use in physics to financial time-series analysis.
  </p>

  <div class="about-header">Technical Stack</div>
  <div class="skill-grid">
    <span class="skill-tag">Python (Pandas, NumPy, Scikit-learn)</span>
    <span class="skill-tag">C++</span>
    <span class="skill-tag">High-Performance Computing (HPC)</span>
    <span class="skill-tag">Monte Carlo Simulation</span>
    <span class="skill-tag">Neutron Scattering</span>
    <span class="skill-tag">Bayesian Optimization</span>
    <span class="skill-tag">Git / CI/CD</span>
  </div>

  <div class="about-header">Education</div>
  <ul>
    <li><strong>Ph.D. in Physics</strong> — Brown University (Providence, RI)</li>
  </ul>

</div>

