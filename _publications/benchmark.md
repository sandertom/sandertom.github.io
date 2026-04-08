---
layout: publication_page
show: true
noheader: true

title: "Detecting Benchmark Contamination through Watermarking"
description:

date: 2025-02-24

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta, École polytechnique]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta, Inria]
  - name: Saeed Mahloujifar
    affiliations: [Meta]
  - name: Alain Durmus
    affiliations: [École polytechnique]
  - name: Chuan Guo
    affiliations: [FAIR Meta]

journal: ICLR Workshop, 2025
arxiv: https://arxiv.org/abs/2502.17259
img: /assets/publis/benchmark/splash.png

---

<p align="center">
  <img src="{{page.img}}" class="img-fluid thumbnail mt-2" style="max-width: 75%;">
</p>

## Abstract

Benchmark contamination poses a significant challenge to the reliability of Large Language Models (LLMs) evaluations, as it is difficult to assert whether a model has been trained on a test set. We introduce a solution to this problem by watermarking benchmarks before their release. The embedding involves reformulating the original questions with a watermarked LLM, in a way that does not alter the benchmark utility. During evaluation, we can detect "radioactivity", i.e. traces that the text watermarks leave in the model during training, using a theoretically grounded statistical test. We test our method by pre-training 1B models from scratch on 10B tokens with controlled benchmark contamination, and validate its effectiveness in detecting contamination on ARC-Easy, ARC-Challenge, and MMLU. Results show similar benchmark utility post-watermarking and successful contamination detection when models are contaminated enough to enhance performance, e.g. p-val $$=10^{-3}$$ for +5% on ARC-Easy.

## Links

- [`arXiv`]({{page.arxiv}})
