---
layout: page
permalink: /blog/
title: Blog
nav: true
nav_order: 1
description: Research notes, publication journeys, and occasional reflections.
_styles: |
  .blog-index {
    --blog-accent: #e799b0;
    margin-top: 1rem;
  }

  .blog-index__intro {
    position: relative;
    overflow: hidden;
    margin-bottom: 1.6rem;
    padding: clamp(1.35rem, 4vw, 2.25rem);
    border: 1px solid color-mix(in srgb, var(--blog-accent) 36%, var(--global-divider-color));
    border-radius: 16px;
    background:
      radial-gradient(circle at 92% 12%, color-mix(in srgb, var(--blog-accent) 23%, transparent), transparent 15rem),
      linear-gradient(135deg, color-mix(in srgb, var(--blog-accent) 10%, var(--global-card-bg-color)), var(--global-card-bg-color));
  }

  .blog-index__intro::after {
    content: "";
    position: absolute;
    right: -2rem;
    bottom: -3rem;
    width: 10rem;
    height: 10rem;
    border: 1px solid color-mix(in srgb, var(--blog-accent) 32%, transparent);
    border-radius: 50%;
  }

  .blog-index__eyebrow {
    margin: 0 0 0.55rem;
    color: var(--global-theme-color);
    font-size: 0.78rem;
    font-weight: 800;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .blog-index__intro h2 {
    margin: 0;
    color: var(--global-text-color);
    font-size: clamp(1.55rem, 4vw, 2.15rem);
    font-weight: 780;
    letter-spacing: -0.025em;
  }

  .blog-index__intro p:last-child {
    max-width: 42rem;
    margin: 0.75rem 0 0;
    color: var(--global-text-color-light);
    line-height: 1.72;
  }

  .blog-index__list {
    display: grid;
    gap: 1rem;
  }

  .blog-index__card {
    display: grid;
    grid-template-columns: 6.6rem minmax(0, 1fr) auto;
    gap: 1.15rem;
    align-items: center;
    padding: 1.25rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 14px;
    background: var(--global-card-bg-color);
    color: var(--global-text-color) !important;
    text-decoration: none !important;
    box-shadow: 0 10px 28px rgba(78, 63, 63, 0.06);
    transition:
      transform 180ms ease,
      border-color 180ms ease,
      box-shadow 180ms ease;
  }

  .blog-index__card:hover {
    border-color: color-mix(in srgb, var(--blog-accent) 58%, var(--global-divider-color));
    box-shadow: 0 16px 38px rgba(78, 63, 63, 0.11);
    transform: translateY(-3px);
  }

  .blog-index__date {
    color: var(--global-theme-color);
    font-size: 0.82rem;
    font-weight: 780;
    letter-spacing: 0.025em;
  }

  .blog-index__card h3 {
    margin: 0;
    color: var(--global-text-color);
    font-size: 1.12rem;
    font-weight: 760;
    line-height: 1.45;
  }

  .blog-index__card p {
    margin: 0.42rem 0 0;
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    line-height: 1.55;
  }

  .blog-index__arrow {
    display: grid;
    width: 2.35rem;
    height: 2.35rem;
    place-items: center;
    border-radius: 50%;
    background: color-mix(in srgb, var(--blog-accent) 17%, var(--global-bg-color));
    color: var(--global-theme-color);
  }

  @media (max-width: 600px) {
    .blog-index__card {
      grid-template-columns: minmax(0, 1fr) auto;
    }

    .blog-index__date {
      grid-column: 1 / -1;
    }
  }
---

<div class="blog-index">
  <section class="blog-index__intro">
    <p class="blog-index__eyebrow">Research Notes</p>
    <h2>科研途中，留下一些可回看的坐标。</h2>
    <p>这里记录论文背后的过程、研究中的想法，以及偶尔值得保存的片段。</p>
  </section>

  <div class="blog-index__list">
    {% for post in site.posts %}
      <a class="blog-index__card" href="{{ post.url | relative_url }}">
        <time class="blog-index__date" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%Y.%m.%d' }}</time>
        <div>
          <h3>{{ post.title }}</h3>
          {% if post.description %}<p>{{ post.description }}</p>{% endif %}
        </div>
        <span class="blog-index__arrow" aria-hidden="true"><i class="fa-solid fa-arrow-right"></i></span>
      </a>
    {% else %}
      <p>文章正在准备中。</p>
    {% endfor %}
  </div>
</div>
