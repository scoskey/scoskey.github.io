---
layout: page
title: All courses
permalink: /allcourses
---

# All courses

{% for post in site.categories.course %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}
