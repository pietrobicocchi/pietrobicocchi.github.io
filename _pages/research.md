---
layout: page
permalink: /research/
title: research
nav: true
nav_order: 1
_styles: |
  /* Research page only. Colours come from the theme variables, so light and dark modes follow the site. */
  .post article {
    --rs-accent: var(--global-theme-color);
    --rs-rule: var(--global-divider-color);
    --rs-ink: var(--global-text-color);
    --rs-muted: var(--global-text-color-light);
    --rs-measure: 38rem;
    --rs-arrow: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 32 10'%3E%3Cpath d='M0 5h30.5M25.5 1l5 4-5 4' fill='none' stroke='%23000' stroke-width='1'/%3E%3C/svg%3E");
  }
  .post article > p,
  .post article > ul,
  .post article > h2,
  .post article > h3,
  .post article > hr { max-width: var(--rs-measure); }
  .post article p,
  .post article li { line-height: 1.7; }
  .post article strong { font-weight: 500; }

  .post article h2 { font-size: 1.6rem; margin: 3.5rem 0 1.25rem; }
  .post article h3 { font-size: 1.3rem; font-weight: 400; margin: 3rem 0 1rem; }
  .rs-num {
    color: var(--rs-accent);
    font-variant-numeric: tabular-nums;
    font-weight: 400;
    margin-right: 0.75rem;
  }

  .rs-lede {
    font-size: 1.25rem;
    line-height: 1.55 !important;
    border-left: 2px solid var(--rs-accent);
    padding-left: 1.25rem;
    margin: 0.75rem 0 2.5rem;
  }

  .rs-label {
    color: var(--rs-muted);
    font-size: 0.75rem;
    font-weight: 500;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    margin: 1.75rem 0 0.6rem;
  }
  .post article .rs-label + ul { list-style: none; padding-left: 0; }
  .rs-label + ul li { position: relative; padding-left: 1.25rem; margin-bottom: 0.7rem; }
  .rs-label + ul li::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0.85em;
    width: 0.5rem;
    border-top: 1px solid var(--rs-accent);
  }

  /* Figures */
  .rs-fig { margin: 3rem 0 3.5rem; }
  .rs-fig figcaption {
    max-width: var(--rs-measure);
    margin-top: 1.75rem;
    color: var(--rs-muted);
    font-size: 0.875rem;
    line-height: 1.6;
  }
  .rs-fig figcaption b { color: var(--rs-ink); font-weight: 500; }
  .rs-fig .rs-n {
    color: var(--rs-accent);
    font-size: 1.5rem;
    font-weight: 300;
    line-height: 1;
    font-variant-numeric: tabular-nums;
  }
  .rs-fig .rs-term {
    color: var(--rs-ink);
    font-size: 0.8rem;
    font-weight: 500;
    letter-spacing: 0.14em;
    text-transform: uppercase;
  }
  .rs-fig a.rs-term:hover { color: var(--rs-accent); text-decoration: none; }
  .rs-fig p { margin: 0; }

  /* Figure 1: three demands and a cross-cutting ambition */
  .rs-demands { list-style: none; margin: 0; padding: 0; }
  .rs-demands li {
    display: grid;
    grid-template-columns: 4rem 12rem 1fr;
    align-items: baseline;
    padding: 1.25rem 0;
    border-bottom: 1px solid var(--rs-rule);
  }
  .rs-demands li:first-child { border-top: 1px solid var(--rs-rule); }
  .rs-demands .rs-q { font-size: 1.15rem; }
  .rs-brace {
    position: relative;
    height: 0.75rem;
    margin-top: 1.5rem;
    border: 1px solid var(--rs-muted);
    border-top: 0;
  }
  .rs-brace::after {
    content: "";
    position: absolute;
    left: 50%;
    top: 100%;
    height: 0.75rem;
    border-left: 1px solid var(--rs-muted);
  }
  .rs-gen { margin-top: 1.5rem; text-align: center; }
  .rs-gen .rs-n { margin-right: 0.9rem; }
  .rs-gen .rs-q { margin-top: 0.4rem; font-size: 1.15rem; font-style: italic; }

  /* Figure 2: how counterfactual claims are tested */
  .rs-stages {
    list-style: none;
    margin: 0;
    padding: 0;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    column-gap: 3.5rem;
  }
  .rs-stages li { position: relative; padding-top: 1.1rem; border-top: 1px solid var(--rs-muted); }
  .rs-stages li.rs-unseen { border-top-style: dashed; }
  .rs-stages li:not(:last-child)::after {
    content: "";
    position: absolute;
    top: 1.35rem;
    right: -2.75rem;
    width: 2rem;
    height: 0.625rem;
    background-color: var(--rs-muted);
    -webkit-mask: var(--rs-arrow) no-repeat center / contain;
    mask: var(--rs-arrow) no-repeat center / contain;
  }
  .rs-stages .rs-term { display: block; margin: 0.9rem 0 0.6rem; }
  .rs-stages p { font-size: 0.95rem; line-height: 1.6; }
  .rs-stages p + p { margin-top: 0.5rem; color: var(--rs-muted); font-style: italic; }
  .rs-guides {
    display: flex;
    justify-content: space-between;
    gap: 2rem;
    margin-top: 2rem !important;
    color: var(--rs-muted);
    font-size: 0.75rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }
  .rs-guides span { display: inline-flex; align-items: center; gap: 0.6rem; }
  .rs-guides span::before,
  .rs-guides span::after {
    width: 2rem;
    height: 0.625rem;
    background-color: currentColor;
    -webkit-mask: var(--rs-arrow) no-repeat center / contain;
    mask: var(--rs-arrow) no-repeat center / contain;
  }
  .rs-guides .rs-to-start::before { content: ""; transform: scaleX(-1); }
  .rs-guides .rs-to-end::after { content: ""; }

  /* Closing terms */
  .post article > hr { margin: 3.5rem 0 1.25rem; border: 0; border-top: 1px solid var(--rs-rule); }
  .rs-keywords { color: var(--rs-muted); font-size: 0.85rem; letter-spacing: 0.02em; }

  @media (max-width: 640px) {
    .rs-demands li { grid-template-columns: 3rem 1fr; row-gap: 0.35rem; }
    .rs-demands .rs-q { grid-column: 2; }
    .rs-stages { grid-template-columns: 1fr; row-gap: 2.75rem; }
    .rs-stages li:not(:last-child)::after {
      top: calc(100% + 0.6rem);
      right: auto;
      left: 0.1rem;
      width: 1.5rem;
      transform: rotate(90deg);
      transform-origin: 0 50%;
    }
    .rs-guides { flex-direction: column; gap: 0.75rem; }
    .rs-guides .rs-to-start::before { transform: rotate(-90deg); }
    .rs-guides .rs-to-end::before { content: ""; transform: rotate(90deg); }
    .rs-guides .rs-to-end::after { content: none; }
  }
---

<p class="rs-lede">Learning simulated worlds of interacting agents—grounded in evidence, responsive to change, and capable of informing what-if questions.</p>

Many of the systems we most need to understand cannot be studied one component at a time. Markets emerge from the decisions of traders and firms; epidemics unfold as people respond to risk; cities change as residents, institutions and infrastructure interact. In each case, what happens depends not only on the behaviour of individual agents, but on how they respond to one another.

We cannot readily experiment on an economy, a city or a society. We can, however, build a model in which to experiment. The difficulty is to know when its conclusions deserve our trust.

My research develops methods for **learning simulated worlds from data**, populating them with **agents that adapt**, and using them to **reason about interventions and unfamiliar conditions**. The central question is simple: **what would make a simulated world a reliable instrument for understanding a real one?**

## From simulation to evidence

A useful simulated world must meet three demands.

It must be **grounded** in observations, rather than merely plausible in its construction. It must be **adaptive**, capturing how agents change their behaviour and how their interactions reshape the system. And it must support **credible counterfactuals**: not just reproducing what has happened, but helping us assess what might happen if the rules, incentives or participants changed.

These demands are connected. A model that fits historical data may do so for the wrong reasons. One that reproduces current behaviour may fail when agents learn or institutions change. Even a convincing simulation cannot, on its own, establish that a prediction about an unobserved intervention is correct. Each step requires its own methods and evidence.

A fourth ambition cuts across all three: **generality**. Can the principles and components of these worlds transfer between settings, rather than requiring every model to be built anew?

<figure class="rs-fig">
  <ol class="rs-demands">
    <li>
      <span class="rs-n">01</span>
      <a class="rs-term" href="#grounding">Grounding</a>
      <span class="rs-q">Does it reflect the observed world?</span>
    </li>
    <li>
      <span class="rs-n">02</span>
      <a class="rs-term" href="#adaptation">Adaptation</a>
      <span class="rs-q">Does it respond as the world changes?</span>
    </li>
    <li>
      <span class="rs-n">03</span>
      <a class="rs-term" href="#counterfactuals">Counterfactuals</a>
      <span class="rs-q">Can its answers survive intervention?</span>
    </li>
  </ol>
  <div class="rs-brace" aria-hidden="true"></div>
  <div class="rs-gen">
    <p><span class="rs-n">04</span><a class="rs-term" href="#generality">Generality</a></p>
    <p class="rs-q">What can be carried from one world to another?</p>
  </div>
  <figcaption><b>Figure 1.</b> Three demands on a simulated world, and the question of what can be reused across worlds.</figcaption>
</figure>

## Research directions

### <span class="rs-num">01</span>Grounding: learning worlds from data {#grounding}

Simulations are often specified by hand and calibrated against a few aggregate statistics. I study how generative models, probabilistic agent-based models and simulation-based inference can instead connect the behaviour of individual agents to the evidence available about the system as a whole.

<p class="rs-label">Questions</p>

- **From aggregates to agents.** How much can we learn about individual behaviour when the observations are chiefly at the population or market level?
- **From fit to knowledge.** If several different mechanisms explain the same data, which claims are identifiable—and how should the remaining uncertainty be represented?
- **From models to estimation.** How can complex, often likelihood-intractable simulations be fitted to data efficiently and at scale?

### <span class="rs-num">02</span>Adaptation: learning and emergence {#adaptation}

An agent does not act in a fixed environment when other agents are learning too. Households alter their expectations, firms change their strategies, and institutions respond. Their adjustments, in turn, change the conditions under which everyone acts.

I study adaptation at both levels: how individual agents learn, using ideas from reinforcement learning, multi-agent learning and language-model agents; and how their interactions give rise to collective patterns that no agent controls.

<p class="rs-label">Questions</p>

- **Learning together.** When many agents adapt at once, under what conditions do their interactions settle, cycle or become unstable?
- **Different timescales.** How can a model accommodate decisions that change in seconds alongside habits and institutions that evolve over years?
- **Behaviour and emergence.** Do artificial agents respond credibly to new incentives, and can their interactions reproduce observed coordination, cascades and regime changes?

### <span class="rs-num">03</span>Counterfactuals: testing what cannot be observed {#counterfactuals}

The most consequential questions concern changes that have not yet occurred: a new policy, an unfamiliar market rule, or the arrival of a different kind of agent. A simulation can produce an answer to any such question. Producing an answer is not the same as establishing its credibility.

I develop ways to evaluate what simulations say beyond the conditions on which they were built, combining controlled synthetic environments with evidence from real interventions and careful accounts of uncertainty.

<p class="rs-label">Questions</p>

- **Validation beyond fit.** What evidence supports a model's response to interventions, rather than only its ability to reproduce historical observations?
- **Tests from the real world.** How can policy changes, natural experiments and shifts between environments provide demanding out-of-sample tests?
- **Failure and uncertainty.** How can we discover where a model breaks down, distinguish robust conclusions from fragile ones, and communicate what remains unknown?

<figure class="rs-fig">
  <ol class="rs-stages">
    <li>
      <span class="rs-n">01</span>
      <span class="rs-term">Controlled worlds</span>
      <p>Known rules; interventions can be repeated.</p>
      <p>Test recovery and failure modes.</p>
    </li>
    <li>
      <span class="rs-n">02</span>
      <span class="rs-term">Observed changes</span>
      <p>Policies, shocks and natural experiments.</p>
      <p>Test against outcomes that did occur.</p>
    </li>
    <li class="rs-unseen">
      <span class="rs-n">03</span>
      <span class="rs-term">Unseen interventions</span>
      <p>New rules, environments and agents.</p>
      <p>Report predictions with uncertainty and limits.</p>
    </li>
  </ol>
  <p class="rs-guides"><span class="rs-to-start">More direct checks</span><span class="rs-to-end">Greater real-world relevance</span></p>
  <figcaption><b>Figure 2.</b> Credibility is built through successive tests, from controlled settings to real changes, before claims are made about interventions not yet seen.</figcaption>
</figure>

### <span class="rs-num">04</span>Generality: foundations that transfer {#generality}

The longer-term ambition is to move beyond simulations built separately for each problem. Economies, markets, cities and societies of AI agents differ in important ways, but they also share structures: agents, incentives, constraints, networks and learning.

<p class="rs-label">Questions</p>

- **Transfer.** What can a world learned in one setting carry to another, and how much new evidence is needed to adapt it?
- **Reuse.** Which representations of agents, environments and interaction can serve as common foundations across domains?
- **Scale.** How can these methods support large populations without sacrificing empirical grounding, meaningful adaptation or credible evaluation?

## The longer view

Simulation has long offered a way to study systems that cannot be brought into a laboratory. Machine learning creates the possibility of making those simulations more closely tied to evidence, more responsive to changing behaviour, and more useful for examining decisions before they are made.

The aim is not to build perfect replicas of the world. It is to build **models whose assumptions can be examined, whose limits can be tested, and whose answers can be trusted in proportion to the evidence behind them**. Such models could become a practical scientific instrument for studying systems shaped by many interacting agents.

---

<p class="rs-keywords">World models · Agent-based modelling · Generative modelling · Reinforcement learning · Multi-agent systems · Causal inference · Complex systems</p>
