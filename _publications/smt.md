---
title: "Source-Style Transferred Mean Teacher for Source-data Free Object Detection"
importance: 0
collection: publications
category: conferences
tags:
  - co-author
  - source-free object detection
  - style
  - teacher-student
  - batch normalization
permalink: /publications/smt
header:
  teaser: "SMT/overview.png"
inner:
  teaser: "SMT/overview.png"

author: 'Dan Zhang, Mao Ye, Lin Xiong, **Shuaifeng Li**, Xue Li'
date: 2021-12-10
venue: '*Proceedings of the 3rd ACM International Conference on Multimedia in Asia* (**ACM MM Asia**)'
supp: ''

keyword: '**Key Words:** Source-Free Object Detection; Batch Normalization Adaptation'
excerpt: ''

paperurl: 'https://dl.acm.org/doi/abs/10.1145/3469877.3490584'
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
Unsupervised cross-domain object detection transfers a detection model trained on a source domain to the target domain that has a different data distribution from the source domain. Conventional domain adaptation detection protocols need source domain data during adaptation. However, due to some reasons such as data security, privacy and storage, we cannot access the source data in many practical applications. In this paper, we focus on source-data free domain adaptive object detection, which uses the pre-trained source model instead of the source data for cross-domain adaptation. Due to the lack of source data, we cannot directly align domain distribution between domains. To challenge this, we propose the Source style transferred Mean Teacher (SMT) for source-data free Object Detection. The batch normalization layers in the pre-trained model contain the style information and the data distribution of the non-observed source data. Thus we use the batch normalization information from the pre-trained source model to transfer the target domain feature to the source-like style feature to make full use of the knowledge from the pre-trained source model. Meanwhile, we use the consistent regularization of the Mean Teacher to further distill the knowledge from the source domain to the target domain. Furthermore, we found that by adding perturbations associated with the target domain distribution, the model can increase the robustness of domain-specific information, thus making the learned model generalized to the target domain. Experiments on multiple domain adaptation object detection benchmarks verify that our method is able to achieve state-of-the-art performance.
" | markdownify}}</div>

<h2 style="margin: 0.5em 0 0.5em;" >Cite this paper</h2>
```bib
@inproceedings{10.1145/3469877.3490584,
  author = {Zhang, Dan and Ye, Mao and Xiong, Lin and Li, Shuaifeng and Li, Xue},
  title = {Source-Style Transferred Mean Teacher for Source-data Free Object Detection},
  year = {2022},
  isbn = {9781450386074},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {https://doi.org/10.1145/3469877.3490584},
  doi = {10.1145/3469877.3490584},
  abstract = {Unsupervised cross-domain object detection transfers a detection model trained on a source domain to the target domain that has a different data distribution from the source domain. Conventional domain adaptation detection protocols need source domain data during adaptation. However, due to some reasons such as data security, privacy and storage, we cannot access the source data in many practical applications. In this paper, we focus on source-data free domain adaptive object detection, which uses the pre-trained source model instead of the source data for cross-domain adaptation. Due to the lack of source data, we cannot directly align domain distribution between domains. To challenge this, we propose the Source style transferred Mean Teacher (SMT) for source-data free Object Detection. The batch normalization layers in the pre-trained model contain the style information and the data distribution of the non-observed source data. Thus we use the batch normalization information from the pre-trained source model to transfer the target domain feature to the source-like style feature to make full use of the knowledge from the pre-trained source model. Meanwhile, we use the consistent regularization of the Mean Teacher to further distill the knowledge from the source domain to the target domain. Furthermore, we found that by adding perturbations associated with the target domain distribution, the model can increase the robustness of domain-specific information, thus making the learned model generalized to the target domain. Experiments on multiple domain adaptation object detection benchmarks verify that our method is able to achieve state-of-the-art performance.},
  booktitle = {Proceedings of the 3rd ACM International Conference on Multimedia in Asia},
  articleno = {4},
  numpages = {8},
  keywords = {style translation, source free object detection, neural networks, domain adaptation},
  location = {Gold Coast, Australia},
  series = {MMAsia '21}
}
```