---
layout: splash
title: "Research — AI for Science × Quantum Materials"
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

  /* Intro lede */
  .research-lede {
    font-size: 1.08rem;
    line-height: 1.75;
    color: #b0b0b0;
    max-width: 62rem;
    margin: 0 0 3rem;
  }
  .research-lede strong {
    color: #ffffff;
  }

  /* The Project Card (text + figure grid) */
  .project-card {
    margin-bottom: 4rem;
    padding-bottom: 2rem;
    border-bottom: 1px solid #333;
    display: grid;
    grid-template-columns: 1fr 350px; /* Text takes rest, Image is 350px fixed */
    gap: 40px;
    align-items: start;
  }
  .project-card:last-of-type {
    border-bottom: none;
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
    background: #000;
    border: 1px solid #333;
    box-shadow: 0 4px 12px rgba(0,0,0,0.5);
  }

  .project-figure img,
  .project-figure video {
    width: 100%;
    height: auto;
    display: block;
    object-fit: cover;
  }

  /* Kicker: small numbered theme label */
  .project-kicker {
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: #4facfe;
    margin-bottom: 8px;
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

  /* Link Styling */
  .project-links-wrapper {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
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
  .project-description strong {
    color: #ffffff;
  }
  .project-description a {
    color: #4facfe;
    text-decoration: none;
  }
  .project-description a:hover {
    text-decoration: underline;
  }

  /* Outcome line: anchors each theme to concrete results */
  .project-outcome {
    font-size: 0.92rem;
    color: #d2e7ff;
    line-height: 1.6;
    margin: -8px 0 20px;
  }
  .project-outcome strong {
    color: #ffffff;
  }

  /* Tag Styling */
  .project-tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-top: auto;
  }

  .tag {
    font-size: 0.75rem;
    background: #222;
    color: #888;
    padding: 4px 10px;
    border-radius: 4px;
    border: 1px solid #444;
  }

  /* CTA row */
  .research-cta-row {
    display: flex;
    justify-content: center;
    gap: 14px;
    flex-wrap: wrap;
    margin-top: 1rem;
  }

  /* Mobile Responsive: Stack text over image */
  @media (max-width: 900px) {
    .project-card {
      grid-template-columns: 1fr;
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

  <p class="research-lede">
    My research connects two things usually done by different people: <strong>a decade of hands-on quantum-materials experiments</strong> and <strong>AI systems that assist the expert judgment those experiments require</strong>. Every claim below is grounded in instruments I have operated and analysis loops I have run by hand — before teaching an agent to help.
  </p>

  <div class="project-card">
    <div class="project-content">
      <div class="project-kicker">01 &middot; Current Focus</div>
      <div class="project-header">
        <span class="project-title">Agentic AI for Science</span>
        <div class="project-links-wrapper">
          <a class="project-link" href="https://drthyang.github.io/web-refinement/" target="_blank" rel="noopener noreferrer">MATERIA ▶</a>
          <a class="project-link" href="/software/">All Tools</a>
        </div>
      </div>
      <p class="project-description">
        The expert loop in scattering analysis — freeing parameters, judging residuals, grading a reduction, watching convergence — never got automated. I study how much of it LLM agents can help with when given real domain tools instead of chat: <a href="https://drthyang.github.io/web-refinement/" target="_blank" rel="noopener noreferrer">MATERIA</a> exposes a refinement engine to agents as MCP tools, <a href="https://drthyang.github.io/nebula3d/" target="_blank" rel="noopener noreferrer">NEBULA3D</a> has an LLM grade reduction quality, <a href="https://drthyang.github.io/rmc-toolkits/" target="_blank" rel="noopener noreferrer">RMCProfile Monitor</a> reasons over live runs, and matdiscover benchmarks agent-driven screening against non-LLM baselines. All of it is independent, personal open-source work.
      </p>
      <p class="project-outcome">
        <strong>Grounding principles:</strong> physics-based tools the agent must call, local-first models, evaluation against baselines — not demos.
      </p>
      <div class="project-tags">
        <span class="tag">LLM Agents</span>
        <span class="tag">MCP Tools</span>
        <span class="tag">Local-First Inference</span>
        <span class="tag">Evaluation & Baselines</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/materia-architecture.svg" alt="MATERIA architecture: web app UI, MCP agent server, and web workers sit on shared parsers and visualization, all calling a pure TypeScript scientific core of eight modules validated by 750 tests">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-kicker">02 &middot; Quantum Materials</div>
      <div class="project-header">
        <span class="project-title">Topology &times; Magnetism in Kagome Metals</span>
        <div class="project-links-wrapper">
          <a class="project-link" href="https://doi.org/10.1038/s41467-026-71683-7" target="_blank" rel="noopener noreferrer">Nat. Commun.</a>
          <a class="project-link" href="/publications/">Publications</a>
        </div>
      </div>
      <p class="project-description">
        Kagome magnets host Weyl nodes and anomalous transport that the lattice can in principle switch — if you find a material where the switch operates. My first-author <strong>Nature Communications (2026)</strong> study of Mn<sub>3</sub>Ga found exactly that: an intrinsic topological Weyl phase transition driven by a magnetostructural transformation near room temperature.
      </p>
      <p class="project-outcome">
        <strong>Why it matters:</strong> a room-temperature, lattice-coupled route to switching topological states — the mechanism antiferromagnetic spintronics needs.
      </p>
      <div class="project-tags">
        <span class="tag">Kagome Magnets</span>
        <span class="tag">Weyl Topology</span>
        <span class="tag">Magnetostructural Transition</span>
        <span class="tag">Neutron Diffraction</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/mn3ga-weyl-transition.png" alt="Mn3Ga summary figure: the magnetostructural transition between two kagome antiferromagnetic spin structures (top) drives a reorganization of Weyl nodes in the Brillouin zone — a topological Weyl phase transition (bottom)">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-kicker">03 &middot; Quantum Materials</div>
      <div class="project-header">
        <span class="project-title">Hidden Local Order Beyond the Average Structure</span>
        <div class="project-links-wrapper">
          <a class="project-link" href="https://doi.org/10.1021/jacs.4c09387" target="_blank" rel="noopener noreferrer">JACS</a>
          <a class="project-link" href="/publications/">Publications</a>
        </div>
      </div>
      <p class="project-description">
        Average structures hide the physics. Using PDF, diffuse scattering, and large-box RMC modeling, I resolve what conventional crystallography misses: local symmetry breaking emerging <em>with</em> antiferromagnetic order in kagome (Fe,Co)Sn (<strong>JACS 2024</strong>), quadrupolar ordering and spin-orbital dimers in GaNb<sub>4</sub>Se<sub>8</sub> (<strong>PRB 2024</strong>), and bond ordering in the cluster Mott insulator GaTa<sub>4</sub>Se<sub>8</sub> (<strong>PRR 2022</strong>).
      </p>
      <p class="project-outcome">
        <strong>The thread:</strong> disorder is not noise — quantifying it is what turns a structure into a mechanism.
      </p>
      <div class="project-tags">
        <span class="tag">PDF / 3D-&Delta;PDF</span>
        <span class="tag">Diffuse Scattering</span>
        <span class="tag">RMC Modeling</span>
        <span class="tag">Local Symmetry Breaking</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/ToC_JACS.png" alt="JACS study: local symmetry breaking coupled to antiferromagnetic order in kagome (Fe,Co)Sn">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-kicker">04 &middot; Method Development</div>
      <div class="project-header">
        <span class="project-title">From Static Ensembles to Lattice Dynamics</span>
        <div class="project-links-wrapper">
          <a class="project-link" href="https://drthyang.github.io/rmc-phonon-dynamics/" target="_blank" rel="noopener noreferrer">Phonon App ▶</a>
          <a class="project-link" href="https://github.com/drthyang/rmc-phonon-dynamics" target="_blank" rel="noopener noreferrer">GitHub</a>
        </div>
      </div>
      <p class="project-description">
        RMC ensembles encode experimentally constrained disorder — but only as static snapshots. I extract dynamics from them: phonon bands, DOS, and simulated INS computed directly from ensembles, ~100&times; faster with WebGPU, plus 3D-&Delta;PDF pipelines where every cleanup decision is inspectable. Everything ships as browser tools — your own data, nothing to install.
      </p>
      <p class="project-outcome">
        <strong>Outcome:</strong> measured total scattering to phonon spectra, no separate simulation backend — published as working, open-source software.
      </p>
      <div class="project-tags">
        <span class="tag">RMC Ensembles</span>
        <span class="tag">Phonons & INS</span>
        <span class="tag">3D-&Delta;PDF Pipelines</span>
        <span class="tag">WebGPU</span>
      </div>
    </div>
    <div class="project-figure">
      <video autoplay loop muted playsinline poster="/assets/images/phonon-concept.svg" aria-label="Animated phonon eigenvector mode extracted from an RMC ensemble, rendered in 3D">
        <source src="/assets/images/phonon-mode.webm" type="video/webm">
        <source src="/assets/images/phonon-mode.mp4" type="video/mp4">
      </video>
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-kicker">05 &middot; Foundation</div>
      <div class="project-header">
        <span class="project-title">Experimental Grounding: Sample &rarr; Signal</span>
        <div class="project-links-wrapper">
          <a class="project-link" href="/publications/">Publications</a>
          <a class="project-link" href="/about/">Background</a>
        </div>
      </div>
      <p class="project-description">
        I have owned every step of the pipeline. Synthesis: flux and vapor-transport crystals, inert-atmosphere chemistry, MBE thin films. Measurement: neutron and synchrotron experiments designed and run at ORNL's Spallation Neutron Source and other national facilities, plus STM/SP-STM down to single molecules — under cryogenic, high-pressure, and UHV conditions.
      </p>
      <p class="project-outcome">
        <strong>Why it matters for AI:</strong> knowing where data comes from — and how it breaks — separates physics-grounded models from black boxes.
      </p>
      <div class="project-tags">
        <span class="tag">Crystal Growth & MBE</span>
        <span class="tag">Measurement Design</span>
        <span class="tag">Neutron & Synchrotron</span>
        <span class="tag">STM / SP-STM</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/PRR_GTS.png" alt="Scattering data from synchrotron and neutron measurements of GaTa4Se8">
    </div>
  </div>

  <div class="research-cta-row">
    <a href="/software/" class="btn btn--primary">Explore the Software</a>
    <a href="/publications/" class="btn btn--primary">View Publications</a>
  </div>

</div>
