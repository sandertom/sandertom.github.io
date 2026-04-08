---
layout: publication_page
show: true
noheader: true

title: "Pixel Seal: Adversarial-Only Training for Invisible Image and Video Watermarking"
description:

date: 2025-12-22

authors:
  - name: Tomáš Souček
    affiliations: [Meta]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Hady Elsahar
    affiliations: [Meta]
  - name: Sylvestre-Alvise Rebuffi
    affiliations: [Meta]
  - name: Valeriu Lacatusu
    affiliations: [Meta]
  - name: Tuan Tran
    affiliations: [Meta]
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta]
  - name: Alexandre Mourachko
    affiliations: [Meta]

journal: Preprint, 2025
arxiv: https://arxiv.org/abs/2512.16874
img: /assets/publis/pixelseal/splash.png

---

<p align="center">
  <img src="{{page.img}}" class="img-fluid thumbnail mt-2" style="max-width: 75%;">
</p>

## Abstract

Invisible watermarking is essential for tracing the provenance of digital content. However, training state-of-the-art models remains notoriously difficult, with current approaches often struggling to balance robustness against true imperceptibility. This work introduces Pixel Seal, which sets a new state-of-the-art for image and video watermarking. We first identify three fundamental issues of existing methods: (i) the reliance on proxy perceptual losses such as MSE and LPIPS that fail to mimic human perception and result in visible watermark artifacts; (ii) the optimization instability caused by conflicting objectives, which necessitates exhaustive hyperparameter tuning; and (iii) reduced robustness and imperceptibility of watermarks when scaling models to high-resolution images and videos. To overcome these issues, we first propose an adversarial-only training paradigm that eliminates unreliable pixel-wise imperceptibility losses. Second, we introduce a three-stage training schedule that stabilizes convergence by decoupling robustness and imperceptibility. Third, we address the resolution gap via high-resolution adaptation, employing JND-based attenuation and training-time inference simulation to eliminate upscaling artifacts. We thoroughly evaluate the robustness and imperceptibility of Pixel Seal on different image types and across a wide range of transformations, and show clear improvements over the state-of-the-art. We finally demonstrate that the model efficiently adapts to video via temporal watermark pooling, positioning Pixel Seal as a practical and scalable solution for reliable provenance in real-world image and video settings.

## Links

- [`arXiv`]({{page.arxiv}})
