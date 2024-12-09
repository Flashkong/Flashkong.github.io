---
title: "Class Discriminative Adversarial Learning for Unsupervised Domain Adaptation"
importance: 0
collection: publications
category: conferences
tags:
  - co-author
  - unsupervised domain adaptation
  - adversarial learning

permalink: /publications/cdal
header:
  teaser: "CDAL/overview.png"
inner:
  teaser: "CDAL/overview.png"

author: 'Lihua Zhou, Mao Ye, Xiatian Zhu, **Shuaifeng Li**, Yiguang Liu'
date: 2022-10-10
venue: '*Proceedings of the 30th ACM International Conference on Multimedia* (**ACM MM**)'
supp: ''

keyword: '**Key Words:** Unsupervised Domain Adaptation; Class Discriminative Adversarial Learning'
excerpt: ''

paperurl: 'https://ieeexplore.ieee.org/abstract/document/10097830'
codeurl: 'https://github.com/buerzlh/CDAL'
projecturl: ''
videourl: 'https://dl.acm.org/doi/suppl/10.1145/3503161.3548143/suppl_file/MM22-fp1660.mp4'
slidesurl: ''
posterurl: ''

blogurl: ''
zhihuurl: ''
xiaohognshuurl: ''

# citation: ''
---

<h2 style="margin: 1em 0 0.5em;" >Abstract</h2>
<div style="text-align: justify;">{{"
As a state-of-the-art family of Unsupervised Domain Adaptation (UDA), bi-classifier adversarial learning methods are formulated in an adversarial (minimax) learning framework with a single feature extractor and two classifiers. Model training alternates between two steps: (I) constraining the learning of the two classifiers to maximize the prediction discrepancy of unlabeled target domain data, and (II) constraining the learning of the feature extractor to minimize this discrepancy. Despite being an elegant formulation, this approach has a fundamental limitation: Maximizing and minimizing the classifier discrepancy is not class discriminative for the target domain, finally leading to a suboptimal adapted model. To solve this problem, we propose a novel **Class Discriminative Adversarial Learning (CDAL)** method characterized by discovering class discrimination knowledge and leveraging this knowledge to discriminatively regulate the classifier discrepancy constraints on-the-fly. This is realized by introducing an evaluation criterion for judging each classifier's capability and each target domain sample's feature reorientation via objective loss reformulation. Extensive experiments on three standard benchmarks show that our CDAL method yields new state-of-the-art performance. Our code is made available at https://github.com/buerzlh/CDAL.
" | markdownify}}</div>

<h2 style="margin: 0.5em 0 0.5em;" >Cite this paper</h2>
```bib
@inproceedings{10.1145/3503161.3548143,
  author = {Zhou, Lihua and Ye, Mao and Zhu, Xiatian and Li, Shuaifeng and Liu, Yiguang},
  title = {Class Discriminative Adversarial Learning for Unsupervised Domain Adaptation},
  year = {2022},
  isbn = {9781450392037},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {https://doi.org/10.1145/3503161.3548143},
  doi = {10.1145/3503161.3548143},
  abstract = {As a state-of-the-art family of Unsupervised Domain Adaptation (UDA), bi-classifier adversarial learning methods are formulated in an adversarial (minimax) learning framework with a single feature extractor and two classifiers. Model training alternates between two steps: (I) constraining the learning of the two classifiers to maximize the prediction discrepancy of unlabeled target domain data, and (II) constraining the learning of the feature extractor to minimize this discrepancy. Despite being an elegant formulation, this approach has a fundamental limitation: Maximizing and minimizing the classifier discrepancy is not class discriminative for the target domain, finally leading to a suboptimal adapted model. To solve this problem, we propose a novel Class Discriminative Adversarial Learning (CDAL) method characterized by discovering class discrimination knowledge and leveraging this knowledge to discriminatively regulate the classifier discrepancy constraints on-the-fly. This is realized by introducing an evaluation criterion for judging each classifier's capability and each target domain sample's feature reorientation via objective loss reformulation. Extensive experiments on three standard benchmarks show that our CDAL method yields new state-of-the-art performance. Our code is made available at https://github.com/buerzlh/CDAL.},
  booktitle = {Proceedings of the 30th ACM International Conference on Multimedia},
  pages = {4318–4326},
  numpages = {9},
  keywords = {unsupervised domain adaptation, class discriminative adversarial learning, bi-classifier adversarial learning},
  location = {Lisboa, Portugal},
  series = {MM '22}
}
```