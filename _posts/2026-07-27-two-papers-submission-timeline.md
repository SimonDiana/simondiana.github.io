---
layout: post
title: "两篇论文的投稿时间线：修改、转投与再次出发"
date: 2026-07-27
categories: research-notes
tags:
  - publishing
  - research
description: "记录两项工作的投稿、修改与转投历程，以及同行评审之外那些漫长但重要的等待。"
related_posts: false
giscus_comments: false
_styles: |
  .publication-journey {
    --journey-accent: #e799b0;
  }

  .journey-note {
    margin: 1.2rem 0 2rem;
    padding: 1rem 1.15rem;
    border: 1px solid color-mix(in srgb, var(--journey-accent) 34%, var(--global-divider-color));
    border-left: 4px solid var(--journey-accent);
    border-radius: 10px;
    background: color-mix(in srgb, var(--journey-accent) 7%, var(--global-card-bg-color));
    color: var(--global-text-color-light);
    font-size: 0.92rem;
    line-height: 1.7;
  }

  .paper-card {
    margin: 2rem 0 1.35rem;
    padding: 1.25rem 1.35rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 14px;
    background:
      linear-gradient(135deg, color-mix(in srgb, var(--journey-accent) 9%, transparent), transparent 58%),
      var(--global-card-bg-color);
    box-shadow: 0 10px 28px rgba(78, 63, 63, 0.06);
  }

  .paper-card__topline {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 0.55rem;
  }

  .paper-card__index,
  .paper-card__status {
    display: inline-flex;
    align-items: center;
    min-height: 1.85rem;
    padding: 0.28rem 0.62rem;
    border-radius: 999px;
    font-size: 0.74rem;
    font-weight: 800;
    letter-spacing: 0.045em;
  }

  .paper-card__index {
    background: var(--global-accent-soft-color);
    color: var(--global-theme-color);
  }

  .paper-card__status {
    border: 1px solid color-mix(in srgb, var(--journey-accent) 48%, var(--global-divider-color));
    color: var(--global-text-color-light);
  }

  .paper-card h2 {
    margin: 0;
    font-size: clamp(1.25rem, 3vw, 1.6rem);
    font-weight: 780;
    line-height: 1.42;
    letter-spacing: -0.018em;
  }

  .paper-card h2 a {
    color: var(--global-text-color);
  }

  .paper-card p {
    margin: 0.65rem 0 0;
    color: var(--global-text-color-light);
    line-height: 1.7;
  }

  .paper-timeline {
    position: relative;
    margin: 0 0 2.4rem 0.3rem;
    padding-left: 2rem;
  }

  .paper-timeline::before {
    content: "";
    position: absolute;
    top: 0.55rem;
    bottom: 0.6rem;
    left: 0.42rem;
    width: 1px;
    background: color-mix(in srgb, var(--journey-accent) 48%, var(--global-divider-color));
  }

  .timeline-entry {
    position: relative;
    display: grid;
    grid-template-columns: 7rem minmax(0, 1fr);
    gap: 1rem;
    padding: 0 0 1.35rem;
  }

  .timeline-entry:last-child {
    padding-bottom: 0;
  }

  .timeline-entry::before {
    content: "";
    position: absolute;
    top: 0.45rem;
    left: -1.97rem;
    width: 0.78rem;
    height: 0.78rem;
    border: 3px solid var(--global-bg-color);
    border-radius: 50%;
    background: var(--journey-accent);
    box-shadow: 0 0 0 1px color-mix(in srgb, var(--journey-accent) 60%, var(--global-divider-color));
  }

  .timeline-entry time {
    color: var(--global-theme-color);
    font-size: 0.82rem;
    font-weight: 780;
    line-height: 1.6;
  }

  .timeline-entry h3 {
    margin: 0;
    color: var(--global-text-color);
    font-size: 1rem;
    font-weight: 760;
    line-height: 1.5;
  }

  .timeline-entry p {
    margin: 0.28rem 0 0;
    color: var(--global-text-color-light);
    font-size: 0.92rem;
    line-height: 1.65;
  }

  .journey-reflection {
    margin-top: 2.2rem;
    padding: 1.3rem;
    border-radius: 14px;
    background: color-mix(in srgb, var(--journey-accent) 8%, var(--global-card-bg-color));
  }

  .journey-reflection h2 {
    margin-top: 0;
  }

  @media (max-width: 560px) {
    .timeline-entry {
      grid-template-columns: 1fr;
      gap: 0.12rem;
    }
  }
---

<div class="publication-journey">
  <p>
    论文页面通常只留下“发表”或“在投”这类最终状态，真正的过程却由一次次提交、等待、修改和重新选择组成。这里整理两项工作的投稿时间线，也为自己保留一份阶段性记录。
  </p>

  <div class="journey-note">
    <strong>公开说明：</strong>
    本文只保留可以公开的论文信息、日期和阶段性状态。稿件编号、作者邮箱、决定信内容、审稿人联络记录及其他内部备注均已隐去；部分密集事件也进行了合并概括。
  </div>

  <section class="paper-card">
    <div class="paper-card__topline">
      <span class="paper-card__index">论文一 · PCCP</span>
      <span class="paper-card__status">已接收并发表</span>
    </div>
    <h2>
      <a href="https://doi.org/10.1039/D5CP03524D">局域透热表示在非绝热本征值问题中的指数收敛</a>
    </h2>
    <p>
      这项工作经历了两轮大修。从初次投稿到正式接收约五个半月，论文题目也在修改过程中变得更加准确。
    </p>
  </section>

  <div class="paper-timeline" aria-label="PCCP paper timeline">
    <div class="timeline-entry">
      <time datetime="2025-09-12">2025.09.12</time>
      <div>
        <h3>初次投稿</h3>
        <p>向 Physical Chemistry Chemical Physics 提交稿件，同行评审流程开始。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2025-10-21">2025.10.21</time>
      <div>
        <h3>第一轮决定：大修</h3>
        <p>根据评审意见重新梳理论证、补充计算，并调整论文表达。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2025-12-08">2025.12.08</time>
      <div>
        <h3>提交第一轮修改稿</h3>
        <p>完成逐条回复，并提交修订后的稿件。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-01-08">2026.01.08</time>
      <div>
        <h3>第二轮决定：大修</h3>
        <p>进入第二轮集中修改，继续完善收敛性分析与结果呈现。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-02-11">2026.02.11</time>
      <div>
        <h3>提交第二轮修改稿</h3>
        <p>完成补充验证与最终文本修订。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-03-02">2026.03.02</time>
      <div>
        <h3>正式接收</h3>
        <p>稿件被接收；随后完成出版与归档流程。</p>
      </div>
    </div>

  </div>

  <section class="paper-card">
    <div class="paper-card__topline">
      <span class="paper-card__index">论文二 · Tensor Networks</span>
      <span class="paper-card__status">Editorial Review · 截至 2026.07.27</span>
    </div>
    <h2>
      <a href="https://doi.org/10.48550/arXiv.2601.16913">张量网络表象中的粗粒化几何量子动力学</a>
    </h2>
    <p>
      第二项工作经历了数次投稿路线调整。下面记录的是同一份稿件从 PRL 开始，先后经过 Nature Communications、Chemical Science，再到 JCTC 的过程。
    </p>
  </section>

  <div class="paper-timeline" aria-label="Tensor-network paper timeline">
    <div class="timeline-entry">
      <time datetime="2026-01-23">2026.01.23</time>
      <div>
        <h3>投稿 Physical Review Letters</h3>
        <p>稿件以 Letter 形式提交，并进入编辑处理流程。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-02-05">2026.02–04</time>
      <div>
        <h3>外审阶段</h3>
        <p>编辑部组织同行评审。出于保密考虑，具体审稿人联络过程不在此展开。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-04-16">2026.04.16</time>
      <div>
        <h3>收到阶段性决定与评审意见</h3>
        <p>PRL 阶段结束，随后重新评估稿件定位与投稿方向。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-06-11">2026.06.11–18</time>
      <div>
        <h3>转投 Nature Communications</h3>
        <p>完成投稿，稿件进入编辑分配与初步处理阶段；之后再次调整投稿路线。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-07-20">2026.07.20</time>
      <div>
        <h3>投稿 Chemical Science</h3>
        <p>完成新一轮投稿并收到系统确认。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-07-24">2026.07.24</time>
      <div>
        <h3>初步评估结束</h3>
        <p>稿件未进入外审。我们随即整理材料并准备下一次投稿。</p>
      </div>
    </div>

    <div class="timeline-entry">
      <time datetime="2026-07-27">2026.07.27</time>
      <div>
        <h3>投稿 Journal of Chemical Theory and Computation</h3>
        <p>稿件已提交，当前状态为 Editorial Review。</p>
      </div>
    </div>

  </div>

  <section class="journey-reflection">
    <h2>写在最后</h2>
    <p>
      两条时间线很不一样：第一篇沿着“评审—修改—再评审”的路径逐步收敛；第二篇则不断重新寻找最合适的读者与期刊定位。它们共同提醒我，投稿并不是研究完成后的简单手续，而是研究表达继续被检验、被重写的过程。
    </p>
    <p>
      等待并不会自动产生答案，但每一次决定都能帮助我们更清楚地理解工作的边界、价值和叙述方式。继续记录，也继续推进。
    </p>
  </section>
</div>
