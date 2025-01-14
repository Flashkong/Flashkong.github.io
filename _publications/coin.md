---
title: "Cloud Object Detector Adaptation by Integrating Different Source Knowledge"
importance: 3
collection: publications
category: conferences
tags:
  - first author
  - cloud object detector adaptation
  - knowledge integration
  - teacher-student
  - CLIP
  - gradient
  - gradient alignment
permalink: /publications/coin
header:
  teaser: "COIN/thumbnail.png"
inner:
  teaser: "COIN/idea.png"

author: '**Shuaifeng Li**, Mao Ye, Lihua Zhou, Nianxin Li, Siying Xiao, Song Tang, Xiatian Zhu'
date: 2024-12-10
venue: '*The Thirty-eighth Annual Conference on Neural Information Processing Systems* (**NeurIPS**)'
supp: ''

keyword: '**Key Words:** Cloud Object Detector Adaptation; Gradient Direction Alignment'
excerpt: '**We propose to explore an interesting and promising problem CODA.**'

paperurl: 'https://openreview.net/pdf?id=S8SEjerTTg'
codeurl: 'https://github.com/Flashkong/COIN'
projecturl: '/projects/coin'
videourl: ''
slidesurl: '/files/COIN/COIN_slides.pdf'
posterurl: '/files/COIN/COIN_poster.pdf'

blogurl: '/blogs/coin'
zhihuurl: 'https://zhuanlan.zhihu.com/p/11666611412'
xiaohognshuurl: ''

# citation: ''
---

<h2 style="margin: 1em 0 0.5em;" >Abstract</h2>

<div style="text-align: justify;">{{"
We propose to explore an interesting and promising problem, **Cloud Object Detector Adaptation (CODA)**, where the target domain leverages detections provided by a large cloud model to build a target detector. Despite with powerful generalization capability, the cloud model still cannot achieve error-free detection in a specific target domain. In this work, we present a novel Cloud Object detector adaptation method by Integrating different source kNowledge (**COIN**). The key idea is to incorporate a public vision-language model (CLIP) to distill positive knowledge while refining negative knowledge for adaptation by self-promotion gradient direction alignment. To that end, *knowledge dissemination, separation, and distillation are carried out successively*. Knowledge dissemination combines knowledge from cloud detector and CLIP model to initialize a target detector and a CLIP detector in target domain. By matching CLIP detector with the cloud detector, knowledge separation categorizes detections into three parts: consistent, inconsistent and private detections such that divide-and-conquer strategy can be used for knowledge distillation. Consistent and private detections are directly used to train target detector; while inconsistent detections are fused based on a consistent knowledge generation network, which is trained by aligning the gradient direction of inconsistent detections to that of consistent detections, because it provides a direction toward an optimal target detector. Experiment results demonstrate that the proposed COIN method achieves the state-of-the-art performance.
" | markdownify}}</div>

<h2 style="margin: 0.5em 0 0.5em;" >Supplement</h2>
*Please note that CODA aims to adapt/distill the cloud detector to target domain, e.g., a target detector, so the use of CLIP is optional. To address the CODA problem, our method, COIN, employs CLIP; however, **this does not imply that the CODA problem setting assumes the existence of a local (CLIP or source domain) detector, nor does it assume that CLIP must necessarily be used.** Please keep this distinction in mind.*

<h2 style="margin: 0.5em 0 0.5em;" >Cite this paper</h2>
```bib
@inproceedings{
    li2024cloud,
    title={Cloud Object Detector Adaptation by Integrating Different Source Knowledge},
    author={Shuaifeng Li and Mao Ye and Lihua Zhou and Nianxin Li and Siying Xiao and Song Tang and Xiatian Zhu},
    booktitle={The Thirty-eighth Annual Conference on Neural Information Processing Systems},
    year={2024},
    url={https://openreview.net/forum?id=S8SEjerTTg}
}
```