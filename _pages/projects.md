---
layout: page
title: Projects
permalink: /projects/
description: 
nav: true
nav_order: 2
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 text-center">
    <h4> 密度汎関数理論に基づく第一原理計算によって、半導体を中心とした先進的な物質・材料の研究を行っています.</h4>
  </div>
</div>

<br>

<div class="row justify-content-sm-center">
  <div class="col-sm-4 mt-2">
    <img src="/web/assets/img/Project.png" class="img-fluid rounded z-depth-1" alt="Project Image" style="display: block; margin: 0 auto; opacity: 0.9;">
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
