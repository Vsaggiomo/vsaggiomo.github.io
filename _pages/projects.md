---
layout: page
title: projects
permalink: /projects/
description: My research is driven by a singular mission. The democratization of science through the intersection of NanoTechnology, Material Science, and Open Hardware. I believe that high-end scientific discovery should not be gated by expensive commercial equipment or specialized cleanroom facilities. By repurposing consumer technologies, such as 3D printers and low-cost microcontrollers, we develop "Open Technologies" that empower researchers to fabricate complex 3D microfluidics, automate entire lab workflows, and deploy sophisticated diagnostic sensors in remote, resource-limited settings. Whether it is transforming a cheap 3D printer into a precision laboratory robot or engineering sustainable, bio-based resins for additive manufacturing, my goal is to provide the global scientific community with the tools to innovate freely, transparently, and affordably. Here you can also find my "fun" projects and hobbies. 

nav: true
nav_order: 1
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
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
