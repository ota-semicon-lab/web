---
layout: page
title: Projects
permalink: /projects/
description: 半導体を中心とした先進的な材料の研究を行っています.
nav: true
nav_order: 2
display_categories: [work]
horizontal: false
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <img src="{{ '/assets/img/Project.png' | relative_url }}" class="img-fluid rounded z-depth-1" alt="Project Image">
  </div>
</div>

<br>

<div class="projects">
  {% assign projects = site.projects | where: "category", "work" | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
