---
layout: page
permalink: /blog/
title: Blog
nav: true
nav_order: 1
_styles: |
  .blog-index {
    --blog-accent: #e799b0;
    margin-top: 1rem;
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
