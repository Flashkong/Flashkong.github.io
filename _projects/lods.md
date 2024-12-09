---
title: "Source-Free Object Detection by Learning to Overlook Domain Style"
collection: projects
tags:
  - first author
  - source-free object detection
  - style
  - style enhancement
  - overlook style
  - teacher-student
permalink: /projects/lods
header:
  teaser: "LODS/idea.png"

author: '**Shuaifeng Li**, Mao Ye, Xiatian Zhu, Lihua Zhou, Lin Xiong'
date: 2022-06-18
venue: '*Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition* (**CVPR**)'
supp: '<span style="color: red;">**ORAL**</span>'

keyword: '**Key Words:** Source-Free Object Detection; Style Enhancement; Overlooking Style'
excerpt: '**We propose a novel learning to overlook domain style strategy for SFOD.**'

paperurl: 'https://openaccess.thecvf.com/content/CVPR2022/html/Li_Source-Free_Object_Detection_by_Learning_To_Overlook_Domain_Style_CVPR_2022_paper.html'
codeurl: 'https://github.com/Flashkong/Source-Free-Object-Detection-by-Learning-to-Overlook-Domain-Style'
projecturl: '/projects/lods'
videourl: 'https://www.youtube.com/watch?v=A7vBStzBZLY'
slidesurl: '/files/LODS/LODS_slides.pptx'
posterurl: '/files/LODS/LODS_poster.pdf'
summaryurl: '/files/LODS/LODS_summary.pdf'

blogurl: ''
zhihuurl: ''
xiaohognshuurl: ''

# citation: ''
---
  <div class="myteaser_old">
    <img src="{{ "LODS/idea1.png" | prepend: "/images/" | prepend: base_path }}" alt="{{ idea }}" style="width:80%;">
  </div>

<h2 style="margin: 1em 0 0.5em;" >Abstract</h2>

<div style="text-align: justify;">{{"
Source-free object detection (SFOD) needs to adapt a detector pre-trained on a labeled source domain to a target domain, with only unlabeled training data from the target domain. Existing SFOD methods typically adopt the pseudo labeling paradigm with model adaption alternating between predicting pseudo labels and fine-tuning the model. This approach suffers from both unsatisfactory accuracy of pseudo labels due to the presence of domain shift and limited use of target domain training data. In this work, we present a novel **Learning to Overlook Domain Style (LODS)** method with such limitations solved in a principled manner. *Our idea is to reduce the domain shift effect by enforcing the model to overlook the target domain style, such that model adaptation is simplified and becomes easier to carry on.* To that end, we enhance the style of each target domain image and leverage the style degree difference between the original image and the enhanced image as a self-supervised signal for model adaptation. By treating the enhanced image as an auxiliary view, we exploit a student-teacher architecture for learning to overlook the style degree difference against the original image, also characterized with a novel style enhancement algorithm and graph alignment constraint. Extensive experiments demonstrate that our LODS yields new state-of-the-art performance on four benchmarks.
" | markdownify}}</div>

<h2 style="margin: 0.5em 0 0.5em;" >Supplement</h2>
<div style="text-align: justify;">{{"
We use the standard Faster R-CNN as the teacher and student. For PASCAL VOC to Clipart and PASCAL VOC to Watercolor, we use Resnet101 as our backbone. For Cityscapes to Foggy-Cityscapes and KITTI to Cityscape, we use VGG16 (without batchnorm) as our backbone.

Note that for the Foggy-Cityscapes dataset, we use the foggy level of 0.02. For Clipart dataset, we use all 1K images for both training and testing.
" | markdownify}}</div>

  <div class="myteaser_old">
    <img src="{{ "LODS/overview1.png" | prepend: "/images/" | prepend: base_path }}" alt="{{ overview }}">
  </div>

  <div class="myteaser_old">
    <img src="{{ "LODS/net.png" | prepend: "/images/" | prepend: base_path }}" alt="{{ net }}" style="width:80%;">
  </div>

  <div class="myteaser_old">
    <img src="{{ "LODS/results1.png" | prepend: "/images/" | prepend: base_path }}" alt="{{ results1 }}">
  </div>

  <div class="myteaser_old">
    <img src="{{ "LODS/results2.png" | prepend: "/images/" | prepend: base_path }}" alt="{{ results2 }}" style="width:80%;">
  </div>

  <div class="myteaser_old">
    <img src="{{ "LODS/results3.png" | prepend: "/images/" | prepend: base_path }}" alt="{{ results3 }}" style="width:80%;">
  </div>

  <div class="myteaser_old">
    <img src="{{ "LODS/results4.png" | prepend: "/images/" | prepend: base_path }}" alt="{{ results4 }}" style="width:80%;">
  </div>


<h2 style="margin: 0.5em 0 0.5em;" >Cite this paper</h2>
```bib
@InProceedings{Li_2022_CVPR,
    author    = {Li, Shuaifeng and Ye, Mao and Zhu, Xiatian and Zhou, Lihua and Xiong, Lin},
    title     = {Source-Free Object Detection by Learning To Overlook Domain Style},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2022},
    pages     = {8014-8023}
}
```