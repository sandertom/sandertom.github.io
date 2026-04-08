---
layout: page
permalink: /
title: Home
description: AI Research Scientist at Meta Superintelligence Labs - FAIR. PhD from École polytechnique and Meta FAIR.

profile:
  image: avatar.jpg
  address: >

nav: false
news: true  # includes a list of news items
---

## About me

<div class="row">
  <div class="col-md-8" markdown="1">
  Hi!

  I am an AI Research Scientist at [Meta Superintelligence Labs - FAIR](https://ai.meta.com/research/) (Fundamental AI Research) in Paris. I completed my PhD at FAIR and [École polytechnique](https://www.polytechnique.edu/en), advised by [Chuan Guo](https://scholar.google.com/citations?user=0gp5M-kAAAAJ&hl=en) and [Alain Durmus](https://scholar.google.fr/citations?user=nqLKv6EAAAAJ&hl=fr), and previously by [Alexandre Sablayrolles](https://scholar.google.fr/citations?hl=fr&user=Wy8wM-cAAAAJ) and [Pierre Stock](https://scholar.google.fr/citations?hl=fr&user=3e2-59cAAAAJ).

  My research focuses on privacy preserving machine learning, data protection, and watermarking, from Differential Privacy to media provenance. I am a core contributor to [Meta Seal](https://github.com/facebookresearch/watermark-anything), Meta's official provenance offering.

  Prior to my PhD I studied at [École polytechnique](https://www.polytechnique.edu/en), majoring in computer science and mathematics.
  I also hold a Master's degree from [École Normale Supérieure Paris-Saclay](https://www.universite-paris-saclay.fr/en) where I studied Mathematics for vision and learning (MVA).
  I previously interned at Polytechnique Montreal [Université de Montreal](https://corail-research.github.io/), on Reinforcement Learning for Constraint Programing, and at [BNP-Paribas](https://mabanque.bnpparibas/) where I developed tools for fraud detection.
  I also spent 6 months as a civil servant in Hanoï (Vietnam) working with the director of [USTH](https://usth.edu.vn/en/), a scientific university.

  </div>
  <div class="col-md-4 m-auto" style="text-align: center">
    <img class="img-responsive rounded-circle profile" src="assets/img/{{page.profile.image}}">
  </div>
</div>

## Featured Work

<div class="row">
  <div class="col-md-6 col-lg-3 mb-4">
    <div style="border: 1px solid var(--global-border-color); border-radius: 0.5em; overflow: hidden; height: 100%; display: flex; flex-direction: column;">
      <a href="https://ai.meta.com/blog/meta-seal-media-provenance-watermarking/" target="_blank" style="display: flex; align-items: center; justify-content: center; background: var(--global-bg-color); min-height: 180px; padding: 0.5rem;">
        <img src="/assets/img/icon.png" class="img-fluid" style="max-height: 120px; object-fit: contain;">
      </a>
      <div style="padding: 0.8rem; flex: 1; display: flex; flex-direction: column;">
        <h5><a href="https://ai.meta.com/blog/meta-seal-media-provenance-watermarking/" target="_blank">Meta Seal</a></h5>
        <p style="font-size: 0.85rem; flex: 1;">Core contributor to Meta's official media provenance offering. My open-source projects WAM and TextSeal power this release.</p>
        <span class="badge" style="background-color: var(--global-theme-color); color: white; align-self: flex-start;">Product</span>
      </div>
    </div>
  </div>
  <div class="col-md-6 col-lg-3 mb-4">
    <div style="border: 1px solid var(--global-border-color); border-radius: 0.5em; overflow: hidden; height: 100%; display: flex; flex-direction: column;">
      <a href="/publications/wam/" style="display: flex; align-items: center; justify-content: center; background: var(--global-bg-color); min-height: 180px; padding: 0.5rem;">
        <img src="/assets/publis/wam/splash.png" class="img-fluid" style="max-height: 170px; object-fit: contain;">
      </a>
      <div style="padding: 0.8rem; flex: 1; display: flex; flex-direction: column;">
        <h5><a href="/publications/wam/">Watermark Anything</a></h5>
        <p style="font-size: 0.85rem; flex: 1;">SOTA image watermarking with localization. 1.1k+ ⭐ on <a href="https://github.com/facebookresearch/watermark-anything">GitHub</a>. Core engine behind Meta Seal.</p>
        <span class="badge" style="background-color: var(--global-theme-color); color: white; align-self: flex-start;">ICLR 2025</span>
      </div>
    </div>
  </div>
  <div class="col-md-6 col-lg-3 mb-4">
    <div style="border: 1px solid var(--global-border-color); border-radius: 0.5em; overflow: hidden; height: 100%; display: flex; flex-direction: column;">
      <a href="/publications/radioactive/" style="display: flex; align-items: center; justify-content: center; background: var(--global-bg-color); min-height: 180px; padding: 0.5rem;">
        <img src="/assets/publis/radioactive/splash.png" class="img-fluid" style="max-height: 170px; object-fit: contain;">
      </a>
      <div style="padding: 0.8rem; flex: 1; display: flex; flex-direction: column;">
        <h5><a href="/publications/radioactive/">Radioactive Watermarks</a></h5>
        <p style="font-size: 0.85rem; flex: 1;">Detect if a model was trained on watermarked data. Used to protect datasets and detect distillation. <a href="https://github.com/facebookresearch/radioactive-watermark">Code</a>.</p>
        <span class="badge" style="background-color: var(--global-theme-color); color: white; align-self: flex-start;">NeurIPS 2024 Spotlight</span>
      </div>
    </div>
  </div>
  <div class="col-md-6 col-lg-3 mb-4">
    <div style="border: 1px solid var(--global-border-color); border-radius: 0.5em; overflow: hidden; height: 100%; display: flex; flex-direction: column;">
      <a href="/publications/tan/" style="display: flex; align-items: center; justify-content: center; background: var(--global-bg-color); min-height: 180px; padding: 0.5rem;">
        <img src="/assets/publis/tan/splash.png" class="img-fluid" style="max-height: 170px; object-fit: contain;">
      </a>
      <div style="padding: 0.8rem; flex: 1; display: flex; flex-direction: column;">
        <h5><a href="/publications/tan/">TAN: Scaling Laws of DP-SGD</a></h5>
        <p style="font-size: 0.85rem; flex: 1;">Scaling laws that enable training privacy-preserving models at scale. Deployed in production. <a href="https://github.com/facebookresearch/tan">Code</a>.</p>
        <span class="badge" style="background-color: var(--global-theme-color); color: white; align-self: flex-start;">ICML 2023</span>
      </div>
    </div>
  </div>
</div>


## News

{% if page.news %}
  {% include news.html %}
{% endif %}
