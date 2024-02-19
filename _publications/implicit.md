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
  
<img src="/assets/publis/tan/poster.png" class="img-fluid thumbnail mt-2" alt="Overview. Total Amount of Noise (TAN) for performance improvement under differential privacy constraing.">

*How?*
- We first use the tools of Rényi Differential Privacy (RDP) to highlight that the privacy budget, when not overcharged, only depends on the total amount of noise (TAN) injected throughout training.
We then derive scaling laws for training models with DP-SGD to optimize hyper-parameters with more than a $$\times 100$$ reduction in computational budget.
- We apply the proposed method on CIFAR-10 and ImageNet and, in particular, strongly improve the state-of-the-art on ImageNet with a $$+9$$ points gain in top-1 accuracy for a privacy budget $$\varepsilon = 8$$.

*When?*
- The method could apply whenever a pratictioner wants to train a machine learning model with Differential Privacy guarantees. 
They would just need to simulate training using the same TAN but with much smaller batch sizes and perform hyper-parameter tuning.
- At the end, these hyper-parameters can be used but this time with the large batch that ensures good privacy guarantees. 


<!-- ## Video

<p align="center"><iframe width="560" height="315" src="" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p> -->

## Links

- [`arXiv`]({{page.arxiv}})
- [`Code`]({{page.code}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})

