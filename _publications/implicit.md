---
layout: publication_page
show: true
noheader: true

title: "Implicit Bias in Noisy-SGD: With Applications to Differentially Private Training"
description: 

date: 2024-02-19

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta, École polytechnique]
  - name: Maxime Sylvestre
    affiliations: [Université Paris-Dauphine, PSL]
  - name: Alain Durmus
    affiliations: [École polytechnique]

journal: International Conference on Artificial Intelligence and Statistics (AISTATS)
bib: /assets/bibliography/implicit.txt
pdf: /assets/publis/implicit/paper.pdf 
arxiv: https://arxiv.org/abs/2210.03403
img: /assets/publis/implicit/splash.png

header-includes:
  - \usepackage[ruled,vlined,linesnumbered]{algorithm2e}
---

## Abstract

*Context* 
- Differential Privacy (DP) has become the gold standard to ensure that a machine learning model does not memorize its training data.
- DP-SGD is popular for training DNNs with (ε, δ)-DP guarantees by adding noise to clipped gradients. We explore how the noise can increase SGD's implicit bias (small batch better than large).
- Why? Our ICML "TAN" (https://arxiv.org/abs/2210.03403) paper highlighted a DP-SGD bottleneck: it needs large batches for good privacy guarantees, but this can harm utility. Indeed, performance can decrease with batch size at fixed effective noise $$\sigma/B$$ and fixed number of training steps.
  
<img src="/assets/publis/implicit/dpsgd_eq.png" class="img-fluid thumbnail mt-2" alt="DP-SGD update: individual gradients are clipped, and Gaussian noise is added to the sum.">

*How?*
- For SGD, the noise structure inherent to stochasticity is known to cause the same implicit bias. Here we observe that Noisy-SGD (DP-SGD w/o clipping = SGD + gaussian) has a similar bias, even with (Big!) isotropic Gaussian noise. On ImageNet with a NF-ResNet, σ/B fixed:

<img src="/assets/publis/implicit/fig1.png" class="img-fluid thumbnail mt-2" alt="Comparaison of SGD, DP-SGD and Noisy-SGD when training from scratch on ImageNet.">


- We thus study the solution of continuous versions of Noisy-SGD for Linear Least Square and Diagonal Linear Network (DLN). DLN is a non-convex toy NN that has properties similar to DNNs. We derive proofs that the implicit bias can indeed be amplified by the additional noise.
- e.g, for DLN, same setup as (Pesme et al., 2021), we look at a sparse linear regression. Our addition of Gaussian noise disrupts a crucial KKT condition, necessitating a mathematical alternative. We show that Noisy-SGD leads to a solution closer to the sparse ground truth than SGD.

<img src="/assets/publis/implicit/splash.png" class="img-fluid thumbnail mt-2" alt="Sparce regression with a Diagonal Linear network: GD, SGD and Noisy-SGD.">

- Disclaimer: Noisy-SGD is used as a DP-SGD substitute but differs from both a privacy and optimization perspective to the DP algorithm due to (1) vanishing noise and (2) non-clipped individual gradients. It is a first approx: see the paper discussion section.
- Future work could leverage methods developed to improve large-batch training in non-private settings to enhance DP-SGD performance. 


<!-- ## Video

<p align="center"><iframe width="560" height="315" src="" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p> -->

## Links

- [`arXiv`]({{page.arxiv}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})

