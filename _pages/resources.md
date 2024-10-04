---
layout: page
title: resources
permalink: /resources/
nav: true
nav_order: 3
display_categories: [resources, fun]
horizontal: false
---

<div class="justify-content-center">
    A growing collection of various non-research stuff.
<div class="justify-content-center">


<!-- pages/projects.md -->

<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "date" | reverse %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  
  <div class="container">
  {%- for project in sorted_projects -%}
    <article class="project">
      {% if project.img %}"
           <a class="project-thumbnail" style="background-image: src="{{ project.img | relative_url }} href="{{project.url | prepend: site.baseurl}}"></a>
      {% else %}
      {% endif %}
      <div class="project-content">
        <h2 class="project-title"><a href="{{project.url | prepend: site.baseurl}}">{{project.title}}</a></h2>
        <p>{{ project.description | strip_html | truncatewords: 15 }}</p>
        <!-- <span class="project-date">{{project.date | date: '%Y, %b %d'}}&nbsp;&nbsp;&nbsp;—&nbsp;</span> -->
        <!-- <span class="project-words">{% capture words %}{{ project.content | number_of_words }}{% endcapture %}{% unless words contains "-" %}{{ words | plus: 250 | divided_by: 250 | append: " minute read" }}{% endunless %}</span> -->
      </div>
    </article>
  {%- endfor %}
  </div>

  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-1">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
