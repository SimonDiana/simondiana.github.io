---
layout: about
title: Home
permalink: /
subtitle:
custom_home: true

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
    --home-accent: var(--global-accent-color);
    margin-top: 0.25rem;
  }

  .home-hero {
    position: relative;
    min-height: min(78vh, 46rem);
    display: flex;
    align-items: center;
    padding: clamp(2rem, 6vw, 4.75rem);
    overflow: hidden;
    border: 1px solid color-mix(in srgb, var(--home-accent) 34%, var(--global-divider-color));
    border-radius: 18px;
    background:
      linear-gradient(135deg, rgba(140, 117, 110, 0.24), rgba(231, 153, 176, 0.22)),
      var(--global-card-bg-color);
    box-shadow:
      0 30px 90px rgba(78, 63, 63, 0.2),
      0 0 0 1px rgba(255, 255, 255, 0.3) inset;
    isolation: isolate;
  }

  .home-hero__image {
    position: absolute;
    top: 50%;
    right: -1%;
    z-index: -3;
    width: auto;
    height: 116%;
    transform: translateY(-50%) scaleX(-1);
    transform-origin: center;
    transition: transform 900ms cubic-bezier(0.2, 0.75, 0.2, 1);
  }

  .home-hero:hover .home-hero__image {
    transform: translateY(-50%) scaleX(-1) scale(1.025);
  }

  .home-hero::before {
    content: "";
    position: absolute;
    inset: 0;
    z-index: -1;
    opacity: 0.72;
    background:
      linear-gradient(rgba(255, 255, 255, 0.075) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255, 255, 255, 0.075) 1px, transparent 1px);
    background-size: 44px 44px;
    mask-image: linear-gradient(90deg, black, transparent 76%);
  }

  .home-hero::after {
    content: "";
    position: absolute;
    inset: 0;
    z-index: -2;
    background:
      radial-gradient(circle at 20% 18%, rgba(231, 153, 176, 0.24), transparent 24rem),
      linear-gradient(90deg, rgba(55, 39, 45, 0.94), rgba(77, 54, 62, 0.7) 46%, rgba(140, 117, 110, 0.08) 80%);
  }

  .home-hero__content {
    width: min(58%, 38rem);
    min-width: 0;
    color: #fff;
  }

  .home-title {
    margin: 0;
    color: #fff;
    font-size: clamp(4rem, 9vw, 6.8rem);
    font-weight: 320;
    line-height: 0.94;
    letter-spacing: -0.035em;
    text-shadow: 0 8px 30px rgba(55, 39, 45, 0.22);
  }

  .home-subtitle {
    max-width: 36rem;
    margin: 1.45rem 0 0;
    color: rgba(255, 255, 255, 0.9);
    font-size: clamp(1rem, 1.8vw, 1.22rem);
    line-height: 1.72;
    overflow-wrap: break-word;
    text-wrap: pretty;
  }

  .home-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    margin-top: 1.8rem;
  }

  .home-actions a {
    display: inline-flex;
    min-height: 3rem;
    align-items: center;
    justify-content: center;
    gap: 0.55rem;
    padding: 0.76rem 1.15rem;
    border: 1px solid rgba(255, 255, 255, 0.3);
    border-radius: 10px;
    background: rgba(255, 255, 255, 0.13);
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
    border-color: color-mix(in srgb, var(--home-accent), white 28%);
    background: var(--home-accent);
    box-shadow: 0 16px 36px rgba(231, 153, 176, 0.3);
  }

  .home-actions a:hover {
    border-color: rgba(255, 255, 255, 0.62);
    background: color-mix(in srgb, var(--home-accent) 82%, transparent);
    box-shadow: 0 18px 42px rgba(55, 39, 45, 0.25);
    transform: translateY(-3px);
  }

  .home-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem 1rem;
    margin-top: 1.45rem;
    color: rgba(255, 255, 255, 0.78);
    font-size: 0.82rem;
    font-weight: 650;
  }

  .home-meta span {
    display: inline-flex;
    align-items: center;
    gap: 0.42rem;
  }

  .home-meta i {
    color: color-mix(in srgb, var(--home-accent), white 24%);
  }

  @media (max-width: 900px) {
    .home-hero {
      min-height: 40rem;
      align-items: flex-start;
    }

    .home-hero__content {
      width: min(100%, 36rem);
    }

    .home-hero__image {
      top: auto;
      right: -3%;
      bottom: -8%;
      height: 92%;
      transform: scaleX(-1);
    }

    .home-hero:hover .home-hero__image {
      transform: scaleX(-1) scale(1.02);
    }

    .home-hero::after {
      background: linear-gradient(180deg, rgba(55, 39, 45, 0.96), rgba(77, 54, 62, 0.72) 56%, rgba(140, 117, 110, 0.18));
    }
  }

  @media (max-width: 560px) {
    .home-hero {
      width: min(100%, calc(100vw - 1.5rem));
      min-height: 39rem;
      padding: 1.45rem;
      border-radius: 14px;
    }

    .home-title {
      font-size: clamp(3.8rem, 20vw, 5.5rem);
    }

    .home-subtitle {
      font-size: 0.98rem;
      line-height: 1.62;
    }

    .home-actions {
      display: grid;
      grid-template-columns: 1fr 1fr;
      width: 100%;
    }

    .home-meta {
      display: grid;
      gap: 0.45rem;
    }

    .home-hero__image {
      right: 50%;
      bottom: -6%;
      height: 69%;
      transform: translateX(50%) scaleX(-1);
    }

    .home-hero:hover .home-hero__image {
      transform: translateX(50%) scaleX(-1);
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .home-hero__image,
    .home-actions a {
      transition: none;
    }
  }
---

<div class="home-page">
  <section class="home-hero" aria-label="Mo Sha home">
    <img class="home-hero__image" src="{{ '/assets/img/home-hero.jpg' | relative_url }}" alt="" aria-hidden="true">
    <div class="home-hero__content">
      <h1 class="home-title">Mo Sha</h1>
      <p class="home-subtitle">
        Ph.D. student in Chemistry at Westlake University, developing theoretical and computational methods for strongly coupled electron-nuclear dynamics.
      </p>
      <div class="home-actions">
        <a href="{{ '/publications/' | relative_url }}"><i class="fa-solid fa-book-open" aria-hidden="true"></i> Publications</a>
        <a href="{{ '/cv/' | relative_url }}"><i class="fa-solid fa-file-lines" aria-hidden="true"></i> CV</a>
      </div>
      <div class="home-meta" aria-label="Academic affiliation">
        <span><i class="fa-solid fa-building-columns" aria-hidden="true"></i> Westlake University</span>
        <span><i class="fa-solid fa-location-dot" aria-hidden="true"></i> Hangzhou, China</span>
      </div>
    </div>
  </section>
</div>
