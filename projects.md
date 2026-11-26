---
layout: page
title: Projects
permalink: /projects/
---

Here is a collection of some projects I have been working on.

<div class="card-grid">
{%- assign projects = site.projects | sort: "order" -%}
{%- for project in projects -%}
  {%- include project-card.html project=project -%}
{%- endfor -%}
</div>
