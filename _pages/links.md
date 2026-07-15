---
layout: page
permalink: /links/
title: Link
description: Academic profiles and contact channels.
nav: true
nav_order: 4

_styles: |
  .links-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(min(100%, 15rem), 1fr));
    gap: 1rem;
    margin-top: 1.5rem;
  }

  .link-card {
    display: grid;
    grid-template-columns: 2.8rem minmax(0, 1fr) auto;
    gap: 0.85rem;
    align-items: center;
    min-height: 5.5rem;
    padding: 1rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 12px;
    background:
      linear-gradient(135deg, var(--global-accent-soft-color), transparent 58%),
      var(--global-card-bg-color);
    color: var(--global-text-color) !important;
    text-decoration: none !important;
    box-shadow: 0 10px 28px rgba(140, 117, 110, 0.08);
    transition:
      transform 180ms ease,
      border-color 180ms ease,
      box-shadow 180ms ease;
  }

  .link-card:hover {
    border-color: color-mix(in srgb, var(--global-accent-color) 65%, var(--global-divider-color));
    box-shadow: 0 16px 36px rgba(140, 117, 110, 0.14);
    transform: translateY(-3px);
  }

  .link-card__icon {
    display: grid;
    width: 2.8rem;
    height: 2.8rem;
    place-items: center;
    border-radius: 10px;
    background: var(--global-accent-color);
    color: #fff;
    font-size: 1.25rem;
  }

  .link-card strong,
  .link-card small {
    display: block;
    overflow-wrap: anywhere;
  }

  .link-card strong {
    font-size: 1rem;
  }

  .link-card small {
    margin-top: 0.18rem;
    color: var(--global-text-color-light);
  }

  .link-card__arrow {
    color: var(--global-theme-color);
  }
---

<div class="links-grid">
  <a class="link-card" href="mailto:jsczfx1641501004@gmail.com">
    <span class="link-card__icon"><i class="fa-solid fa-envelope" aria-hidden="true"></i></span>
    <span><strong>Email</strong><small>jsczfx1641501004@gmail.com</small></span>
    <i class="fa-solid fa-arrow-up-right-from-square link-card__arrow" aria-hidden="true"></i>
  </a>

  <a class="link-card" href="https://scholar.google.com/citations?user=dn2UfYoAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">
    <span class="link-card__icon"><i class="ai ai-google-scholar" aria-hidden="true"></i></span>
    <span><strong>Google Scholar</strong><small>Publications and citations</small></span>
    <i class="fa-solid fa-arrow-up-right-from-square link-card__arrow" aria-hidden="true"></i>
  </a>

  <a class="link-card" href="https://orcid.org/0009-0003-1717-4517" target="_blank" rel="noopener noreferrer">
    <span class="link-card__icon"><i class="ai ai-orcid" aria-hidden="true"></i></span>
    <span><strong>ORCID</strong><small>0009-0003-1717-4517</small></span>
    <i class="fa-solid fa-arrow-up-right-from-square link-card__arrow" aria-hidden="true"></i>
  </a>

  <a class="link-card" href="https://github.com/SimonDiana" target="_blank" rel="noopener noreferrer">
    <span class="link-card__icon"><i class="fa-brands fa-github" aria-hidden="true"></i></span>
    <span><strong>GitHub</strong><small>SimonDiana</small></span>
    <i class="fa-solid fa-arrow-up-right-from-square link-card__arrow" aria-hidden="true"></i>
  </a>

  <a class="link-card" href="https://space.bilibili.com/10044859" target="_blank" rel="noopener noreferrer">
    <span class="link-card__icon"><i class="fa-solid fa-play" aria-hidden="true"></i></span>
    <span><strong>Bilibili</strong><small>Video channel</small></span>
    <i class="fa-solid fa-arrow-up-right-from-square link-card__arrow" aria-hidden="true"></i>
  </a>
</div>
