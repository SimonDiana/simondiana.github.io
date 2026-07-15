---
layout: about
title: Home
permalink: /
subtitle:

profile: false
selected_papers: true
social: true

announcements:
  enabled: false

latest_posts:
  enabled: false

_styles: |
  .post-header {
    display: none;
  }

  .quantum-home {
    --qh-cyan: #63d8e6;
    --qh-violet: #9a8cff;
    --qh-amber: #ffca78;
    margin-top: 0.4rem;
  }

  .quantum-hero {
    position: relative;
    display: grid;
    grid-template-columns: minmax(0, 1.25fr) minmax(17rem, 0.75fr);
    gap: clamp(2rem, 6vw, 5.5rem);
    min-height: min(74vh, 46rem);
    align-items: center;
    overflow: hidden;
    padding: clamp(2rem, 6vw, 5.25rem);
    border: 1px solid rgba(148, 163, 184, 0.2);
    border-radius: 1.75rem;
    background:
      radial-gradient(circle at 82% 18%, rgba(154, 140, 255, 0.2), transparent 28%),
      radial-gradient(circle at 8% 86%, rgba(99, 216, 230, 0.14), transparent 31%),
      linear-gradient(145deg, #08131d 0%, #0d1d29 55%, #12172b 100%);
    box-shadow: 0 2rem 5rem rgba(2, 8, 23, 0.2);
    isolation: isolate;
  }

  .quantum-hero::after {
    content: "";
    position: absolute;
    inset: auto -8rem -12rem auto;
    z-index: -1;
    width: 28rem;
    height: 28rem;
    border: 1px solid rgba(99, 216, 230, 0.18);
    border-radius: 50%;
    box-shadow:
      0 0 0 3.5rem rgba(99, 216, 230, 0.035),
      0 0 0 7rem rgba(154, 140, 255, 0.025);
  }

  .quantum-eyebrow {
    display: flex;
    align-items: center;
    gap: 0.7rem;
    margin: 0 0 1.1rem;
    color: var(--qh-cyan);
    font-family: "SFMono-Regular", Consolas, monospace;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .quantum-eyebrow::before {
    content: "";
    width: 0.55rem;
    height: 0.55rem;
    border-radius: 50%;
    background: var(--qh-cyan);
    box-shadow: 0 0 0 0.35rem rgba(99, 216, 230, 0.12);
  }

  .quantum-title {
    max-width: 12ch;
    margin: 0;
    color: #f8fafc;
    font-size: clamp(3rem, 8vw, 6.6rem);
    font-weight: 780;
    line-height: 0.92;
    letter-spacing: -0.055em;
  }

  .quantum-title span {
    display: block;
    margin-top: 0.18em;
    background: linear-gradient(90deg, var(--qh-cyan), #c9c3ff 58%, var(--qh-amber));
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    font-size: 0.48em;
    line-height: 1.12;
    letter-spacing: -0.025em;
  }

  .quantum-intro {
    max-width: 39rem;
    margin: 1.5rem 0 0;
    color: rgba(226, 232, 240, 0.82);
    font-size: clamp(1rem, 1.5vw, 1.16rem);
    line-height: 1.75;
  }

  .quantum-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.7rem;
    margin-top: 1.8rem;
  }

  .quantum-actions a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.55rem;
    min-height: 2.85rem;
    padding: 0.72rem 1.05rem;
    border: 1px solid rgba(226, 232, 240, 0.2);
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.06);
    color: #f8fafc !important;
    font-size: 0.9rem;
    font-weight: 700;
    text-decoration: none !important;
    backdrop-filter: blur(12px);
    transition:
      transform 180ms ease,
      border-color 180ms ease,
      background 180ms ease;
  }

  .quantum-actions a:first-child {
    border-color: transparent;
    background: linear-gradient(110deg, #42b8c7, #7668d8);
    box-shadow: 0 0.9rem 2.3rem rgba(82, 157, 210, 0.24);
  }

  .quantum-actions a:hover {
    border-color: rgba(99, 216, 230, 0.7);
    background-color: rgba(99, 216, 230, 0.12);
    transform: translateY(-2px);
  }

  .state-field {
    position: relative;
    display: grid;
    min-height: 23rem;
    place-items: center;
  }

  .state-orbit,
  .state-orbit::before,
  .state-orbit::after {
    position: absolute;
    border: 1px solid rgba(148, 163, 184, 0.3);
    border-radius: 50%;
  }

  .state-orbit {
    width: min(21rem, 82%);
    aspect-ratio: 1;
    transform: rotate(-18deg) scaleY(0.44);
    box-shadow: 0 0 2.5rem rgba(99, 216, 230, 0.08);
  }

  .state-orbit::before,
  .state-orbit::after {
    content: "";
    inset: -1px;
  }

  .state-orbit::before {
    transform: rotate(60deg);
  }

  .state-orbit::after {
    transform: rotate(120deg);
  }

  .state-core {
    position: relative;
    z-index: 2;
    display: grid;
    width: 7.4rem;
    aspect-ratio: 1;
    place-items: center;
    border: 1px solid rgba(99, 216, 230, 0.38);
    border-radius: 50%;
    background: radial-gradient(circle at 35% 30%, #d8fbff, #58cbd9 24%, #6355bd 66%, #17152f);
    box-shadow:
      0 0 2.5rem rgba(99, 216, 230, 0.34),
      inset -1rem -1rem 1.8rem rgba(14, 23, 54, 0.45);
    color: #fff;
    font-family: Georgia, serif;
    font-size: 2.3rem;
    font-style: italic;
  }

  .state-node {
    position: absolute;
    z-index: 3;
    width: 0.85rem;
    height: 0.85rem;
    border: 2px solid #07121c;
    border-radius: 50%;
    background: var(--qh-amber);
    box-shadow: 0 0 1rem rgba(255, 202, 120, 0.8);
  }

  .state-node--a {
    top: 25%;
    right: 8%;
  }

  .state-node--b {
    bottom: 22%;
    left: 12%;
    background: var(--qh-cyan);
  }

  .state-caption {
    position: absolute;
    bottom: 0;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.45rem;
  }

  .state-caption span {
    padding: 0.34rem 0.62rem;
    border: 1px solid rgba(148, 163, 184, 0.22);
    border-radius: 999px;
    background: rgba(15, 23, 42, 0.5);
    color: rgba(226, 232, 240, 0.76);
    font-family: "SFMono-Regular", Consolas, monospace;
    font-size: 0.7rem;
  }

  .identity-strip {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    overflow: hidden;
    margin: 1rem 0 2.5rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 1.1rem;
    background: var(--global-divider-color);
  }

  .identity-item {
    padding: 1rem 1.2rem;
    background: var(--global-card-bg-color);
  }

  .identity-item strong {
    display: block;
    color: var(--global-text-color);
    font-size: 1rem;
  }

  .identity-item span {
    color: var(--global-text-color-light);
    font-size: 0.78rem;
  }

  .research-heading {
    max-width: 44rem;
    margin: 0 0 1.25rem;
  }

  .research-heading p {
    margin: 0 0 0.35rem;
    color: var(--global-theme-color);
    font-size: 0.76rem;
    font-weight: 800;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .research-heading h2 {
    margin: 0;
    color: var(--global-text-color);
    font-size: clamp(1.65rem, 3vw, 2.35rem);
    letter-spacing: -0.025em;
  }

  .research-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;
    margin-bottom: 2.6rem;
  }

  .research-card {
    position: relative;
    min-height: 15rem;
    overflow: hidden;
    padding: 1.4rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 1.2rem;
    background: var(--global-card-bg-color);
    transition:
      transform 180ms ease,
      border-color 180ms ease,
      box-shadow 180ms ease;
  }

  .research-card::after {
    content: attr(data-index);
    position: absolute;
    right: 0.9rem;
    bottom: -0.45rem;
    color: color-mix(in srgb, var(--global-theme-color) 11%, transparent);
    font-size: 5.5rem;
    font-weight: 800;
    line-height: 1;
  }

  .research-card:hover {
    border-color: color-mix(in srgb, var(--global-theme-color) 52%, var(--global-divider-color));
    box-shadow: 0 1rem 2.6rem rgba(15, 23, 42, 0.08);
    transform: translateY(-4px);
  }

  .research-icon {
    display: grid;
    width: 2.7rem;
    height: 2.7rem;
    place-items: center;
    border-radius: 0.85rem;
    background: color-mix(in srgb, var(--global-theme-color) 13%, var(--global-card-bg-color));
    color: var(--global-theme-color);
  }

  .research-card h3 {
    position: relative;
    z-index: 1;
    margin: 1.2rem 0 0.65rem;
    color: var(--global-text-color);
    font-size: 1.12rem;
  }

  .research-card p {
    position: relative;
    z-index: 1;
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    line-height: 1.65;
  }

  .current-work {
    display: grid;
    grid-template-columns: 0.7fr 1.3fr;
    gap: 1.5rem;
    align-items: center;
    margin-bottom: 2.8rem;
    padding: clamp(1.4rem, 3vw, 2rem);
    border: 1px solid var(--global-divider-color);
    border-radius: 1.35rem;
    background:
      linear-gradient(120deg, color-mix(in srgb, var(--global-theme-color) 10%, transparent), transparent 48%),
      var(--global-card-bg-color);
  }

  .current-work__label {
    color: var(--global-theme-color);
    font-family: "SFMono-Regular", Consolas, monospace;
    font-size: 0.76rem;
    font-weight: 800;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }

  .current-work h2 {
    margin: 0.45rem 0 0;
    color: var(--global-text-color);
    font-size: clamp(1.45rem, 2.7vw, 2rem);
  }

  .current-work__items {
    display: grid;
    gap: 0.7rem;
  }

  .current-work__items a {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1rem;
    padding: 0.85rem 1rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.9rem;
    background: var(--global-bg-color);
    color: var(--global-text-color);
    font-size: 0.87rem;
    font-weight: 650;
    line-height: 1.4;
    text-decoration: none;
  }

  .current-work__items a:hover {
    border-color: var(--global-theme-color);
    color: var(--global-theme-color);
    text-decoration: none;
  }

  @media (prefers-reduced-motion: no-preference) {
    .state-core {
      animation: quantum-pulse 4.5s ease-in-out infinite;
    }

    .state-orbit {
      animation: quantum-drift 12s linear infinite;
    }
  }

  @keyframes quantum-pulse {
    0%, 100% { transform: scale(0.96); }
    50% { transform: scale(1.04); }
  }

  @keyframes quantum-drift {
    from { rotate: 0deg; }
    to { rotate: 360deg; }
  }

  @media (max-width: 820px) {
    .quantum-hero {
      grid-template-columns: 1fr;
      min-height: auto;
    }

    .state-field {
      min-height: 18rem;
    }

    .research-grid,
    .current-work {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 560px) {
    .quantum-hero {
      padding: 1.45rem;
      border-radius: 1.2rem;
    }

    .quantum-title {
      font-size: clamp(2.8rem, 16vw, 4.3rem);
    }

    .quantum-actions {
      display: grid;
      grid-template-columns: 1fr 1fr;
    }

    .quantum-actions a {
      padding-inline: 0.7rem;
    }

    .identity-strip,
    .research-grid {
      grid-template-columns: 1fr;
    }

    .state-field {
      min-height: 15rem;
    }
  }
---

<div class="quantum-home">
  <section class="quantum-hero" aria-labelledby="quantum-home-title">
    <div>
      <p class="quantum-eyebrow">Theoretical Chemistry · Quantum Dynamics</p>
      <h1 class="quantum-title" id="quantum-home-title">
        Mo Sha
        <span>Mapping molecular motion beyond the adiabatic picture.</span>
      </h1>
      <p class="quantum-intro">
        I am a Chemistry Ph.D. student at Westlake University, developing local diabatic and tensor-network methods for accurate, tractable simulations of strongly coupled electron-nuclear dynamics.
      </p>
      <div class="quantum-actions" aria-label="Primary links">
        <a href="{{ '/publications/' | relative_url }}"><i class="fa-solid fa-book-open" aria-hidden="true"></i> Publications</a>
        <a href="{{ '/cv/' | relative_url }}"><i class="fa-solid fa-file-lines" aria-hidden="true"></i> CV</a>
        <a href="https://scholar.google.com/citations?user=dn2UfYoAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer"><i class="ai ai-google-scholar" aria-hidden="true"></i> Scholar</a>
        <a href="mailto:jsczfx1641501004@gmail.com"><i class="fa-solid fa-envelope" aria-hidden="true"></i> Contact</a>
      </div>
    </div>

    <div class="state-field" aria-hidden="true">
      <div class="state-orbit"></div>
      <div class="state-core">Ψ</div>
      <span class="state-node state-node--a"></span>
      <span class="state-node state-node--b"></span>
      <div class="state-caption">
        <span>local diabatic</span>
        <span>tensor network</span>
        <span>quantum geometry</span>
      </div>
    </div>
  </section>

  <section class="identity-strip" aria-label="Academic profile summary">
    <div class="identity-item">
      <strong>Westlake University</strong>
      <span>Ph.D. in Chemistry · 2024–2029</span>
    </div>
    <div class="identity-item">
      <strong>2 publications</strong>
      <span>PCCP · arXiv</span>
    </div>
    <div class="identity-item">
      <strong>Hangzhou, China</strong>
      <span>Advised by Prof. Bing Gu</span>
    </div>
  </section>

  <div class="research-heading">
    <p>Research coordinates</p>
    <h2>Three connected ways of making quantum molecular dynamics computable.</h2>
  </div>

  <section class="research-grid" aria-label="Research interests">
    <article class="research-card" data-index="01">
      <div class="research-icon"><i class="fa-solid fa-wave-square" aria-hidden="true"></i></div>
      <h3>Nonadiabatic Dynamics</h3>
      <p>Understanding molecular motion where electronic and nuclear degrees of freedom become inseparable.</p>
    </article>
    <article class="research-card" data-index="02">
      <div class="research-icon"><i class="fa-solid fa-diagram-project" aria-hidden="true"></i></div>
      <h3>Local Diabatic Structure</h3>
      <p>Building stable local representations with controlled convergence for nonadiabatic eigenvalue problems.</p>
    </article>
    <article class="research-card" data-index="03">
      <div class="research-icon"><i class="fa-solid fa-cubes" aria-hidden="true"></i></div>
      <h3>Tensor Networks</h3>
      <p>Compressing high-dimensional wavefunctions and propagators without discarding essential quantum correlations.</p>
    </article>
  </section>

  <section class="current-work" aria-labelledby="current-work-title">
    <div>
      <span class="current-work__label">Selected work · 2026</span>
      <h2 id="current-work-title">From rigorous convergence to high-dimensional dynamics.</h2>
    </div>
    <div class="current-work__items">
      <a href="https://doi.org/10.1039/D5CP03524D" target="_blank" rel="noopener noreferrer">
        <span>Exponential Convergence of the Local Diabatic Representation</span>
        <i class="fa-solid fa-arrow-up-right-from-square" aria-hidden="true"></i>
      </a>
      <a href="https://doi.org/10.48550/arXiv.2601.16913" target="_blank" rel="noopener noreferrer">
        <span>Coarse-Grained Geometric Quantum Dynamics in Tensor Networks</span>
        <i class="fa-solid fa-arrow-up-right-from-square" aria-hidden="true"></i>
      </a>
    </div>
  </section>
</div>
