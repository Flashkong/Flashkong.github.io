---
permalink: /
title: ""
author_profile: true
layout: archive
redirect_from: 
  - /about/
  - /about.html
---
<style>
  body {
    line-height: 1.5;
  }
  .entry {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
}

  .entry .content {
    flex: 3; /* 主内容宽度 */
  }

  .entry .time {
    flex: 1; /* 时间宽度 */
    text-align: right; /* 时间右对齐 */
    font-style: italic; /* 可选：时间的字体样式 */
  }

  .myp {
    margin-top: 0;
  }

  .myh2 {
    margin-top: 1em;
  }

</style>

<p style="text-align: justify;">
I am a Ph.D. student at CVLAB, University of Electronic Science and Technology of China (UESTC), supervised by Professor <a href="https://scholar.google.com/citations?user=UUbEzBYAAAAJ">Mao Ye</a>. Specifically, I am enrolled in a combined Master and Doctoral program, with my Master's study spanning from 2020 to 2022 and my Ph.D. research continuing from 2022 to the present. Before this, I completed my Bachelor's degree at UESTC (2016–2020).
My primary research interests include Large Cloud Model Adaptation and Domain Adaptive Object Detection. Additionally, I have a broad interest in language-vision models, encompassing recognition, detection, and segmentation tasks.
</p>
<p style="text-align: justify;">
I am open to research collaborations. If you share similar interests or are interested in my previous work, please feel free to contact me.
</p>

<h1 class="myh2">💥 News</h1>
- [2024/09] 1 paper that explores cloud object detector adaptation is accepted by **NeurIPS 2024**!
- [2024/08] 1 paper about black-box domain adaptation is accepted by **ACMM MM 2024**! Congrats to Siying!
- [2023/04] 1 paper using mutual learning for UDA is accepted by **TCSVT**! Congrats to Lihua!
- [2022/08] 1 paper about unsupervised domain adaptation (UDA) is accepted by **ACMM MM 2022**! Congrats to Lihua!
- [2022/03] 1 paper about source-free object detection by overlooking domain style is accepted by **CVPR 2022** (<span style="color: red; font-weight: bold;">ORAL</span>)!
- [2021/12] 1 paper about source-free object detection is accepted by **ACMM MM Asia 2021**! Congrats to Dan Zhang!

<h1 class="myh2">🎯 Publications</h1>
<hr/>
{% assign sorted_by_date = site.publications | sort: 'date' %} <!-- 按日期升序排列 -->
{% assign sorted_posts = sorted_by_date | sort: 'importance' | reverse %} <!-- 按重要性降序排列 -->

{% for post in sorted_posts %}
  {% include archive-single-publication-project.html %}
  {% unless forloop.last %}
{% raw %}
<hr />
{% endraw %}
  {% endunless %}
{% endfor %}

<h1 class="myh2">🏆️ Selected awards</h1>
<hr/>
- [2024] Second Prize, China Postgraduate Mathematical Contest in Modeling
- [2020–2024] Multiple Academic Excellence Scholarships (First Class, Second Class)
- [2022] Academic Seedling Award, University of Electronic Science and Technology of China
- [2016–2020] Multiple National Encouragement Scholarships and Outstanding Student Scholarships (Top 20% Students)

<h1 class="myh2">🧭 Service</h1>
<hr/>
- Conference Reviewer
  - ACM International Conference on Multimedia (ACM MM), 2023, 2024
  - The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2025
- Journal Reviewer
  - Knowledge-Based Systems (KBS)