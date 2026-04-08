---
layout: publication_page
show: true
noheader: true

title: "Rethinking the Role of Verbatim Memorization in LLM Privacy"
description:

date: 2025-06-01

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta, École polytechnique]
  - name: Bargav Jayaraman
    affiliations: [Meta]
  - name: Mark Ibrahim
    affiliations: [Meta]
  - name: Chuan Guo
    affiliations: [FAIR Meta]
  - name: Kamalika Chaudhuri
    affiliations: [FAIR Meta]

journal: NeurIPS, 2025
pdf: https://openreview.net/pdf?id=Xuvdo6oMkE
img: /assets/publis/verbatim/splash.png

---

<p align="center">
  <img src="{{page.img}}" class="img-fluid thumbnail mt-2" style="max-width: 75%;">
</p>

## Abstract

Conventional wisdom in machine learning privacy research states that memorization directly implies a loss of privacy. In contrast, a well-generalized model only remembers distributional patterns and preserves privacy of its training data. In this work, we show that this relationship is much more complex for LLMs trained for chat, and depends heavily on how knowledge is encoded and manipulated. To this end, we fine-tune language models on synthetically generated biographical information including PIIs, and try to extract them in different ways after instruction fine-tuning. We find counter to conventional wisdom that better verbatim memorization does not necessarily increase data leakage via chat. We also find that it is easier to extract information via chat from an LLM that is better able to manipulate and process knowledge even if it is smaller, and that not all attributes are equally extractable. This suggests that the relationship between privacy, memorization and language understanding of LLMs is very intricate, and that examining memorization in isolation can lead to misleading conclusions.

## Links

- [`PDF`]({{page.pdf}})
