---
title: "Rethinking Weak-to-Strong Augmentation in Source-Free Domain Adaptive Object Detection"
importance: 0
collection: publications
category: underreviews
tags:
  - co-author
  - source-free object detection
  - style
  - teacher-student
  - contrastive learning
  - clustering
permalink: /publications/wscol
header:
  teaser: "WSCOL/overview.png"
inner:
  teaser: "WSCOL/overview.png"

author: 'Jiuzheng Yang, Song Tang, Yangkuiyi Zhang, **Shuaifeng Li**, Mao Ye, Jianwei Zhang, Xiatian Zhu'
date: 2024-10-7
venue: '*arXiv preprint*'
supp: ''

keyword: '**Key Words:** Source-Free Object Detection; Weak-to-Strong Contrastive Learning'
excerpt: ''

paperurl: 'https://arxiv.org/pdf/2410.05557'
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
Source-Free domain adaptive Object Detection (SFOD) aims to transfer a detector (pre-trained on source domain) to new unlabelled target domains. Current SFOD methods typically follow the Mean Teacher framework, where weak-to-strong augmentation provides diverse and sharp contrast for self-supervised learning. However, this augmentation strategy suffers from an inherent problem called crucial semantics loss: Due to random, strong disturbance, strong augmentation is prone to losing typical visual components, hindering cross-domain feature extraction. To address this thus-far ignored limitation, **this paper introduces a novel Weak-to-Strong Contrastive Learning (WSCoL) approach**. The core idea is to distill semantics lossless knowledge in the weak features (from the weak/teacher branch) to guide the representation learning upon the strong features (from the strong/student branch). To achieve this, we project the original features into a shared space using a mapping network, thereby reducing the bias between the weak and strong features. Meanwhile, a weak features-guided contrastive learning is performed in a weak-to-strong manner alternatively. Specifically, we first conduct an adaptation-aware prototype-guided clustering on the weak features to generate pseudo labels for corresponding strong features matched through proposals. Sequentially, we identify positive-negative samples based on the pseudo labels and perform cross-category contrastive learning on the strong features where an uncertainty estimator encourages adaptive background contrast. Extensive experiments demonstrate that WSCoL yields new state-of-the-art performance, offering a built-in mechanism mitigating crucial semantics loss for traditional Mean Teacher framework. The code and data will be released soon.
" | markdownify}}</div>

<h2 style="margin: 0.5em 0 0.5em;" >Cite this paper</h2>
```bib
@article{yang2024rethinking,
  title={Rethinking Weak-to-Strong Augmentation in Source-Free Domain Adaptive Object Detection},
  author={Yang, Jiuzheng and Tang, Song and Zhang, Yangkuiyi and Li, Shuaifeng and Ye, Mao and Zhang, Jianwei and Zhu, Xiatian},
  journal={arXiv preprint arXiv:2410.05557},
  year={2024}
}
```