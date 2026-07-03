# Research Page Improvement Plan

Goal: make the research page evidence that I can carry a quantum materials problem end-to-end: grow or prepare materials, characterize them, design and execute scattering measurements, analyze/model the data, publish the physics, and prototype software when existing tools are not enough.

## Core Message

Position the page around full-stack experimental materials research:

> I work across the full materials research loop: material growth and preparation, synchrotron and neutron scattering, local-structure and magnetic analysis, advanced computational modeling, rapid research-tool prototyping, publication, and reusable software development.

The page should not make computation look secondary or weak. It should show computation as one of my major strengths, integrated with hands-on experimental materials science.

## Proposed Page Structure

### 1. Opening Narrative

Add a short intro before the project cards.

Suggested direction:

> My research focuses on quantum and functional materials where local structure, magnetism, lattice dynamics, and defects control emergent behavior. I combine material growth/preparation, synchrotron and neutron scattering, total scattering/PDF, RMC and magnetic-PDF modeling, and advanced Python/C++ workflows to connect atomic-scale disorder with transport, symmetry breaking, and dynamics.

### 2. Full-Stack Materials Research Strip

Add a compact visual/process strip:

`Grow / Prepare -> Measure -> Analyze -> Model -> Prototype -> Publish -> Build Tools`

Each step should have one short phrase:

- `Grow / Prepare`: crystal growth, solid-state synthesis, sample environments
- `Measure`: synchrotron, neutron scattering, PDF, diffuse scattering, INS
- `Analyze`: Rietveld, PDF, mPDF, symmetry, local structure
- `Model`: RMC, phonons, DFT/phonopy where appropriate
- `Prototype`: browser tools, Python/C++ workflows, WebGPU/Pyodide proof-of-concepts
- `Publish`: first-author papers, peer-reviewed results
- `Build Tools`: reusable apps and open-source scientific software

### 3. Research Cards With Ownership

Rewrite each project card with a consistent structure:

- `Question`: the scientific problem
- `Ownership`: what I personally drove
- `Methods`: experimental and computational toolkit
- `Outcome`: discovery, paper, tool, or reusable workflow

Tone should use confident language:

- `I led...`
- `I developed...`
- `I combined...`
- `I built...`
- `This resulted in...`

Avoid vague phrasing like `we investigate` unless emphasizing collaboration.

## Project Rewrite Targets

### Topological Kagome Magnets

Suggested title:

`Kagome Magnets: Magnetostructural Transitions, Local Disorder, and Topological Transport`

Points to show:

- Materials: Mn3Sn, Mn3Ga, (Fe,Co)Sn
- Experimental: material growth/preparation, neutron/synchrotron scattering, total scattering/PDF
- Computational: RMC, mPDF, symmetry analysis, Python workflows
- Outcome: anomalous Hall transport, Weyl phase transition, local symmetry breaking, antiferromagnetism

### Local Structure and Magnetic Correlations

Suggested title:

`Local Structure and Magnetic Correlations From Total Scattering`

Points to show:

- Question: what local correlations are invisible to average diffraction?
- Methods: neutron total scattering, PDF, magnetic PDF, RMC
- Ownership: experimental design/analysis/modeling pipeline
- Outcome: connect short-range correlations to emergent magnetic/topological behavior

### Phonon Dynamics From RMC Ensembles

Suggested title:

`Phonon Dynamics Reconstructed From Total Scattering`

Points to show:

- Question: can static total-scattering/RMC ensembles reveal dynamical information?
- Methods: RMCProfile, force constants, phonon DOS, INS simulation, Python/C++, WebGPU app
- Ownership: developed analysis workflow and software prototype/tooling
- Outcome: research-derived software and reusable computational workflow

### Cluster Mott and Spin-Orbital Physics

Suggested title:

`Local Symmetry Breaking in Cluster Mott Insulators`

Points to show:

- Materials: GaTa4Se8, GaNb4Se8 if appropriate
- Experimental: total scattering/PDF and local-structure analysis
- Computational: local distortion modeling, symmetry interpretation
- Outcome: Jahn-Teller physics, spin-orbital dimer formation, hidden local symmetry breaking

## Prototyping Section

Add prototyping as an explicit capability, not just a software afterthought.

Suggested framing:

> When a research bottleneck cannot be solved well with existing tools, I prototype the missing workflow: local-data browser apps, WebGPU/Pyodide proof-of-concepts, reusable Python/C++ pipelines, and visualization dashboards for scattering and RMC analysis.

Examples:

- `rmc-phonon-dynamics`: phonon analysis from RMC ensembles; main WebGPU speedup belongs here
- `rmc-toolkits`: RMCProfile/STOG monitoring, visualization, KDE slices, and model inspection
- `nebula3d`: 3D diffuse scattering cleanup and 3D-DeltaPDF workflow

## Methods Section

Add a compact `Methods I Use` or `Methods I Own` section.

Suggested groups:

- `Materials`: crystal growth, solid-state synthesis, sample preparation
- `Scattering`: neutron diffraction, synchrotron diffraction, total scattering, PDF, diffuse scattering, INS
- `Local/Magnetic Analysis`: RMC, mPDF, Rietveld/magnetic refinement, symmetry analysis
- `Computation`: Python, C++, HPC, sparse/numerical methods, DFT, phonopy, WebGPU/Pyodide prototyping
- `Output`: papers, analysis software, browser apps, reproducible workflows

## Recent Highlights

Research highlights should name systems and outcomes directly:

- First-author Nature Communications work linking magnetostructural transformation to Weyl physics in Mn3Sn
- JACS work revealing coupled antiferromagnetism and local symmetry breaking in kagome (Fe,Co)Sn
- Software prototypes turning RMC/scattering workflows into reusable browser-based or Python tools

## Figure Strategy

Replace placeholder/concept graphics over time with real evidence:

- paper TOC figures
- PDF/RMC fit panels
- neutron/synchrotron scattering maps
- local distortion motifs
- phonon DOS / INS simulation plots
- screenshots from browser tools

Real figures should be prioritized because this page is meant to prove experimental and computational ownership.

## Implementation Order

1. Add opening narrative and full-stack process strip.
2. Rewrite project cards using `Question / Ownership / Methods / Outcome`.
3. Add prototyping section.
4. Add methods section.
5. Replace placeholder graphics with real figures/screenshots.
6. Add direct DOI/code links to each project card.

No public changes should be committed, pushed, deployed, or hosted without explicit permission.
