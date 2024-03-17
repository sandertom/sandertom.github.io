---
layout: publication_page
show: true
noheader: true

title: "Differentially Private Representation Learning via Image Captioning"
description: 

date: 2024-03-04

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta, École polytechnique]
  - name: Yaodong Yu
    url: "https://scholar.google.com/citations?user=bZ9oyW8AAAAJ&hl=en"
    affiliations: [FAIR Meta, Berkeley]
  - name: Maziar Sanjabi
    affiliations: [Meta]
  - name: Alain Durmus
    affiliations: [École polytechnique]
  - name: Yi Ma
    affiliations: [Berkeley]
  - name: Kamalika Chaudhuri
    affiliations: [FAIR Meta]
  - name: Chuan Guo
    affiliations: [FAIR Meta]

# journal: International Conference of Machine Learning (ICML)
bib: /assets/bibliography/dpcap.txt
pdf: /assets/publis/dpcap/paper.pdf 
arxiv: https://arxiv.org/abs/2403.02506
img: /assets/publis/dpcap/splash.png

header-includes:
  - \usepackage[ruled,vlined,linesnumbered]{algorithm2e}
---

## Abstract

Differentially private (DP) machine learning is considered the gold-standard solution for training a model from sensitive data while still preserving privacy. However, a major barrier to achieving this ideal is its sub-optimal privacy-accuracy trade-off, which is particularly visible in DP representation learning. Specifically, it has been shown that under modest privacy budgets, most models learn representations that are not significantly better than hand-crafted features. In this work, we show that effective DP representation learning can be done via image captioning and scaling up to internet-scale multimodal datasets. Through a series of engineering tricks, we successfully train a DP image captioner (DP-Cap) on a 233M subset of LAION-2B from scratch using a reasonable amount of computation, and obtaining unprecedented high-quality image features that can be used in a variety of downstream vision and vision-language tasks.  For example, under a privacy budget of $$\varepsilon=8$$, a linear classifier trained on top of learned DP-Cap features attains $$65.8\%$$ accuracy on ImageNet-1K, considerably improving the previous SOTA of $$56.5\%$$. Our work challenges the prevailing sentiment that high-utility DP representation learning cannot be achieved by training from scratch.
  
## Twitter Thread

Check our twitter thread!

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">&quot;Differentially Private Representation Learning via Image Captioning&quot;. We&#39;ve trained a DP image captioner on 200M+ image-text pairs, with SOTA DP image representation and better than non private MAE on certain tasks<a href="https://t.co/BQtU0mtYXc">https://t.co/BQtU0mtYXc</a><a href="https://twitter.com/AIatMeta?ref_src=twsrc%5Etfw">@AIatMeta</a> <a href="https://twitter.com/berkeley_ai?ref_src=twsrc%5Etfw">@berkeley_ai</a> <a href="https://twitter.com/Polytechnique?ref_src=twsrc%5Etfw">@Polytechnique</a> <a href="https://t.co/hfaXZievwp">pic.twitter.com/hfaXZievwp</a></p>&mdash; Tom Sander (@RednasTom) <a href="https://twitter.com/RednasTom/status/1767083465843851384?ref_src=twsrc%5Etfw">March 11, 2024</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<!-- <img src="/assets/publis/tan/poster.png" class="img-fluid thumbnail mt-2" alt="Overview. Total Amount of Noise (TAN) for performance improvement under differential privacy constraing."> --> 


<!-- ## Video

<p align="center"><iframe width="560" height="315" src="" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p> -->

## Links

- [`arXiv`]({{page.arxiv}})
- [`Code`]({{page.code}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})
- ['Twitter'] (https://x.com/RednasTom/status/1767083465843851384?s=20)

