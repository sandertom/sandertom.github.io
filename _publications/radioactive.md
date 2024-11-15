---
layout: publication_page
show: true
noheader: true

title: 'Watermarking Makes Language Models Radioactive'
description: 

date: 2024-04-01

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
  - name: Matthijs Douze
    url: "https://scholar.google.com/citations?user=0eFZtREAAAAJ&hl=en"
    affiliations: [FAIR Meta]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [Inria]

journal: Neurips 2024 (Spotlight)
arxiv: https://arxiv.org/abs/2402.14904
bib: /assets/bibliography/radioactive.txt
pdf: /assets/publis/radioactive/paper.pdf 
img: /assets/publis/radioactive/splash.png


---

## TL;DR

We derive reliable statistical methods to spot if a model was trained on watermarked data with high confidence. Our work will be presented as a spotlight at Neurips 2024 (Vancouver).

## Abstract

We investigate the radioactivity of text generated by large language models (LLM), i.e. whether it is possible to detect that such synthetic input was used to train a subsequent LLM. Current methods like membership inference or active IP protection either work only in settings where the suspected text is known or do not provide reliable statistical guarantees. We discover that, on the contrary, it is possible to reliably determine if a language model was trained on synthetic
data if that data is output by a watermarked LLM. Our new methods, specialized for radioactivity, detects with a provable confidence weak residuals of the watermark signal in the fine-tuned LLM. We link the radioactivity contamination level to the following properties: the watermark robustness, its proportion in the training set, and the fine-tuning process. For instance, if the suspect model is open-weight, we demonstrate that training on watermarked instructions can be detected with high confidence (p-value < 10−5) even when as little as 5% of training text is watermarked. Radioactivity detection code is available at <a href="https://github.com/facebookresearch/radioactive-watermark">https://github.com/facebookresearch/radioactive-watermark</a>

## Thread on Twitter

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">OpenAI may secretly know that you trained on GPT outputs!<br>In our work &quot;Watermarking Makes Language Models Radioactive&quot;, we show that training on watermarked text can be easily spotted ☢️ <br>Paper: <a href="https://t.co/EETij4oLF0">https://t.co/EETij4oLF0</a><a href="https://twitter.com/pierrefdz?ref_src=twsrc%5Etfw">@pierrefdz</a> <a href="https://twitter.com/AIatMeta?ref_src=twsrc%5Etfw">@AIatMeta</a> <a href="https://twitter.com/Polytechnique?ref_src=twsrc%5Etfw">@Polytechnique</a> <a href="https://twitter.com/Inria?ref_src=twsrc%5Etfw">@Inria</a> <a href="https://t.co/cjjyhp1DMg">pic.twitter.com/cjjyhp1DMg</a></p>&mdash; Tom Sander (@RednasTom) <a href="https://twitter.com/RednasTom/status/1762109247783891340?ref_src=twsrc%5Etfw">February 26, 2024</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## Links

- [`arXiv`]({{page.arxiv}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})