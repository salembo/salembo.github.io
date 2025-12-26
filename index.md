---
layout: home
title: Inicio
---

# ¡Hi! I am Ana Maria Ruiz 👋

I am a data engineer and tech entusiast passionate about community building, and diving into complex problems. In my spare time I enjoy paper crafting or learning about universal history.  I have experience on SQL, Snowflake and currently learning more about AWS, dbt and Rust. 

## My tech work

- 🚀 I am a data engineer with expertise in SQL, Snowflake and AWS.
- 💡 Currently volunteering using my tech skills. 
- 🌱 Learning more about AWS, and starting with Rust. Dbt coming soon.

## My projects

{% for project in site.projects limit:3 %}
- [{{ project.title }}]({{ project.url }}) - {{ project.description }}
{% endfor %}

[Take a look at all my projects →](/projects)

## Latest posts

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[Take a look at all my posts →](/blog)