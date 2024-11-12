---
layout: publication_page
show: true
noheader: true

title: 'Watermark Anything with Localized Messages'
description: 

date: 2024-11-12

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta, CMAP Ecole polytechnique]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta, Inria]
  - name: Alain Durmus
    url: "https://alain.perso.math.cnrs.fr/"
    affiliations: [CMAP Ecole polytechnique]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [Inria]
  - name: Matthijs Douze
    url: "https://scholar.google.com/citations?user=0eFZtREAAAAJ&hl=en"
    affiliations: [FAIR Meta]

journal: arxiv
arxiv: https://arxiv.org/abs/2411.07231
bib: /assets/bibliography/wam.txt
pdf: /assets/publis/wam/paper.pdf 
img: /assets/publis/wam/splash.png


---

## TL;DR

Image watermarking is promising  for digital content protection. But images often undergo many modifications—spliced or altered by AI. Watermark Anything Model (WAM) not only "where does the image come from," but "what part comes from where."

## Abstract

Image watermarking methods are not tailored to handle small watermarked areas. This restricts applications in real-world scenarios where parts of the image may come from different sources or have been edited. We introduce a deep-learning model for localized image watermarking, dubbed the Watermark Anything Model (WAM). The WAM embedder imperceptibly modifies the input image, while the extractor segments the received image into watermarked and non-watermarked areas and recovers one or several hidden messages from the areas found to be watermarked. The models are jointly trained at low resolution and without perceptual constraints, then post-trained for imperceptibility and multiple watermarks. Experiments show that WAM is competitive with state-of-the art methods in terms of imperceptibility and robustness, especially against inpainting and splicing, even on high-resolution images. Moreover, it offers new capabilities: WAM can locate watermarked areas in spliced images and extract distinct 32-bit messages with less than 1 bit error from multiple small regions – no larger than 10% of the image surface – even for small 256 × 256 images.  Code and models are available at <a href="https://github.com/facebookresearch/watermark-anything">https://github.com/facebookresearch/watermark-anything</a>


## Links

- [`arXiv`]({{page.arxiv}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})