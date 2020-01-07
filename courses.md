---
layout: page
title: Courses
permalink: /courses
---

# Recent courses

(You can also [view all courses](/allcourses))

{% for post in site.categories.course %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign lower = "August 1, 2016" | date: '%s' %}
  {% if postdate >= lower %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

