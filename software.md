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

  .software-figure img,
  .software-figure video {
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
    Browser-first research tools for crystal &amp; magnetic structure refinement, RMC analysis, neutron diffuse scattering, phonon dynamics, and experiment planning, several with AI agents that work through the tools&#39; own analyses. These projects emphasize local data privacy, interactive visualization, and deployable workflows that can run directly from GitHub Pages when the science allows it.
  </p>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">MATERIA Workbench</span>
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/web-refinement/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/web-refinement" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-subtitle">
        Crystal and magnetic structure refinement that runs entirely in the browser.
      </p>
      <p class="software-description">
        A public-beta workbench for powder, single-crystal, and pair-distribution-function refinement with X-ray or neutron data, on one engine.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Refinement means choosing among several specialist packages, each with its own formats and conventions &mdash; a steep start before a first fit.</li>
        <li><strong>Approach:</strong> A tested TypeScript core (1,700+ tests), cross-checked against GSAS-II, FullProf, and PDFfit2, behind a guided workflow from data import to refined nuclear and magnetic structures.</li>
        <li><strong>Value:</strong> Nothing to install and data stays local. Fits report correlations and uncertainties, not just an agreement factor.</li>
        <li><strong>AI agent:</strong> An in-app Agent (Claude, or a local model on Ollama or LM Studio) reads the live fit and works through the page&#39;s own controls. You approve each change unless you turn on auto-approve, every change can be undone, and the refinement engine, not the model, sets every value. It follows method skills it reads when needed, and eval scenarios built from its past mistakes run in CI. The same core is open to other agents as 40 MCP tools.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">TypeScript</span><span class="tag">Rietveld</span><span class="tag">Single Crystal</span><span class="tag">PDF</span><span class="tag">Magnetic Structures</span><span class="tag">AI Agent</span><span class="tag">MCP Agent Tools</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/materia-workbench.png" alt="MATERIA Workbench — a converged two-phase Mn3Ga + MnO time-of-flight Rietveld refinement with observed/calculated/difference curves and the symmetry-allowed parameter table">
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">NeXus Viewer</span>
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/neutron-nexus-viewer/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/neutron-nexus-viewer" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-subtitle">
        Quick looks at 3D neutron scattering volumes, in the browser.
      </p>
      <p class="software-description">
        A no-install viewer for Mantid MDHistoWorkspace and 3D NXdata files, with reciprocal-space slices, line cuts, symmetry averaging, and artifact masking &mdash; then one click hands the cleaned volume to NEBULA3D.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> A first look at a 3D single-crystal volume usually means opening Mantid or writing one-off scripts.</li>
        <li><strong>Approach:</strong> Slices drawn in true reciprocal geometry from the UB matrix, and symmetry averaging applied exactly on the bin grid for any Laue class, with a check that the operations fit the cell.</li>
        <li><strong>Value:</strong> Opens a 401&sup3; volume in about 2 s with data kept local, compares two temperatures side by side, and exports a symmetrized, masked volume straight into NEBULA3D&#39;s 3D-ΔPDF pipeline.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">JavaScript</span><span class="tag">h5wasm</span><span class="tag">NeXus / Mantid</span><span class="tag">Symmetry Averaging</span><span class="tag">Diffuse Scattering</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/nexus-viewer.jpg" alt="NeXus Viewer comparing a synthetic crystal at 300 K and 10 K: HK and HL slices split along the diagonal, with 6/mmm symmetry averaging applied, showing diffuse short-range-order scattering at 300 K condensing into superlattice peaks at 10 K">
    </div>
  </div>

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
        Neutron Elastic Background Utility for Local Analysis and 3D-ΔPDF.
      </p>
      <p class="software-description">
        A Python toolkit and browser app that cleans 3D neutron diffuse-scattering data and computes 3D-ΔPDF maps.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Weak diffuse signal is often buried under powder rings, Bragg peaks, and background before any 3D-ΔPDF interpretation can begin.</li>
        <li><strong>Approach:</strong> One reproducible pipeline &mdash; powder-ring subtraction, Bragg-peak removal and backfill, background flattening, and the ΔPDF transform &mdash; with visual checks at each step.</li>
        <li><strong>Value:</strong> The same pipeline runs natively or entirely in the browser via Pyodide, so every cleanup decision is inspectable and repeatable.</li>
        <li><strong>AI agent:</strong> NEBULA Pilot, a panel beside every page, connects to a local or cloud model that grades each stage from metrics computed in the browser, measures the cuts it needs, and can run and tune the pipeline stage by stage &mdash; choosing only among a fixed set of settings, within hard limits.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">Pyodide</span><span class="tag">Neutron Scattering</span><span class="tag">Diffuse Scattering</span><span class="tag">3D-ΔPDF</span><span class="tag">AI Agent</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/nebula3d-delta-pdf.jpg" alt="NEBULA3D 3D-ΔPDF view of a synthetic rock-salt dataset: three linked orthogonal real-space cuts through the difference pair-distribution function, with window, contrast and colormap controls">
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">RMCProfile Workbench</span>
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/rmc-toolkits/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/rmc-toolkits" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-description">
        A no-install browser dashboard for RMCProfile: open a local run folder to review fits, structures, and atomic displacements without uploading data.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Judging an RMC refinement means reading plots, logs, structures, and fit metrics that live in separate files and tools.</li>
        <li><strong>Approach:</strong> Reads a run folder in place and brings fits, density maps, displacement analysis, and 3D structures into one view.</li>
        <li><strong>Value:</strong> Live monitoring while a run writes, and figure export.</li>
        <li><strong>AI agent:</strong> An optional AI Copilot on every page answers questions about the run by calling the Workbench&#39;s own analyses through tool calls, checks each result before using it, and ends with a verdict on whether the question was answered. Beta: built and tested, not yet tried with real models.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">React</span><span class="tag">RMCProfile</span><span class="tag">WebGPU</span><span class="tag">Three.js</span><span class="tag">AI Copilot</span><span class="tag">Live Monitoring</span>
      </div>
    </div>
    <div class="software-figure">
      <img src="/assets/images/rmcprofile-displacement-directions.jpg" alt="RMCProfile Workbench — the Displacement Directions view of a GaTa4Se8 RMC run: displacements for a Ta site binned in solid angle on a hex-tiled sphere, with fixed a/b/c axis views alongside and the site ellipsoids in the folded unit cell">
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
        A browser app that infers harmonic phonon band structures, animated modes, simulated neutron spectra, and DOS from RMCProfile ensembles.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> RMC models capture measured local disorder, but turning them into lattice dynamics usually takes separate scripts and a computing backend.</li>
        <li><strong>Approach:</strong> Derives phonons from the ensemble's displacement correlations and runs the heavy linear algebra on the user's GPU via WebGPU.</li>
        <li><strong>Value:</strong> Interactive dispersion curves, mode animation, and simulated INS with phonopy-style export &mdash; no scientific stack to install.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">React</span><span class="tag">WebGPU</span><span class="tag">RMCProfile</span><span class="tag">Phonons</span><span class="tag">INS</span>
      </div>
    </div>
    <div class="software-figure" style="background: #000;">
      <video autoplay loop muted playsinline poster="/assets/images/phonon-concept.svg" aria-label="Animated phonon eigenvector mode extracted from an RMC ensemble, rendered in 3D">
        <source src="/assets/images/phonon-mode.webm" type="video/webm">
        <source src="/assets/images/phonon-mode.mp4" type="video/mp4">
      </video>
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">NEXPLAN <span style="font-weight: 400; color: #888;">(work in progress)</span></span>
        <div style="display: flex; gap: 8px;">
          <a href="https://drthyang.github.io/nexplan/" class="software-link" target="_blank" rel="noopener noreferrer">Web App</a>
          <a href="https://github.com/drthyang/nexplan" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="software-subtitle">
        Neutron Experiment Planner: plan diffraction measurements from a crystal structure, in the browser.
      </p>
      <p class="software-description">
        A no-install planner for SNS diffraction experiments: reflections and structure factors from a CIF, powder patterns of NOMAD and POWGEN banks, TOPAZ and CORELLI measurement plans, and MDNorm binning.
      </p>
      <ul class="case-list">
        <li><strong>Problem:</strong> Planning a beamtime means working out, instrument by instrument, which reflections a setting records and what the data will resolve.</li>
        <li><strong>Approach:</strong> Instrument geometry from Mantid&#39;s instrument definitions and measured peak widths, with every formula and data source documented; geometry and relative Bragg intensities only.</li>
        <li><strong>AI agent:</strong> The same calculations are 26 tools for AI agents, served over MCP, including hand-offs that write inputs for MATERIA, NEBULA3D, and the NeXus Viewer.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">TypeScript</span><span class="tag">Experiment Planning</span><span class="tag">TOPAZ / CORELLI</span><span class="tag">NOMAD / POWGEN</span><span class="tag">MCP Agent Tools</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Experiment Planner]</span>
    </div>
  </div>

  <div class="software-card">
    <div class="software-content">
      <div class="software-header">
        <span class="software-title">Athanor — Agentic AI for Materials <span style="font-weight: 400; color: #888;">(exploratory)</span></span>
        <a href="https://github.com/drthyang/agentic-ai-materials" class="software-link" target="_blank" rel="noopener noreferrer">GitHub</a>
      </div>
      <p class="software-subtitle">
        An early, exploratory prototype — a research direction I am actively learning in, not a finished tool.
      </p>
      <p class="software-description">
        A closed-loop experiment: an LLM agent proposes candidate materials, screens them with physics-grounded surrogate models, and iterates on the results &mdash; on local models by default.
      </p>
      <ul class="case-list">
        <li><strong>Question:</strong> Can an LLM agent using real domain tools help decide which materials to try next &mdash; measurably, not anecdotally?</li>
        <li><strong>Approach:</strong> A proposer and an independent critic drive deterministic tools (CHGNet relaxation, convex-hull stability, band-gap models), with every candidate logged.</li>
        <li><strong>Honest status:</strong> An early prototype. Compared against non-LLM baselines under the same cap on relaxations, not matched on total compute &mdash; results are exploratory.</li>
      </ul>
      <div class="software-tags">
        <span class="tag">Python</span><span class="tag">LLM Agents</span><span class="tag">Ollama</span><span class="tag">CHGNet</span><span class="tag">Materials Project</span>
      </div>
    </div>
    <div class="software-figure" style="padding: 20px; text-align: center; color: #b0b0b0; border: 1px dashed #4facfe;">
      <span>[Discovery Loop]</span>
    </div>
  </div>


</div>
