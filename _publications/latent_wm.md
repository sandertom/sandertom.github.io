---
layout: publication_page
show: true
noheader: true

title: "Learning to Watermark in the Latent Space of Generative Models"
description:

date: 2026-01-20

authors:
  - name: Sylvestre-Alvise Rebuffi
    affiliations: [Meta]
  - name: Tuan Tran
    affiliations: [Meta]
  - name: Valeriu Lacatusu
    affiliations: [Meta]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Tomáš Souček
    affiliations: [Meta]
  - name: Nikola Jovanović
    affiliations: [Meta]
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta]
  - name: Hady Elsahar
    affiliations: [Meta]
  - name: Alexandre Mourachko
    affiliations: [Meta]

journal: Preprint, 2026
arxiv: https://arxiv.org/abs/2601.16140
img: /assets/publis/latent_wm/splash.png

---

<p align="center">
  <img src="{{page.img}}" class="img-fluid thumbnail mt-2" style="max-width: 75%;">
</p>

## Abstract

Existing approaches for watermarking AI-generated images often rely on post-hoc methods applied in pixel space, introducing computational overhead and potential visual artifacts. In this work, we explore latent space watermarking and introduce DistSeal, a unified approach for latent watermarking that works across both diffusion and autoregressive models. Our approach works by training post-hoc watermarking models in the latent space of generative models. We demonstrate that these latent watermarkers can be effectively distilled either into the generative model itself or into the latent decoder, enabling in-model watermarking. The resulting latent watermarks achieve competitive robustness while offering similar imperceptibility and up to 20x speedup compared to pixel-space baselines. Our experiments further reveal that distilling latent watermarkers outperforms distilling pixel-space ones, providing a solution that is both more efficient and more robust.

## Links

- [`arXiv`]({{page.arxiv}})
