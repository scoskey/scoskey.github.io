---
layout: page
title: Courses
permalink: /courses
---
# Recent courses

{% for post in site.categories.course %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign lower = "August 1, 2015" | date: '%s' %}
  {% if postdate >= lower %}

[{{ post.title }}]({{ post.url }}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

You can also view [all courses](/allcourses).