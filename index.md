---
layout: default
title: Home
---

<section class="hero">
  <img class="hero-photo" src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="Ana Maria Ruiz">
  <div>
    <p class="kicker">$ whoami</p>
    <h1>Hi! I am Ana Maria Ruiz 👋</h1>
    <p class="hero-subtitle">Data engineer and tech enthusiast, passionate about community building and diving into complex problems.</p>
    <p class="hero-links">
      <a class="btn" href="{{ '/projects/' | relative_url }}">See my projects</a>
      <a class="btn btn-secondary" href="{{ '/blog/' | relative_url }}">Read the blog</a>
    </p>
  </div>
</section>

## My tech work

-  Data engineer with experience in SQL, Snowflake and AWS.
-  Currently volunteering with my tech skills.
-  Learning more about AWS and starting with Rust.

In my spare time I enjoy paper crafting and learning about universal history.

## Featured projects

<div class="card-grid">
{%- assign featured = site.projects | sort: "order" -%}
{%- for project in featured limit:3 -%}
  {%- include project-card.html project=project -%}
{%- endfor -%}
</div>

[cd ~/projects →]({{ '/projects/' | relative_url }}){: .more-link}

## Latest posts

<ul class="post-list">
{%- for post in site.posts limit:3 -%}
  <li>
    <span class="post-meta">{{ post.date | date: site.minima.date_format }}</span>
    <h3><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
  </li>
{%- endfor -%}
</ul>

[cd ~/blog →]({{ '/blog/' | relative_url }}){: .more-link}
