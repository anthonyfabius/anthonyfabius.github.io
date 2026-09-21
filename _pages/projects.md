---
layout: page
title: projects
permalink: /projects/
description: A growing collection of my projects. [WIP]
nav: true
nav_order: 3
---

<!-- pages/projects.md -->
<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <div class="table-responsive">
    <table class="table table-sm table-borderless">
      {% for project in sorted_projects %}
        {% include projects_list.liquid %}
      {% endfor %}
    </table>
  </div>
</div>
