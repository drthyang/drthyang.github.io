---
layout: single
title: "AI Agents for Scattering Analysis"
permalink: /agents/
author_profile: true
classes: wide
excerpt: "One design for AI agents in five scattering tools: agents over tested scientific cores, numbers from code, guardrails in code, evals written from real failures, local or cloud models, and MCP hand-offs."
---

<style>
  .ag-lede {
    font-size: 1.08rem;
    line-height: 1.75;
    color: #b0b0b0;
    max-width: 62rem;
    margin: 0.5rem 0 2.2rem;
  }
  .ag-lede strong { color: #ffffff; }

  .ag-section-title {
    color: #ffffff;
    font-size: 1.35rem;
    font-weight: 700;
    margin: 2.6rem 0 0.3rem;
  }
  .ag-section-sub {
    color: #8fa8bd;
    font-size: 0.95rem;
    margin: 0 0 1.3rem;
  }

  /* Design-pattern cards */
  .ag-pattern-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
  }
  .ag-pattern {
    background: rgba(255, 255, 255, 0.02);
    border: 1px solid rgba(255, 255, 255, 0.07);
    border-left: 3px solid rgba(79, 172, 254, 0.55);
    border-radius: 6px;
    padding: 1rem 1.1rem;
  }
  .ag-pattern h4 {
    margin: 0 0 0.45rem;
    color: #ffffff;
    font-size: 0.98rem;
    font-weight: 700;
  }
  .ag-pattern p {
    margin: 0;
    color: #b0b0b0;
    font-size: 0.9rem;
    line-height: 1.6;
  }

  .ag-figure {
    margin: 1.6rem 0 0;
    max-width: 760px;
  }
  .ag-figure img {
    width: 100%;
    border: 1px solid #333;
    border-radius: 8px;
  }
  .ag-figure figcaption {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
    color: #8fa8bd;
    font-size: 0.85rem;
    line-height: 1.5;
    margin-top: 0.5rem;
  }

  /* Tool cards */
  .ag-tool-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.2rem;
  }
  .ag-tool {
    border: 1px solid #333;
    border-radius: 8px;
    padding: 1.2rem 1.4rem;
    display: flex;
    flex-direction: column;
    transition: transform 0.2s ease, border-color 0.2s ease;
  }
  .ag-tool:hover {
    transform: translateY(-2px);
    border-color: #4facfe;
  }
  .ag-tool:last-child { grid-column: 1 / -1; }
  .ag-tool-head {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    flex-wrap: wrap;
    gap: 8px;
    border-bottom: 1px solid #333;
    padding-bottom: 0.5rem;
    margin-bottom: 0.7rem;
  }
  .ag-tool-name {
    color: #ffffff;
    font-size: 1.1rem;
    font-weight: 700;
  }
  .ag-tool-name span {
    color: #888;
    font-weight: 400;
    font-size: 0.9rem;
  }
  .ag-tool-agent {
    color: #4facfe;
    font-size: 0.85rem;
    font-weight: 600;
  }
  .ag-tool p {
    color: #b0b0b0;
    font-size: 0.93rem;
    line-height: 1.6;
    margin: 0 0 0.8rem;
  }
  .ag-tool code,
  .ag-case code {
    font-size: 0.82rem;
    color: #d2e7ff;
    background: rgba(79, 172, 254, 0.08);
    padding: 0 3px;
    border-radius: 3px;
  }
  .page__content .ag-tool code::before,
  .page__content .ag-tool code::after,
  .page__content .ag-case code::before,
  .page__content .ag-case code::after { content: none; }
  .ag-tool-links {
    margin-top: auto;
    display: flex;
    gap: 14px;
  }
  .ag-tool-links a {
    color: #4facfe;
    font-size: 0.85rem;
    font-weight: 600;
    text-decoration: none;
  }
  .ag-tool-links a:hover { text-decoration: underline; }

  /* Case studies */
  .ag-case-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.2rem;
  }
  .ag-case {
    background: rgba(79, 172, 254, 0.04);
    border: 1px solid rgba(79, 172, 254, 0.25);
    border-radius: 8px;
    padding: 1.2rem 1.4rem;
  }
  .ag-case-kicker {
    font-size: 0.8rem;
    font-weight: 700;
    letter-spacing: 0.03em;
    color: #4facfe;
    margin-bottom: 0.3rem;
  }
  .ag-case h4 {
    margin: 0 0 0.4rem;
    color: #ffffff;
    font-size: 1rem;
    font-weight: 700;
  }
  .ag-case-stat {
    font-family: 'SF Mono', Menlo, monospace;
    color: #e2f1ff;
    font-size: 1.15rem;
    font-weight: 700;
    margin: 0 0 0.5rem;
  }
  .ag-case p {
    color: #b0b0b0;
    font-size: 0.92rem;
    line-height: 1.6;
    margin: 0;
  }

  /* Limits */
  .ag-limits {
    background: rgba(255, 255, 255, 0.02);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-left: 4px solid #4facfe;
    border-radius: 6px;
    padding: 1.1rem 1.4rem;
  }
  .ag-limits ul {
    margin: 0;
    padding-left: 1.1rem;
  }
  .ag-limits li {
    color: #b0b0b0;
    font-size: 0.95rem;
    line-height: 1.6;
    margin-bottom: 0.5rem;
  }
  .ag-limits li:last-child { margin-bottom: 0; }
  .ag-limits strong { color: #ffffff; }

  .ag-cta-row {
    display: flex;
    justify-content: center;
    gap: 14px;
    flex-wrap: wrap;
    margin-top: 2.5rem;
  }

  @media (max-width: 900px) {
    .ag-pattern-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  }
  @media (max-width: 768px) {
    .ag-pattern-grid,
    .ag-tool-grid,
    .ag-case-grid { grid-template-columns: 1fr; }
  }
</style>

<p class="ag-lede">
  Since mid-2026 I have been adding AI agents to the scattering software I build. Five tools share one design: <strong>the agent works on top of a tested scientific core, calls the same code the buttons call, and never supplies a number of its own.</strong>
</p>

<h2 class="ag-section-title">One pattern</h2>
<p class="ag-section-sub">The same six choices in every tool.</p>

<div class="ag-pattern-grid">
  <div class="ag-pattern">
    <h4>A tested core first</h4>
    <p>The science is deterministic, unit-tested code: 1,800+ tests in MATERIA, 570+ Python and 300+ web tests in NEBULA3D. The agent is a new way in, not a new engine.</p>
  </div>
  <div class="ag-pattern">
    <h4>Numbers come from code</h4>
    <p>The model chooses what to run and explains the result. Refined values and metrics come from tested code, never from the model.</p>
  </div>
  <div class="ag-pattern">
    <h4>Guardrails in code</h4>
    <p>Rules a prompt could forget are enforced in code: correlation limits, symmetry-allowed parameters only, a checked settings catalog, a hard-limit veto.</p>
  </div>
  <div class="ag-pattern">
    <h4>Evals from real failures</h4>
    <p>A failure on real data becomes a test, so the fix stays fixed: MATERIA&#39;s ten eval scenarios each replay one in CI.</p>
  </div>
  <div class="ag-pattern">
    <h4>Local or cloud models</h4>
    <p>The agents run on a local model (Ollama, LM Studio) or a cloud one, so unpublished data need not leave the machine.</p>
  </div>
  <div class="ag-pattern">
    <h4>MCP hand-offs</h4>
    <p>The cores are also MCP tool servers that hand work to each other: NEXPLAN writes inputs for MATERIA, NEBULA3D and the NeXus Viewer.</p>
  </div>
</div>

<figure class="ag-figure">
  <img src="/assets/images/materia-architecture.svg" alt="MATERIA architecture: the web app UI, the in-app Agent, the MCP server and web workers sit on shared parsers and visualization, all calling a pure TypeScript scientific core of thirteen modules with more than 1,800 tests">
  <figcaption>MATERIA: the page, the in-app Agent, the MCP server and the workers all call one tested core.</figcaption>
</figure>

<h2 class="ag-section-title">What each agent does</h2>
<p class="ag-section-sub">Five tools, from refinement to experiment planning.</p>

<div class="ag-tool-grid">
  <div class="ag-tool">
    <div class="ag-tool-head">
      <span class="ag-tool-name">MATERIA</span>
      <span class="ag-tool-agent">In-app Agent &middot; MCP server</span>
    </div>
    <p>An Agent beside a powder or PDF fit, on Claude or a local model, with 42 tools on the powder page, its magnetic step and the PDF page. <em>Ask first</em> puts each change on an approval card; <em>Auto</em> works through the method&#39;s stages and stops when a decision is yours. Every change is an undoable History step, and the engine sets the values. It reads five agent skills on demand and follows method rules written in code: no refining parameters correlated at |ρ| ≥ 0.95, no bare occupancy, a stage checklist. A 40-tool MCP server opens the same core to other agents.</p>
    <div class="ag-tool-links">
      <a href="https://drthyang.github.io/web-refinement/" target="_blank" rel="noopener noreferrer">Launch ▶</a>
      <a href="https://github.com/drthyang/web-refinement" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>
  </div>

  <div class="ag-tool">
    <div class="ag-tool-head">
      <span class="ag-tool-name">NEBULA3D</span>
      <span class="ag-tool-agent">NEBULA Pilot</span>
    </div>
    <p>An agent beside every page of the 3D-ΔPDF console, on a local or cloud model, with 22 tools backed by unit-tested metrics. It grades each reduction stage (<code>assess_stage</code>), checks the ΔPDF against the cell&#39;s symmetry (<code>symmetry_check</code>), tells a second grain from displaced Bragg peaks, and checks the UB. <code>tune_pipeline</code> tunes stage by stage from a checked catalog; a trial past a hard limit cannot win. Its measured analysis report exports as HTML/PDF or Markdown.</p>
    <div class="ag-tool-links">
      <a href="https://drthyang.github.io/nebula3d/" target="_blank" rel="noopener noreferrer">Launch ▶</a>
      <a href="https://github.com/drthyang/nebula3d" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>
  </div>

  <div class="ag-tool">
    <div class="ag-tool-head">
      <span class="ag-tool-name">RMCProfile Workbench <span>(beta)</span></span>
      <span class="ag-tool-agent">AI Copilot</span>
    </div>
    <p>A chatbox on every page, on a local or cloud model, that answers questions about a reverse Monte Carlo run by calling seven of the Workbench&#39;s own analyses (displacement directions, bond angles, the symmetry finder, convergence) through OpenAI-compatible tool calling. Deterministic checks read each result; the answer ends with an Outcome verdict. Built and tested with scripted model replies; real-model testing has just begun.</p>
    <div class="ag-tool-links">
      <a href="https://drthyang.github.io/rmc-toolkits/" target="_blank" rel="noopener noreferrer">Launch ▶</a>
      <a href="https://github.com/drthyang/rmc-toolkits" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>
  </div>

  <div class="ag-tool">
    <div class="ag-tool-head">
      <span class="ag-tool-name">NEXPLAN <span>(work in progress)</span></span>
      <span class="ag-tool-agent">26 MCP tools</span>
    </div>
    <p>My personal SNS experiment planner serves its calculations to agents over stdio: instrument coverage and limits, goniometer settings, powder patterns, MDNorm binning. Hand-off tools write the next tool&#39;s inputs in its own format: an instrument file for MATERIA; symmetry operations and Bragg positions for NEBULA3D and the NeXus Viewer.</p>
    <div class="ag-tool-links">
      <a href="https://drthyang.github.io/nexplan/" target="_blank" rel="noopener noreferrer">Launch ▶</a>
      <a href="https://github.com/drthyang/nexplan" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>
  </div>

  <div class="ag-tool">
    <div class="ag-tool-head">
      <span class="ag-tool-name">Athanor <span>(exploratory)</span></span>
      <span class="ag-tool-agent">Closed-loop screening agent</span>
    </div>
    <p>An agent that proposes candidate compositions, screens them with physics-grounded surrogates (CHGNet relaxation, convex-hull stability, MEGNet band gaps) and iterates, on local models by default. Campaigns are compared with non-LLM baselines under the same relaxation cap, not matched total compute; results are surrogate-level.</p>
    <div class="ag-tool-links">
      <a href="https://github.com/drthyang/agentic-ai-materials" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>
  </div>
</div>

<h2 class="ag-section-title">Case studies</h2>
<p class="ag-section-sub">From validation rounds on real data; each round fixed what it exposed.</p>

<div class="ag-case-grid">
  <div class="ag-case">
    <div class="ag-case-kicker">MATERIA &middot; neutron powder (D1A)</div>
    <h4>PbSO₄: why is the fit poor?</h4>
    <p class="ag-case-stat">wR 12% → 3.7%</p>
    <p>On the GSAS-II tutorial data, the Agent&#39;s fit diagnosis read the residual cause by cause and found the missing peak asymmetry.</p>
  </div>

  <div class="ag-case">
    <div class="ag-case-kicker">MATERIA &middot; lab X-ray (Cu Kα)</div>
    <h4>Fluorapatite: is the cell right?</h4>
    <p class="ag-case-stat">1 part in 10⁵</p>
    <p>The round added what lab data need, starting with the Kα₂ doublet. The cell check&#39;s cell now agrees with GSAS-II&#39;s refined cell to 1 part in 10⁵.</p>
  </div>

  <div class="ag-case">
    <div class="ag-case-kicker">MATERIA &middot; neutron powder, 150 K</div>
    <h4>Cr₂WO₆: do the two cations differ?</h4>
    <p class="ag-case-stat">P = 0.90</p>
    <p>The Agent&#39;s Bayesian check (<code>sample_posterior</code>) gave B(W) &gt; B(Cr) a posterior probability of only 0.90: the data cannot separate the two cations&#39; B, so one tied B is the defensible model.</p>
  </div>

  <div class="ag-case">
    <div class="ag-case-kicker">NEBULA3D &middot; a measured 6/mmm volume</div>
    <h4>Does the ΔPDF keep the crystal&#39;s symmetry?</h4>
    <p class="ag-case-stat">12.6% RMS → agree to rounding</p>
    <p>A symmetry check built during expert-review rounds exposed a pipeline defect: six-fold partners differed by 12.6% RMS. Now they agree to rounding, a property of the pipeline, not an agent result. The rounds also showed 176 of 188 apparent leftover peaks on one plane were short-range-order maxima, now kept.</p>
  </div>
</div>

<h2 class="ag-section-title">Limits</h2>
<p class="ag-section-sub">What this work has not shown yet.</p>

<div class="ag-limits">
  <ul>
    <li><strong>No real-model eval results yet.</strong> MATERIA&#39;s ten eval scenarios replay in CI with a scripted model. That shows each check catches the failure it was written for, not how often a real model passes.</li>
    <!--
      REAL-MODEL EVAL RESULTS GO HERE (not published yet).
      When MATERIA's eval scenarios have been run against real models (npm run eval:agent),
      add a card or bullet with: model names and versions, local or cloud, pass rate per
      scenario, number of runs, and the date. Do the same for NEBULA Pilot and the
      RMCProfile Workbench AI Copilot if they get eval suites. Until then, state no pass rates.
    -->
    <li><strong>A handful of datasets.</strong> The validation rounds cover a few real datasets, not a benchmark.</li>
    <li><strong>Drafts and betas.</strong> Two of MATERIA&#39;s five skills are first drafts; the AI Copilot is a beta; NEXPLAN is a work in progress; Athanor is exploratory.</li>
    <li><strong>Solo and recent.</strong> Personal open-source work by one developer, built since mid-2026; not peer reviewed.</li>
    <li><strong>A person decides.</strong> Guardrails limit what an agent can change, not whether its explanation is right. Check anything you publish against established tools.</li>
  </ul>
</div>

<div class="ag-cta-row">
  <a href="/software/" class="btn btn--primary">Packages &amp; Tools</a>
  <a href="/research/" class="btn btn--inverse">Research</a>
</div>
