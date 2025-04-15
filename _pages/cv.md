---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}
<hr/>

<style>
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

<h2>🛕 Education</h2>
{% assign education_content1 = "
  - Combined Master and Doctoral Program
    - M.S.: Sep. 2020 – Jun. 2022
    - Ph.D.: Sep. 2022 – Present
  - Computer Science and Technology
  - Supervisor: [Prof. Mao Ye](https://scholar.google.com/citations?user=UUbEzBYAAAAJ)
" %}
{% assign education_content2 = "
  - Computer Science and Technology
  - GPA: 3.82/4.0, Top 20% Students
  - Postgraduate Recommendation
" %}

<hr/>
<div class="education">
  <div class="entry">
    <div class="content">
      <p class="myp">Ph.D., University of Electronic Science and Technology of China</p>
      {{education_content1 | markdownify}}
    </div>
    <div class="time">Sep. 2020 – Present</div>
  </div>
  <div class="entry">
    <div class="content">
      <p class="myp">B.S., University of Electronic Science and Technology of China</p>
      {{education_content2 | markdownify}}
    </div>
    <div class="time">Sep. 2016 – Jun. 2020</div>
  </div>
</div>

<h2 class="myh2">🧐 Research Experience</h2>
<hr/>
{% assign research1 = "
  - Cloud Object Detector Adaptation
" %}
{% assign research2 = "
  - Unsupervised Domain Adaptive Object Detection
  - Source-free Object Detection
" %}
{% assign research3 = "
  - Thermal Pedestrian Detection
  - Multispectral Pedestrian Detection
" %}
<div class="research">
  <div class="entry">
    <div class="content">
      <p class="myp">Large Cloud Model Adaptation</p>
      {{research1 | markdownify}}
    </div>
    <div class="time">2024 – Present</div>
  </div>
  <div class="entry">
    <div class="content">
      <p class="myp">Domain Adaptive Object Detection</p>
      {{research2 | markdownify}}
    </div>
    <div class="time">2020 – Present</div>
  </div>
  <div class="entry">
    <div class="content">
      <p class="myp">Multi-Modal Pedestrian Detection</p>
      {{research3 | markdownify}}
    </div>
    <div class="time">2023 – Present</div>
  </div>
</div>

<h2 class="myh2">🎯 Publications</h2>
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


<h2>🏆️ Selected awards</h2>
<hr/>
- [2024] Second Prize, China Postgraduate Mathematical Contest in Modeling
- [2020–2024] Multiple Academic Excellence Scholarships (First Class, Second Class)
- [2022] Academic Seedling Award, University of Electronic Science and Technology of China
- [2016–2020] Multiple National Encouragement Scholarships and Outstanding Student Scholarships (Top 20% Students)
  
<h2>🧭 Service</h2>
<hr/>
- Conference Reviewer
  - The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2025
  - International Conference on Computer Vision (ICCV), 2025
  - Annual Conference on Neural Information Processing Systems (NeurIPS), 2025
  - ACM International Conference on Multimedia (ACM MM), 2023, 2024, 2025
- Journal Reviewer
  - Knowledge-Based Systems (KBS)