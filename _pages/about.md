---
layout: about
title: Home
permalink: /
subtitle:

profile: false
selected_papers: false
social: false

announcements:
  enabled: false

latest_posts:
  enabled: false

_styles: |
  .post-header {
    display: none;
  }

  .home-page {
    --home-accent: #e799b0;
    --home-accent-strong: #df7898;
    --home-accent-soft: rgba(231, 153, 176, 0.13);
    margin-top: 0.25rem;
  }

  .home-hero {
    position: relative;
    min-height: min(72vh, 44rem);
    display: flex;
    align-items: center;
    margin-bottom: 2.25rem;
    padding: clamp(2rem, 7vw, 5rem);
    overflow: hidden;
    border: 1px solid rgba(91, 78, 86, 0.18);
    border-radius: 0.9rem;
    background: #f8f4f6;
    box-shadow: 0 1.6rem 4.5rem rgba(46, 37, 42, 0.13);
    isolation: isolate;
  }

  .home-hero__image {
    position: absolute;
    inset: 0;
    z-index: -3;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center 43%;
    transform: scaleX(-1);
  }

  .home-hero::before {
    content: "";
    position: absolute;
    inset: 0;
    z-index: -2;
    background: linear-gradient(
      90deg,
      rgba(25, 34, 38, 0.93) 0%,
      rgba(33, 39, 44, 0.82) 32%,
      rgba(46, 43, 48, 0.52) 54%,
      rgba(63, 49, 57, 0.08) 82%
    );
  }

  .home-hero::after {
    content: "";
    position: absolute;
    inset: 0;
    z-index: -1;
    opacity: 0.22;
    background-image:
      linear-gradient(rgba(255, 255, 255, 0.16) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255, 255, 255, 0.16) 1px, transparent 1px);
    background-size: 4rem 4rem;
    mask-image: linear-gradient(90deg, #000, transparent 72%);
  }

  .home-hero__content {
    width: min(100%, 43rem);
  }

  .home-kicker {
    display: flex;
    align-items: center;
    gap: 0.85rem;
    margin: 0 0 1.25rem;
    color: rgba(255, 255, 255, 0.92);
    font-size: 0.8rem;
    font-weight: 800;
    letter-spacing: 0.13em;
    text-transform: uppercase;
  }

  .home-kicker::before {
    content: "";
    width: 2.8rem;
    height: 1px;
    background: rgba(255, 255, 255, 0.66);
  }

  .home-title {
    margin: 0;
    color: #fff;
    font-size: clamp(4rem, 9vw, 7rem);
    font-weight: 300;
    line-height: 0.96;
    letter-spacing: -0.045em;
  }

  .home-subtitle {
    max-width: 39rem;
    margin: 1.5rem 0 0;
    color: rgba(255, 255, 255, 0.9);
    font-size: clamp(1rem, 1.8vw, 1.22rem);
    line-height: 1.75;
  }

  .home-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    margin-top: 1.8rem;
  }

  .home-actions a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.6rem;
    min-height: 3rem;
    padding: 0.75rem 1.15rem;
    border: 1px solid rgba(255, 255, 255, 0.23);
    border-radius: 0.7rem;
    background: rgba(78, 75, 82, 0.55);
    color: #fff !important;
    font-size: 0.94rem;
    font-weight: 750;
    text-decoration: none !important;
    backdrop-filter: blur(12px);
    transition:
      transform 180ms ease,
      border-color 180ms ease,
      background 180ms ease,
      box-shadow 180ms ease;
  }

  .home-actions a:first-child {
    border-color: var(--home-accent);
    background: var(--home-accent);
    box-shadow: 0 0.85rem 2rem rgba(231, 153, 176, 0.28);
  }

  .home-actions a:hover {
    border-color: rgba(255, 255, 255, 0.54);
    background: rgba(231, 153, 176, 0.78);
    transform: translateY(-2px);
  }

  .home-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
    margin-top: 1.45rem;
  }

  .home-tags span {
    padding: 0.38rem 0.68rem;
    border: 1px solid rgba(255, 255, 255, 0.28);
    border-radius: 0.55rem;
    background: rgba(57, 60, 65, 0.34);
    color: rgba(255, 255, 255, 0.9);
    font-family: "SFMono-Regular", Consolas, monospace;
    font-size: 0.75rem;
    font-weight: 700;
    backdrop-filter: blur(8px);
  }

  .home-panel {
    border: 1px solid var(--global-divider-color);
    border-radius: 0.8rem;
    background:
      linear-gradient(135deg, var(--home-accent-soft), transparent 48%),
      var(--global-card-bg-color);
    box-shadow: 0 0.8rem 2.5rem rgba(40, 32, 36, 0.05);
  }

  .home-collaboration {
    display: grid;
    grid-template-columns: minmax(0, 1fr) auto;
    gap: 1.5rem;
    align-items: center;
    margin-bottom: 2.1rem;
    padding: clamp(1.3rem, 3vw, 1.8rem);
  }

  .home-section-title {
    display: flex;
    align-items: center;
    gap: 0.7rem;
    margin: 0 0 0.8rem;
    color: var(--global-text-color);
    font-size: clamp(1.3rem, 2.2vw, 1.7rem);
    font-weight: 780;
  }

  .home-section-title::before {
    content: "";
    width: 0.65rem;
    height: 0.65rem;
    border-radius: 50%;
    background: var(--home-accent);
    box-shadow: 0 0 0 0.3rem var(--home-accent-soft);
  }

  .home-section-title::after {
    content: "";
    width: 3rem;
    height: 2px;
    background: linear-gradient(90deg, var(--home-accent), transparent);
  }

  .home-collaboration p {
    margin: 0;
    color: var(--global-text-color-light);
    line-height: 1.65;
  }

  .home-outline-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.55rem;
    min-height: 3rem;
    padding: 0.75rem 1.2rem;
    border: 1px solid color-mix(in srgb, var(--home-accent) 66%, var(--global-divider-color));
    border-radius: 0.65rem;
    background: color-mix(in srgb, var(--home-accent) 6%, var(--global-card-bg-color));
    color: var(--home-accent-strong) !important;
    font-weight: 760;
    text-decoration: none !important;
    white-space: nowrap;
    transition:
      transform 180ms ease,
      background 180ms ease;
  }

  .home-outline-button:hover {
    background: var(--home-accent-soft);
    transform: translateY(-2px);
  }

  .home-feed-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.25rem;
    margin-bottom: 2rem;
  }

  .home-feed-card {
    padding: clamp(1.25rem, 3vw, 1.75rem);
  }

  .home-list {
    display: grid;
    gap: 0.7rem;
    margin: 1.1rem 0 0;
    padding: 0;
    list-style: none;
  }

  .home-list li,
  .home-list a {
    color: var(--global-text-color);
    text-decoration: none;
  }

  .home-list li {
    display: grid;
    grid-template-columns: auto minmax(0, 1fr);
    gap: 0.8rem;
    align-items: center;
    min-height: 3.3rem;
    padding: 0.6rem 0.85rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.65rem;
    background: var(--global-bg-color);
    transition:
      border-color 180ms ease,
      transform 180ms ease;
  }

  .home-list li:hover {
    border-color: color-mix(in srgb, var(--home-accent) 64%, var(--global-divider-color));
    transform: translateY(-1px);
  }

  .home-list__number {
    display: grid;
    min-width: 2.1rem;
    height: 2.1rem;
    place-items: center;
    border: 1px solid color-mix(in srgb, var(--home-accent) 42%, var(--global-divider-color));
    border-radius: 50%;
    color: var(--home-accent-strong);
    font-size: 0.78rem;
    font-weight: 800;
  }

  .home-list__content {
    min-width: 0;
  }

  .home-list__content strong {
    display: block;
    color: var(--global-text-color);
    font-size: 0.92rem;
  }

  .home-list__content span {
    display: block;
    margin-top: 0.15rem;
    color: var(--home-accent-strong);
    font-size: 0.74rem;
    font-weight: 700;
  }

  .home-social-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.65rem;
    padding: 0.8rem 0 0.2rem;
  }

  .home-social-row a {
    display: inline-flex;
    align-items: center;
    gap: 0.45rem;
    padding: 0.55rem 0.75rem;
    border-radius: 0.55rem;
    color: var(--global-text-color-light);
    font-size: 0.82rem;
    font-weight: 700;
    text-decoration: none;
  }

  .home-social-row a:hover {
    background: var(--home-accent-soft);
    color: var(--home-accent-strong);
    text-decoration: none;
  }

  @media (max-width: 820px) {
    .home-hero {
      min-height: 36rem;
      padding: 2rem;
    }

    .home-hero::before {
      background: linear-gradient(90deg, rgba(25, 34, 38, 0.94), rgba(35, 39, 44, 0.72));
    }

    .home-collaboration,
    .home-feed-grid {
      grid-template-columns: 1fr;
    }

    .home-outline-button {
      width: fit-content;
    }
  }

  @media (max-width: 560px) {
    .home-hero {
      min-height: 34rem;
      padding: 1.35rem;
      border-radius: 0.75rem;
    }

    .home-hero__image {
      object-position: 42% center;
    }

    .home-hero::before {
      background: linear-gradient(180deg, rgba(25, 34, 38, 0.92), rgba(39, 41, 47, 0.58));
    }

    .home-title {
      font-size: clamp(3.7rem, 19vw, 5.2rem);
    }

    .home-actions {
      display: grid;
      grid-template-columns: 1fr 1fr;
    }

    .home-tags {
      gap: 0.4rem;
    }

    .home-tags span {
      font-size: 0.66rem;
    }
  }
---

<div class="home-page">
  <section class="home-hero" aria-labelledby="home-title">
    <img class="home-hero__image" src="{{ '/assets/img/home-hero.jpg' | relative_url }}" alt="" aria-hidden="true">
    <div class="home-hero__content">
      <p class="home-kicker">Theoretical Chemistry · Quantum Dynamics</p>
      <h1 class="home-title" id="home-title">Mo Sha</h1>
      <p class="home-subtitle">
        Ph.D. student in Chemistry at Westlake University, developing theoretical and computational methods for strongly coupled electron-nuclear dynamics.
      </p>
      <div class="home-actions" aria-label="Primary navigation">
        <a href="#research"><i class="fa-solid fa-wave-square" aria-hidden="true"></i> Research</a>
        <a href="{{ '/publications/' | relative_url }}"><i class="fa-solid fa-book-open" aria-hidden="true"></i> Publications</a>
        <a href="{{ '/cv/' | relative_url }}"><i class="fa-solid fa-file-lines" aria-hidden="true"></i> CV</a>
      </div>
      <div class="home-tags" aria-label="Research keywords">
        <span>nonadiabatic.qm</span>
        <span>local_diabatic.md</span>
        <span>tensor_networks.yml</span>
      </div>
    </div>
  </section>

  <section class="home-panel home-collaboration">
    <div>
      <h2 class="home-section-title">Open to Collaboration</h2>
      <p>Interested in nonadiabatic dynamics, quantum geometry, or tensor-network methods? I would be glad to discuss related ideas and possible collaborations.</p>
    </div>
    <a class="home-outline-button" href="mailto:jsczfx1641501004@gmail.com"><i class="fa-solid fa-envelope" aria-hidden="true"></i> Contact Me</a>
  </section>

  <div class="home-feed-grid" id="research">
    <section class="home-panel home-feed-card">
      <h2 class="home-section-title">Research Focus</h2>
      <ul class="home-list">
        <li>
          <span class="home-list__number">01</span>
          <span class="home-list__content"><strong>Nonadiabatic Quantum Dynamics</strong><span>electron–nuclear coupling</span></span>
        </li>
        <li>
          <span class="home-list__number">02</span>
          <span class="home-list__content"><strong>Local Diabatic Representations</strong><span>stable and convergent structure</span></span>
        </li>
        <li>
          <span class="home-list__number">03</span>
          <span class="home-list__content"><strong>Tensor-Network Methods</strong><span>high-dimensional quantum dynamics</span></span>
        </li>
      </ul>
    </section>

    <section class="home-panel home-feed-card">
      <h2 class="home-section-title">Selected Work</h2>
      <ul class="home-list">
        <li>
          <span class="home-list__number">#2</span>
          <a class="home-list__content" href="https://doi.org/10.1039/D5CP03524D" target="_blank" rel="noopener noreferrer"><strong>Exponential Convergence of the Local Diabatic Representation</strong><span>PCCP · 2026</span></a>
        </li>
        <li>
          <span class="home-list__number">#1</span>
          <a class="home-list__content" href="https://doi.org/10.48550/arXiv.2601.16913" target="_blank" rel="noopener noreferrer"><strong>Coarse-Grained Geometric Quantum Dynamics</strong><span>arXiv · 2026</span></a>
        </li>
      </ul>
    </section>
  </div>

  <nav class="home-social-row" aria-label="Academic profiles">
    <a href="https://scholar.google.com/citations?user=dn2UfYoAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer"><i class="ai ai-google-scholar" aria-hidden="true"></i> Scholar</a>
    <a href="https://orcid.org/0009-0003-1717-4517" target="_blank" rel="noopener noreferrer"><i class="ai ai-orcid" aria-hidden="true"></i> ORCID</a>
    <a href="https://github.com/SimonDiana" target="_blank" rel="noopener noreferrer"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
    <a href="https://space.bilibili.com/10044859" target="_blank" rel="noopener noreferrer"><i class="fa-solid fa-play" aria-hidden="true"></i> Bilibili</a>
  </nav>
</div>
