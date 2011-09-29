---
layout: default
title: Projects
---


{% for post in site.pages.categories.projects %}
  * [{{ post.title }}]({{ post.url }})
{% endfor %}

