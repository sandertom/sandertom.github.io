---
layout: publication_page
show: true
noheader: true

title: "TextSeal2: Distortion-Free LLM Watermarking with Copula Mixing and Memoryless Races"
description:

date: 2026-10-29

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Itai Gat
    affiliations: [Meta]
  - name: Haiming Bao
    affiliations: [Meta]
  - name: Jiaxin Shi
    affiliations: [Meta]
  - name: Jason Park
    affiliations: [Meta]
  - name: Valeriu Lacatusu
    affiliations: [Meta]
  - name: Sylvestre-Alvise Rebuffi
    affiliations: [Meta]
  - name: Hongyan Chang
    affiliations: [Meta]
  - name: Hady Elsahar
    affiliations: [Meta]
  - name: Tomáš Souček
    affiliations: [Meta]
  - name: Tuan Tran
    affiliations: [Meta]
  - name: Surya Parimi
    affiliations: [Meta]
  - name: Alexandre Mourachko
    affiliations: [Meta]

journal: Preprint, 2026
arxiv: https://arxiv.org/abs/2610.40613
img: /assets/publis/textseal2/splash.png

---

<p align="center">
  <video controls style="max-width: 100%;">
    <source src="/assets/publis/textseal2/textseal2.mp4" type="video/mp4">
  </video>
</p>

## Abstract

We present TextSeal2, a distortion-free watermark for large language models that keeps its signal under speculative decoding: tokens that replace rejected drafts remain watermarked with the same keys, and the acceptance rate is unchanged. It also preserves output diversity and adds no measurable inference latency. Its predecessor, TextSeal, restores diversity in the Gumbel-max scheme by routing each token to one of two keys via a coin flip. This is suboptimal because the detector averages the scores from both keys without knowing which key was used. TextSeal2 instead merges two or more keys into a single virtual key and couples it to fresh noise through AutoMark's Gaussian copula. Any number of keys, including publicly shared keys, can be merged this way without diluting detection. Under speculative decoding, TextSeal2 verifies keyed drafts with one more exponential race, run on the leftovers of the draft races. By memorylessness, this race reproduces block verification, so the output follows the target model exactly. We evaluate TextSeal2 on three LLMs. At equal output token diversity, TextSeal2 detects 8 to 22 percentage points more 100-token answers than TextSeal at a false-positive rate of $10^{-3}$, and is comparable to textGrain while requiring no post-logits optimization. Under speculative decoding, it detects 18 and 22 percentage points more 200-token answers than TextSeal and textGrain, respectively, at the same acceptance rate.

## Links

- [`arXiv`]({{page.arxiv}})
- [`Code`](https://github.com/facebookresearch/textseal)
- [`LinkedIn post`](https://www.linkedin.com/posts/tomsdr_excited-to-share-textseal2-distortion-free-ugcPost-7523003110131142658-ywTt/)
- [`X post`](https://x.com/RednasTom/status/2117273999831138363)
