---
layout: publication_page
show: true
noheader: true

title: "TextSeal: A Localized LLM Watermark for Provenance & Distillation Protection"
description:

date: 2026-05-12

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta]
  - name: Hongyan Chang
    affiliations: [Meta]
  - name: Tomáš Souček
    affiliations: [Meta]
  - name: Tuan Tran
    affiliations: [Meta]
  - name: Valeriu Lacatusu
    affiliations: [Meta]
  - name: Sylvestre-Alvise Rebuffi
    affiliations: [Meta]
  - name: Alexandre Mourachko
    affiliations: [Meta]
  - name: Surya Parimi
    affiliations: [Meta]
  - name: Christophe Ropers
    affiliations: [Meta]
  - name: Rashel Moritz
    affiliations: [Meta]
  - name: Vanessa Stark
    affiliations: [Meta]
  - name: Hady Elsahar
    affiliations: [Meta]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]

journal: Preprint, 2026
arxiv: https://arxiv.org/abs/2605.12456
img: /assets/publis/textseal/splash.png

---

## Abstract

We introduce TextSeal, a state-of-the-art watermark for large language models. Building on Gumbel-max sampling, TextSeal introduces dual-key generation to restore output diversity, along with entropy-weighted scoring and multi-region localization for improved detection. It supports serving optimizations such as speculative decoding and multi-token prediction, and does not add any inference overhead. TextSeal strictly dominates baselines like SynthID-text in detection strength and is robust to dilution, maintaining confident localized detection even in heavily mixed human/AI documents. The scheme is theoretically distortion-free, and evaluation across reasoning benchmarks confirms that it preserves downstream performance; while a multilingual human evaluation (6000 A/B comparisons, 5 languages) shows no perceptible quality difference. Beyond its use for provenance detection, TextSeal is also ``radioactive'': its watermark signal transfers through model distillation, enabling detection of unauthorized use.

## Links

- [`arXiv`]({{page.arxiv}})
