---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing
design:
  css_class: vivid-home lab-home

sections:
  - block: hero
    content:
      title: |
        VIVID Lab
      image:
        filename: shiyans.jpg
      text: |
        <div class="lab-hero-kicker">Volumetric Intelligence, Visual Imaging &amp; Data</div>
        <p class="lab-hero-copy">面向<strong>三维视觉、医学影像与空间智能</strong>的研究平台，聚焦从<strong>感知、重建、理解</strong>到<strong>可解释建模</strong>的一体化方法设计，服务真实场景中的稳健分析与智能决策。</p>
        <div class="lab-hero-meta">
          <span>3D Vision</span>
          <span>Medical Imaging</span>
          <span>3D Gaussian Splatting</span>
          <span>SLAM</span>
        </div>
        <div class="lab-hero-actions">
          <a class="btn btn-primary btn-lg" href="./publication/">Selected Papers</a>
          <a class="lab-link-btn" href="./people/">Meet the Team <i class="fas fa-angle-right"></i></a>
        </div>
    design:
      background:
        gradient_start: '#f8f2e8'
        gradient_end: '#dfe9f3'
        gradient_angle: 120
        text_color_light: false
      spacing:
        padding: ['56px', '0', '40px', '0']
      css_class: hero-balanced home-hero lab-hero-panel

  - block: markdown
    content:
      title: Research Focus
      subtitle: Four directions connecting geometry, imaging, and robust machine learning.
      text: |
        <div class="lab-focus-grid">
          <article class="lab-focus-card">
            <div class="lab-card-index">01</div>
            <h3>3D Vision &amp; Point Clouds</h3>
            <p>围绕点云理解、空间结构建模与三维场景感知，探索高效而稳定的几何表示学习方法。</p>
          </article>
          <article class="lab-focus-card">
            <div class="lab-card-index">02</div>
            <h3>Medical Image Analysis</h3>
            <p>面向脑 MRI 等医学影像任务，关注分割、重建与临床可用性的平衡。</p>
          </article>
          <article class="lab-focus-card">
            <div class="lab-card-index">03</div>
            <h3>3DGS &amp; SLAM</h3>
            <p>结合 3D Gaussian Splatting 与定位建图技术，提升真实场景中的表达质量与效率。</p>
          </article>
          <article class="lab-focus-card">
            <div class="lab-card-index">04</div>
            <h3>Clustering &amp; Learning Theory</h3>
            <p>从聚类、结构约束与鲁棒优化出发，研究具有理论支撑的数据建模方法。</p>
          </article>
        </div>
    design:
      columns: '1'
      css_class: vivid-collection lab-overview

  - block: collection
    content:
      title: Publications
      text: ""
      count: 4
      filters:
        folders:
          - publication
        publication_type: 'paper-conference'
      order: desc
    design:
      view: citation
      columns: '1'
      css_class: vivid-collection home-publications lab-publication-section

  - block: collection
    content:
      title: Latest News
      subtitle: Recent paper acceptances, milestones, and lab updates.
      text:
      count: 4
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: compact
      columns: '1'
      css_class: news-compact vivid-collection home-news lab-news-section

  - block: markdown
    content:
      title: Explore VIVID
      subtitle: Clear entry points for people, publications, and collaboration.
      text: |
        <div class="lab-route-grid">
          <a class="lab-route-card" href="./people/">
            <span class="lab-route-label">People</span>
            <h3>Research Team</h3>
            <p>View faculty, students, and collaborators across the lab.</p>
          </a>
          <a class="lab-route-card" href="./publication/">
            <span class="lab-route-label">Output</span>
            <h3>Publication Archive</h3>
            <p>Browse papers, PDFs, code links, and conference publications.</p>
          </a>
          <a class="lab-route-card" href="./contact/">
            <span class="lab-route-label">Connect</span>
            <h3>Contact &amp; Collaboration</h3>
            <p>Reach out for research exchange, graduate opportunities, and joint projects.</p>
          </a>
        </div>
    design:
      columns: '1'
      css_class: vivid-collection lab-route-section

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        <div class="lab-cta-panel">
          <div class="lab-cta-kicker">Collaborate with VIVID</div>
          <h2>Open to academic collaboration, graduate recruitment, and interdisciplinary projects.</h2>
          <p>We welcome connections with researchers, students, and industry partners working at the intersection of visual intelligence and data-driven imaging.</p>
          <div class="lab-hero-actions lab-cta-actions">
            <a class="btn btn-primary btn-lg" href="./contact/">Contact the Lab</a>
            <a class="lab-link-btn" href="./publication/">Browse Publications <i class="fas fa-angle-right"></i></a>
          </div>
        </div>
    design:
      columns: '1'
      css_class: vivid-cta lab-home-cta
---
