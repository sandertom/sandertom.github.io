---
layout: publication_page
show: true
noheader: true

title: "How Good is Post-Hoc Watermarking With Language Model Rephrasing?"
description:

date: 2026-01-01

authors:
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta]
  - name: Hady Elsahar
    affiliations: [Meta]
  - name: Haonan Chang
    affiliations: [Meta]
  - name: Tomáš Souček
    affiliations: [Meta]
  - name: Vlad Lacatusu
    affiliations: [Meta]

journal: Preprint, 2026
arxiv: https://arxiv.org/abs/2512.16904
img: /assets/publis/posthoc/splash.png

---

<p align="center">
  <img src="{{page.img}}" class="img-fluid thumbnail mt-2" style="max-width: 75%;">
</p>

## Abstract

Generation-time text watermarking embeds statistical signals into text for traceability of AI-generated content. We explore *post-hoc watermarking* where an LLM rewrites existing text while applying generation-time watermarking, to protect copyrighted documents, or detect their use in training or RAG via watermark radioactivity. Unlike generation-time approaches, which is constrained by how LLMs are served, this setting offers additional degrees of freedom for both generation and detection. We investigate how allocating compute (through larger rephrasing models, beam search, multi-candidate generation, or entropy filtering at detection) affects the quality-detectability trade-off. Our strategies achieve strong detectability and semantic fidelity on open-ended text such as books. Among our findings, the simple Gumbel-max scheme surprisingly outperforms more recent alternatives under nucleus sampling, and most methods benefit significantly from beam search. However, most approaches struggle when watermarking verifiable text such as code, where we counterintuitively find that smaller models outperform larger ones. This study reveals both the potential and limitations of post-hoc watermarking, laying groundwork for practical applications and future research.

## Links

- [`arXiv`]({{page.arxiv}})
