---
layout: page
title: Blog
permalink: /blog/
---

Here I share my experiences, learnings and reflections on data engineering, technology and the projects I build.

<ul class="post-list">
{%- for post in site.posts -%}
  <li class="post-item">
    <span class="post-meta">{{ post.date | date: site.minima.date_format }}</span>
    <h3><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
    {%- if post.description -%}
    <p>{{ post.description }}</p>
    {%- else -%}
    {{ post.excerpt }}
    {%- endif -%}
    {%- if post.tags.size > 0 -%}
    <p class="tags">{% for t in post.tags %}<span class="tag">{{ t }}</span>{% endfor %}</p>
    {%- endif -%}
  </li>
{%- endfor -%}
</ul>

<p class="rss-subscribe">Want to follow along? Subscribe <a href="{{ '/feed.xml' | relative_url }}">via RSS</a>, follow me on <a href="https://github.com/salembo">GitHub</a> or connect on <a href="https://www.linkedin.com/in/anamariaruizruiz">LinkedIn</a>.</p>
