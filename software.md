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
  .software-subtitle {
    color: #4facfe;
    font-size: 0.9rem;
    line-height: 1.45;
    margin: -4px 0 12px 0;
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

  <p class="software-description" style="margin: 0 0 0.5rem 0; max-width: 920px;">
    Browser-first research tools for structure refinement, RMC analysis, neutron diffuse scattering, and phonon dynamics, plus early experiments in agentic AI for materials. These projects emphasize local data privacy, interactive visualization, and deployable workflows that can run directly from GitHub Pages when the science allows it.
  </p>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">NEBULA3D</span>
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/nebula3d/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/nebula3d" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-subtitle">
        Neutron Elastic Background Utilities for Local Analysis &amp; 3D-delta PDF.
      </p>
      <p class="software-description">
        A Python toolkit and hosted browser console for cleaning 3D reciprocal-space neutron diffuse scattering volumes and preparing 3D-ΔPDF analysis products from Mantid-style HKL data.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Weak diffuse signals can be buried under powder-ring backgrounds, sharp Bragg and satellite peaks, radial pedestals, and transform artifacts before 3D-ΔPDF interpretation even begins.</li>
        <li><strong>Approach:</strong> The workflow unifies ring subtraction, Bragg/satellite punching, q-shell backfill, radial-background flattening, 3D-ΔPDF transforms, inverse-FFT consistency checks, and multi-view visual QA.</li>
        <li><strong>Value:</strong> It provides both full-resolution native workflows and a GitHub Pages web app that can run real pipeline stages client-side via Pyodide for modest volumes, making cleanup decisions inspectable and reproducible.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">React</span><span class="tag">Pyodide</span><span class="tag">Neutron Scattering</span><span class="tag">Diffuse Scattering</span><span class="tag">3D-ΔPDF</span><span class="tag">GitHub Pages</span>
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
        A no-install browser dashboard for RMCProfile, STOG, and EXAFS outputs. Select a local run folder to inspect refinement charts, KDE slices, folded 3D structures, and AI-guided summaries of model and fit details without uploading data.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> RMC validation spans plots, logs, structures, and fit metrics that are hard to inspect together during refinement.</li>
        <li><strong>Approach:</strong> The React/Vite app reads run folders locally, auto-detects outputs, renders interactive charts, and connects KDE, slab, and Three.js structure views.</li>
        <li><strong>Value:</strong> Live monitoring, figure export, EXAFS-aware plotting, WebGPU KDE, and an AI assistant help users understand model details, fit quality, and refinement diagnostics in one private dashboard.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">React/Vite</span><span class="tag">Python</span><span class="tag">AI Assistant</span><span class="tag">RMCProfile</span><span class="tag">EXAFS</span><span class="tag">WebGPU KDE</span><span class="tag">Three.js</span><span class="tag">Live Monitoring</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[RMC Fits Image]</span>
    </div>
  </div>

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
        A fully client-side phonon analysis app for RMCProfile ensembles. Open the hosted page, select a local run folder, and compute phonon band structures, animated 3D modes, simulated INS S(|Q|,E), and phonon DOS directly in the browser.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> RMC ensembles encode experimentally constrained local disorder, but translating those configurations into lattice-dynamical insight usually requires separate scripts, backends, or model assumptions.</li>
        <li><strong>Approach:</strong> The app extracts displacement-covariance phonons from the selected ensemble, runs the S(k) diagonalization on the user's machine with WebGPU, and keeps all files local through the browser folder picker.</li>
        <li><strong>Value:</strong> It turns RMC-derived structure into interactive dynamics: dispersion curves, soft-mode highlighting, 3D eigenvector animation, INS maps, DOS, fit-quality overlays, and phonopy-compatible exports without installing a scientific stack.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">React/Vite</span><span class="tag">WebGPU</span><span class="tag">RMCProfile</span><span class="tag">Phonons</span><span class="tag">INS</span><span class="tag">Client-side</span><span class="tag">GitHub Pages</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Phonon DOS Image]</span>
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">Web Refinement Workbench</span>
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/web-refinement/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/web-refinement" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-subtitle">
        Browser-native crystal &amp; magnetic structure refinement, built to be driven by people and AI agents alike.
      </p>
      <p class="software-description">
        A zero-install workbench that refines nuclear and magnetic structures from single-crystal and powder data in one shared least-squares engine, with a pure, tested TypeScript core designed to double as an agent tool and skill layer.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Starting a Rietveld or single-crystal refinement usually means choosing among several mature but heavy packages, each with its own data formats, workflows, and magnetic formalism, and some effectively Windows-only.</li>
        <li><strong>Approach:</strong> One browser app unifies single-crystal and powder, X-ray and neutron (constant-wavelength and time-of-flight), and nuclear and magnetic structures on a Levenberg–Marquardt engine with symmetry-adapted constrained parameters, a magnetic space-group and propagation-vector workflow, and a 3D structure and moment viewer.</li>
        <li><strong>Value:</strong> Nothing to install and data stays local; every scientific function is pure, tested TypeScript, so the same code that backs the UI can be exposed as agent tools, with fit quality judged by F<sub>obs</sub> vs F<sub>calc</sub> and residual plots rather than a single R-factor.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">TypeScript/React</span><span class="tag">Vite</span><span class="tag">Rietveld</span><span class="tag">Single-Crystal</span><span class="tag">Magnetic Structures</span><span class="tag">Three.js</span><span class="tag">Agent-Ready Core</span><span class="tag">GitHub Pages</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Refinement Workbench]</span>
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">matdiscover — Agentic AI for Materials <span style="font-weight: 400; color: #888;">(exploratory)</span></span>
        <a href="https://github.com/drthyang/agentic-ai-materials" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
      </div>
      <p class="software-subtitle">
        An early, exploratory prototype — a research direction I am actively learning in, not a finished tool.
      </p>
      <p class="software-description">
        A closed-loop experiment in whether an LLM agent can usefully drive materials screening: it states a hypothesis, proposes candidate compositions, screens them with physics-grounded surrogate models, reflects in a lab notebook, and iterates, running on local models by default.
      </p>
      <ul class="case-list">
        <li><strong>Question:</strong> Can an LLM agent that uses real domain tools, not just chat, meaningfully help decide which materials to try next, and can that help be measured rather than asserted?</li>
        <li><strong>Approach:</strong> A proposer LLM and an independent critic drive deterministic tools — charge-balance filters, CHGNet relaxation, convex-hull stability, MEGNet band gaps — with budgets enforced in code and every candidate logged to ground truth.</li>
        <li><strong>Honest status:</strong> A prototype under active development. Each campaign is benchmarked against non-LLM baselines (random and similarity) at equal compute, so "the agent helps" stays a claim with a control group, and often only a modest one. Treat the results as exploratory.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">LLM Agents</span><span class="tag">Ollama</span><span class="tag">CHGNet</span><span class="tag">Materials Project</span><span class="tag">Exploratory</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Discovery Loop]</span>
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
