---
layout: page
permalink: /
title: Home
description: AI Research Scientist at Meta FAIR. PhD from École polytechnique and Meta FAIR.

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

  I am an AI Research Scientist at [Meta FAIR](https://ai.meta.com/research/) (Fundamental AI Research) in Paris. I completed my PhD at FAIR and [École polytechnique](https://www.polytechnique.edu/en), advised by [Chuan Guo](https://scholar.google.com/citations?user=0gp5M-kAAAAJ&hl=en) and [Alain Durmus](https://scholar.google.fr/citations?user=nqLKv6EAAAAJ&hl=fr), and previously by [Alexandre Sablayrolles](https://scholar.google.fr/citations?hl=fr&user=Wy8wM-cAAAAJ) and [Pierre Stock](https://scholar.google.fr/citations?hl=fr&user=3e2-59cAAAAJ).

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


## News

{% if page.news %}
  {% include news.html %}
{% endif %}
