---
layout: publication_page
show: true
noheader: true

title: "TAN Without a Burn: Scaling Laws of DP-SGD"
description: 

date: 2023-07-15

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta, École polytechnique]
  - name: Pierre Stock
    url: "https://scholar.google.fr/citations?hl=fr&user=3e2-59cAAAAJ"
    affiliations: [FAIR Meta]
  - name: Alexandre Sablayrolles
    url: "https://scholar.google.fr/citations?hl=fr&user=Wy8wM-cAAAAJ"
    affiliations: [FAIR Meta]

journal: International Conference of Machine Learning (ICML)
bib: /assets/bibliography/TAN.txt
pdf: /assets/publis/tan/paper.pdf 
arxiv: https://arxiv.org/abs/2210.03403
img: /assets/publis/tan/splash.png
code: https://github.com/facebookresearch/tan

header-includes:
  - \usepackage[ruled,vlined,linesnumbered]{algorithm2e}
---

## Abstract

*Context* 
- Differential privacy has become the gold standard to ensure that a machine learning model does not memorize its training data.
- Differentially Private methods for training Deep Neural Networks (DNNs) have progressed recently, in particular with the use of massive batches and aggregated data augmentations for a large number of training steps.
These techniques require much more computing resources than their non-private counterparts, shifting the traditional privacy-accuracy trade-off to a privacy-accuracy-compute trade-off.
- We decouple privacy analysis and experimental behavior of noisy training to explore the trade-off with minimal computational requirements. 
  

*How?*
- We first use the tools of Rényi Differential Privacy (RDP) to highlight that the privacy budget, when not overcharged, only depends on the total amount of noise (TAN) injected throughout training.
We then derive scaling laws for training models with DP-SGD to optimize hyper-parameters with more than a $100\times$ reduction in computational budget.
- We apply the proposed method on CIFAR-10 and ImageNet and, in particular, strongly improve the state-of-the-art on ImageNet with a $+9$ points gain in top-1 accuracy for a privacy budget \(\varepsilon=8\).

*When?*
- The method could apply whenever a pratictioner wants to train a machine learning model with Differential Privacy Guarantees. 
They would just need to simulate training using the same TAN but with much smaller batch sizes.
In this setting, one can perform all the hyper-parameter choice that is needed.
- At the end, one can use these parameters but this time with the large batch that ensures good privacy guarantees. 
The parameters that were found in the simulation regime will still be optimal.


<!-- ## Video

<p align="center"><iframe width="560" height="315" src="" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p> -->

## Links

- [`arXiv`]({{page.arxiv}})
- [`Code`]({{page.code}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})

