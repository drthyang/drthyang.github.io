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

  /* Intro strip */
  .research-intro {
    margin-bottom: 3rem;
    padding-bottom: 2rem;
    border-bottom: 1px solid #333;
  }

  .research-intro p {
    font-size: 1.1rem;
    color: #b0b0b0;
    line-height: 1.7;
    max-width: 900px;
    margin: 0 0 1.5rem 0;
  }

  .research-intro p strong {
    color: #e0e0e0;
  }

  .stat-row {
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
  }

  .stat {
    font-size: 0.85rem;
    color: #4facfe;
    background: rgba(79, 172, 254, 0.08);
    border: 1px solid rgba(79, 172, 254, 0.4);
    padding: 8px 16px;
    border-radius: 6px;
    font-weight: 600;
    letter-spacing: 0.02em;
  }

  /* Section headings */
  .section-heading {
    font-size: 1.6rem;
    font-weight: 700;
    color: #ffffff;
    margin: 0 0 0.5rem 0;
    padding-left: 14px;
    border-left: 4px solid #4facfe;
    line-height: 1.2;
  }

  .section-subtitle {
    font-size: 1rem;
    color: #888;
    margin: 0 0 2.5rem 14px;
    padding-left: 4px;
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

  .project-description em {
    color: #d0d0d0;
    font-style: normal;
    font-weight: 600;
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

  <div class="research-intro">
    <p>
      I work across the full chain of quantum-materials research — from <strong>synthesis and custom instrumentation</strong> to <strong>neutron and synchrotron scattering</strong> to <strong>physics-based modeling and scientific software</strong>. My path spans 15+ years: MBE thin-film growth and spin-polarized STM in Taiwan, DFT and quantum-transport modeling at Academia Sinica, building a high-pressure crystallography capability during my Ph.D. at Brown, and now leading neutron-scattering investigations of topological and correlated materials at Oak Ridge National Laboratory.
    </p>
    <div class="stat-row">
      <span class="stat">First-author: Nat. Commun. &amp; JACS</span>
      <span class="stat">9 SNS/HFIR instruments</span>
      <span class="stat">10+ beamtime proposals as PI/lead</span>
    </div>
  </div>

  <h2 class="section-heading">Research Themes</h2>
  <p class="section-subtitle">Current and recent scientific programs</p>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Kagome Magnets &amp; Topological Materials</span>
        <div class="project-links-wrapper">
          <a href="/publications/" class="project-link">Publications</a>
        </div>
      </div>
      <p class="project-description">
        How does local structure control topology? I discovered an intrinsic Weyl phase transition driven by a magnetostructural transformation in a kagome magnet (<em>Nat. Commun. 2026</em>) and showed that antiferromagnetism and local symmetry breaking emerge simultaneously in (Fe,Co)Sn (<em>JACS 2024</em>). Ongoing work connects local symmetry breaking to the anomalous Hall effect in Mn<sub>3</sub>Sn. This research was featured in a DOE research highlight for the ORNL Neutron Science Division.
      </p>
      <div class="project-tags">
        <span class="tag">Weyl Semimetals</span>
        <span class="tag">Kagome Lattice</span>
        <span class="tag">Neutron Diffraction</span>
        <span class="tag">Symmetry Analysis</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/prl-mn3sn-concept.svg" alt="Kagome magnetic correlations and anomalous Hall transport concept">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Lacunar Spinels &amp; Spin-Orbital Physics</span>
        <div class="project-links-wrapper">
          <a href="/publications/" class="project-link">Publications</a>
        </div>
      </div>
      <p class="project-description">
        My Ph.D. work established how molecular spin-orbital degrees of freedom shape the GaM<sub>4</sub>X<sub>8</sub> cluster Mott insulators: Jahn-Teller-driven quadrupolar ordering and spin-orbital dimer formation in GaNb<sub>4</sub>Se<sub>8</sub> (<em>PRB 2024</em>) and bond ordering with molecular spin-orbital fluctuations in GaTa<sub>4</sub>Se<sub>8</sub> (<em>PRR 2022</em>). Using a high-pressure XRD capability I built in-house, I also tracked structural evolution across the pressure-induced superconducting transition in this family.
      </p>
      <div class="project-tags">
        <span class="tag">Spin-Orbital Coupling</span>
        <span class="tag">Jahn-Teller Physics</span>
        <span class="tag">Cluster Mott Insulators</span>
        <span class="tag">High Pressure</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/PRR_GTS.png" alt="Bond ordering and spin-orbital fluctuations in GaTa4Se8">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Disordered &amp; High-Entropy Magnetic Materials</span>
        <div class="project-links-wrapper">
          <a href="/publications/" class="project-link">Publications</a>
        </div>
      </div>
      <p class="project-description">
        Disorder is not noise — it is often where the physics lives. I design scattering strategies for high-entropy spinel ferrites, rare-earth compounds, and field/temperature-dependent magnetic structures, using total scattering/PDF, diffuse scattering, 3D-ΔPDF, and reverse Monte Carlo modeling to extract short-range correlations and hidden local order that conventional crystallography averages away.
      </p>
      <div class="project-tags">
        <span class="tag">High-Entropy Materials</span>
        <span class="tag">Local Disorder</span>
        <span class="tag">Diffuse Scattering</span>
        <span class="tag">Magnetic Structure</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/mpdf-correlations.svg" alt="Magnetic pair distribution function and spin correlations concept">
    </div>
  </div>

  <h2 class="section-heading">Capabilities &amp; Instrumentation</h2>
  <p class="section-subtitle">The experimental and computational toolkit behind the science</p>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Neutron &amp; Synchrotron Scattering</span>
      </div>
      <p class="project-description">
        Design and execution of scattering campaigns across 9 SNS and HFIR instruments — including POWGEN, NOMAD, CORELLI, ARCS, CNCS, SEQUOIA, TOPAZ, and DEMAND — plus synchrotron X-ray work at APS, NSLS-II, and CHESS. Techniques span powder and single-crystal diffraction, total scattering/PDF, diffuse scattering, and inelastic neutron scattering under low-temperature, magnetic-field, and specialized sample environments. Authored 10+ successful peer-reviewed beamtime proposals as PI or lead contributor.
      </p>
      <div class="project-tags">
        <span class="tag">Neutron Scattering</span>
        <span class="tag">Synchrotron XRD</span>
        <span class="tag">PDF / Diffuse</span>
        <span class="tag">Inelastic Scattering</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/ToC_JACS.png" alt="Neutron scattering study of a kagome magnet">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Instrumentation &amp; Prototyping</span>
      </div>
      <p class="project-description">
        Built and commissioned an in-house high-pressure (&gt;10 GPa), low-temperature X-ray diffraction capability by integrating diamond anvil cells, cryostats, alignment procedures, and custom sample environments. Designed and fabricated custom sample holders and fixtures — including metal 3D-printed components — and prepared EDM gaskets for extreme-environment measurements. Extensive hands-on integration of commercial instruments with custom-designed hardware for cryogenic, high-pressure, and beamline experiments.
      </p>
      <div class="project-tags">
        <span class="tag">Diamond Anvil Cells</span>
        <span class="tag">Cryogenics</span>
        <span class="tag">3D-Printed Fixtures</span>
        <span class="tag">Systems Integration</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/instrumentation-dac-concept.svg" alt="Diamond anvil cell and cryostat high-pressure XRD schematic">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Synthesis &amp; Thin-Film Growth</span>
      </div>
      <p class="project-description">
        Synthesis of scattering-grade single crystals and polycrystalline quantum materials — including lacunar spinels — using flux/CVT-style solid-state methods, multi-zone furnace workflows, and inert-atmosphere glovebox techniques. Earlier graduate research included epitaxial thin-film growth by MBE and sputter deposition under UHV with in-situ RHEED monitoring, and atomic-scale surface characterization by spin-polarized STM, AFM, LEED, and AES.
      </p>
      <div class="project-tags">
        <span class="tag">Crystal Growth</span>
        <span class="tag">MBE / UHV</span>
        <span class="tag">STM / SP-STM</span>
        <span class="tag">Glovebox Techniques</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/synthesis-growth-concept.svg" alt="Crystal growth and MBE thin-film synthesis schematic">
    </div>
  </div>

  <div class="project-card">
    <div class="project-content">
      <div class="project-header">
        <span class="project-title">Computational &amp; Physics-Based Modeling</span>
        <div class="project-links-wrapper">
          <a href="/software/" class="project-link">Related Tools</a>
        </div>
      </div>
      <p class="project-description">
        DFT with Quantum ESPRESSO and VASP, phonon calculations with Phonopy, reverse Monte Carlo modeling with RMCProfile, Rietveld and magnetic structure refinement, NEGF quantum transport, and symmetry analysis with ISODISTORT/FINDSYM/Bilbao tools — all connected through reproducible Python/HPC workflows that validate physical models against high-fidelity experimental observables. This experiment–simulation loop is packaged into open-source scientific software.
      </p>
      <div class="project-tags">
        <span class="tag">DFT / Phonopy</span>
        <span class="tag">RMC Modeling</span>
        <span class="tag">Python / HPC</span>
        <span class="tag">Symmetry Analysis</span>
      </div>
    </div>
    <div class="project-figure">
      <img src="/assets/images/phonon-concept.svg" alt="Phonon dynamics and density of states concept">
    </div>
  </div>

</div>
