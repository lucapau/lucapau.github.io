---
layout: page
title: Projects
permalink: /projects/
description: A showcase of my growing collection of technical and creative projects.
nav: true
nav_order: 3
display_categories: [academic, personal]
horizontal: false
---

- title: "QT4in1 App"
  description: "A multi-featured application including Weather Forecasting, Currency Conversion, a Password Manager, and a Note-Taking feature."
  category: academic
  link: "https://github.com/lucapau/QT4in1App"
  importance: 1

- title: "Restaurant Web App"
  description: "A full-stack restaurant review website built with Django."
  category: academic
  link: "https://github.com/lucapau/restaurant_webapp"
  importance: 2

- title: "Unity 2D Platformer"
  description: "A 2D platformer game demonstrating skills in game design, physics, and user experience."
  category: personal
  link: "https://github.com/lucapau/Unity2DPlatformer"
  importance: 3


<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">

    <!-- Personalized category names -->
    <h2 class="category">{{ category == 'academic' ? 'Academic Projects' : 'Personal Projects' }}</h2>

  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}

  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
