---
layout: single
title: "AI Agents for Scattering Analysis"
permalink: /agents/
author_profile: true
classes: wide
excerpt: "One design for the AI agents in my scattering tools: agents on tested scientific cores, with numbers and guardrails in code."
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
  .ag-case:last-child:nth-child(odd) { grid-column: 1 / -1; }
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
  I have been adding AI agents to the scattering software I build. They share one design: <strong>the agent works on top of a tested scientific core and calls the same code the buttons call; refined values and metrics come from that code, not from the model.</strong>
</p>

<h2 class="ag-section-title">One pattern</h2>
<p class="ag-section-sub">Six choices that run through the tools.</p>

<div class="ag-pattern-grid">
  <div class="ag-pattern">
    <h4>A tested core first</h4>
    <p>The science is deterministic, unit-tested code (1,700+ tests in MATERIA alone). The agent is a new way in, not a new engine.</p>
  </div>
  <div class="ag-pattern">
    <h4>Numbers come from code</h4>
    <p>The model chooses what to run and explains the result. Refined values and metrics come from tested code, never from the model.</p>
  </div>
  <div class="ag-pattern">
    <h4>Guardrails in code</h4>
    <p>Rules a prompt could forget are enforced in code, from correlation limits to a hard-limit veto.</p>
  </div>
  <div class="ag-pattern">
    <h4>Evals from real failures</h4>
    <p>A failure on real data becomes a test, so the fix stays fixed: MATERIA&#39;s ten eval scenarios replay in CI.</p>
  </div>
  <div class="ag-pattern">
    <h4>Local or cloud models</h4>
    <p>The agents run on a local model (Ollama, LM Studio) or a cloud one, so unpublished data need not leave the machine.</p>
  </div>
  <div class="ag-pattern">
    <h4>MCP hand-offs</h4>
    <p>MATERIA and NEXPLAN are also MCP tool servers, and NEXPLAN writes inputs in the formats MATERIA, NEBULA3D and the NeXus Viewer read.</p>
  </div>
</div>

<figure class="ag-figure">
  <img src="/assets/images/materia-architecture.svg" alt="MATERIA architecture: the web app UI, the in-app Agent, the MCP server and web workers sit on shared parsers and visualization, all calling a pure TypeScript scientific core of thirteen modules with more than 1,700 tests">
  <figcaption>MATERIA: the page, the in-app Agent, the MCP server and the workers all call one tested core.</figcaption>
</figure>

<h2 class="ag-section-title">What each agent does</h2>
<p class="ag-section-sub">Four scattering tools and one materials-screening experiment.</p>

<div class="ag-tool-grid">
  <div class="ag-tool">
    <div class="ag-tool-head">
      <span class="ag-tool-name">MATERIA</span>
      <span class="ag-tool-agent">In-app Agent &middot; MCP server</span>
    </div>
    <p>An Agent beside a powder or PDF fit, on Claude or a local model, that works through the page&#39;s own controls. You approve each change or let it run in <em>Auto</em>; every change can be undone, and the engine, not the model, computes the refined values. An MCP server opens the same core to other agents.</p>
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
    <p>An agent beside every page of the 3D-ΔPDF console, on a local or cloud model. It grades each reduction stage from unit-tested metrics, checks the ΔPDF against the crystal&#39;s symmetry, and tunes the pipeline from a checked catalog; a trial past a hard limit cannot win.</p>
    <div class="ag-tool-links">
      <a href="https://drthyang.github.io/nebula3d/" target="_blank" rel="noopener noreferrer">Launch ▶</a>
      <a href="https://github.com/drthyang/nebula3d" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>
  </div>

  <div class="ag-tool">
    <div class="ag-tool-head">
      <span class="ag-tool-name">RMCProfile Workbench</span>
      <span class="ag-tool-agent">AI Copilot (beta)</span>
    </div>
    <p>A chatbox on every page, on a local or cloud model, that answers questions about a reverse Monte Carlo run by calling the Workbench&#39;s own analyses; deterministic checks read each result. The Workbench is live; the Copilot is not deployed yet.</p>
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
    <p>My personal SNS experiment planner serves its calculations to agents (on a development branch), with hand-off tools that write the next tool&#39;s inputs: an instrument file for MATERIA, symmetry operations and Bragg positions for NEBULA3D and the NeXus Viewer.</p>
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
    <p>An agent that proposes candidate compositions, screens them with physics-grounded surrogates and iterates, on local models by default. Compared with non-LLM baselines under the same relaxation cap, not matched total compute.</p>
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
    <p>On the GSAS-II tutorial data, the Agent&#39;s fit diagnosis found the missing peak asymmetry.</p>
  </div>

  <div class="ag-case">
    <div class="ag-case-kicker">MATERIA &middot; lab X-ray (Cu Kα)</div>
    <h4>Fluorapatite: is the cell right?</h4>
    <p class="ag-case-stat">1 part in 10⁵</p>
    <p>Once the cell check handled lab data (the Kα₂ doublet, a zero shift), its cell agreed with GSAS-II&#39;s refined cell to 1 part in 10⁵.</p>
  </div>

  <div class="ag-case">
    <div class="ag-case-kicker">MATERIA &middot; neutron powder, 150 K</div>
    <h4>Cr₂WO₆: do the two cations differ?</h4>
    <p class="ag-case-stat">P = 0.90</p>
    <p>The Agent&#39;s Bayesian check gave B(W) &gt; B(Cr) a probability of only 0.90, so one tied B is the defensible model.</p>
  </div>

  <div class="ag-case">
    <div class="ag-case-kicker">NEBULA3D &middot; a measured 6/mmm volume</div>
    <h4>Does the ΔPDF keep the crystal&#39;s symmetry?</h4>
    <p class="ag-case-stat">12.6% RMS → agree to rounding</p>
    <p>A symmetry check exposed a pipeline defect: six-fold partners differed by 12.6% RMS. Now they agree to rounding, a fix to the pipeline, not an agent result.</p>
  </div>

  <div class="ag-case">
    <div class="ag-case-kicker">RMCProfile Workbench &middot; two local models</div>
    <h4>Does the AI Copilot hold up on a real model?</h4>
    <p class="ag-case-stat">5 of 6 and 4 of 6 fully right</p>
    <p>Six questions on the demo run: every tool call was valid, and the runs exposed four bugs, now fixed. Both models rated every answer &ldquo;achieved&rdquo;, so trust the checks, not the verdict.</p>
  </div>
</div>

<h2 class="ag-section-title">Limits</h2>
<p class="ag-section-sub">What this work has not shown yet.</p>

<div class="ag-limits">
  <ul>
    <li><strong>No real-model eval pass rates yet.</strong> MATERIA&#39;s eval scenarios replay in CI with a scripted model; the AI Copilot&#39;s real-model test is a six-question spot check.</li>
    <!--
      REAL-MODEL EVAL RESULTS GO HERE (not published yet).
      When MATERIA's or NEBULA Pilot's eval scenarios have been run against real models
      (npm run eval:agent in each repo; NEBULA3D's runs from web/), add a card or bullet with:
      model names and versions, local or cloud, pass rate per scenario, number of runs, and
      the date. The AI Copilot's 2026-10-10 spot check (rmc-toolkits, src/llm/README.md) is
      already a case study above. Until then, state no pass rates.
    -->
    <li><strong>A handful of datasets.</strong> The validation rounds cover a few real datasets, not a benchmark.</li>
    <li><strong>Not all released.</strong> MATERIA&#39;s newest Agent work (its three case studies) and NEXPLAN&#39;s MCP tools are on development branches, not yet in the live apps. Athanor is exploratory.</li>
    <li><strong>Solo work.</strong> Personal open-source work by one developer; not peer reviewed.</li>
    <li><strong>A person decides.</strong> Guardrails limit what an agent can change, not whether its explanation is right. Check anything you publish against established tools.</li>
  </ul>
</div>

<div class="ag-cta-row">
  <a href="/software/" class="btn btn--primary">Packages &amp; Tools</a>
  <a href="/research/" class="btn btn--inverse">Research</a>
</div>
