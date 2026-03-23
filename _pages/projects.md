---
layout: page
title: Projects
permalink: /projects/
description: 半導体を中心とした先進的な材料の研究を行っています.
nav: true
nav_order: 2
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 text-center">
    <h4>当研究室では、第一原理計算や材料インフォマティクスを活用し、次世代デバイスに欠かせないワイドバンドギャップ半導体の物理的解明と、新しい機能材料の探索を行っています。</h4>
  </div>
</div>

<br>

<div class="row justify-content-sm-center">
  <div class="col-sm-6 mt-3 mt-md-0">
    <img src="/web/assets/img/Project.png" class="img-fluid rounded z-depth-1" alt="Project Image" style="display: block; margin: 0 auto;">
  </div>
</div>

<br>
<hr>
<br>

<div class="projects">
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in site.projects %}
      {% if project.category == "work" %}
        {% include projects.liquid %}
      {% endif %}
    {% endfor %}
  </div>
</div>
