---
layout: page
title: Projects
permalink: /projects/
description: 半導体を中心とした先進的な材料の研究を行っています.
nav: true
nav_order: 2
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <img src="{{ site.baseurl }}/assets/img/Project.png" 
         class="img-fluid rounded z-depth-1" 
         alt="Project Image" 
         style="width: 100%;">
  </div>
</div>

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
