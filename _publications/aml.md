---
title: "Adaptive Mutual Learning for Unsupervised Domain Adaptation"
importance: 0
collection: publications
category: journals
tags:
  - co-author
  - unsupervised domain adaptation
  - mutual learning
  - teacher-student
permalink: /publications/aml
header:
  teaser: "AML/overview.png"
inner:
  teaser: "AML/overview.png"

author: 'Lihua Zhou, Siying Xiao, Mao Ye, Xiatian Zhu, **Shuaifeng Li**'
date: 2023-04-10
venue: '*IEEE Transactions on Circuits and Systems for Video Technology* (**TCSVT**)'
supp: ''

keyword: '**Key Words:** Unsupervised Domain Adaptation; Adaptive Mutual Learning'
excerpt: ''

paperurl: 'https://ieeexplore.ieee.org/abstract/document/10097830'
codeurl: ''
projecturl: ''
videourl: ''
slidesurl: ''
posterurl: ''

blogurl: ''
zhihuurl: ''
xiaohognshuurl: ''

# citation: ''
---

<h2 style="margin: 1em 0 0.5em;" >Abstract</h2>
<div style="text-align: justify;">{{"
Unsupervised domain adaptation aims to transfer knowledge from labeled source domain to unlabeled target domain. The semi-supervised method based on mean-teacher framework is one of the main stream approaches. By enforcing consistency constraints, it is hopeful that the teacher network will distill useful source domain knowledge to the student network. However, in practice negative transfer often emerges because the performance of the teacher network is not guaranteed to be always better than the student network. To address this limitation, a novel **Adaptive Mutual Learning (AML) strategy** is proposed in this paper. Specifically, given a target sample, the network with worse prediction will be optimized by pushing its prediction close to the better prediction. This is in the spirit of traditional knowledge distillation. On the other hand, the network with better prediction is further refined by requiring its prediction to stay away from the worse prediction. This can be regarded conceptually as reverse knowledge distillation. In this way, two networks learn from each other according to their respective performance. At inference phase, the averaged output of these two networks can be taken as the final prediction. Experimental results demonstrate that our AML achieves competitive results.
" | markdownify}}</div>

<h2 style="margin: 0.5em 0 0.5em;" >Cite this paper</h2>
```bib
@ARTICLE{10097830,
  author={Zhou, Lihua and Xiao, Siying and Ye, Mao and Zhu, Xiatian and Li, Shuaifeng},
  journal={IEEE Transactions on Circuits and Systems for Video Technology}, 
  title={Adaptive Mutual Learning for Unsupervised Domain Adaptation}, 
  year={2023},
  volume={33},
  number={11},
  pages={6622-6634},
  keywords={Knowledge engineering;Task analysis;Feature extraction;Reliability;Adaptation models;Entropy;Adaptive systems;Unsupervised domain adaptation;consistency constraints;adaptive mutual learning},
  doi={10.1109/TCSVT.2023.3265853}
}
```