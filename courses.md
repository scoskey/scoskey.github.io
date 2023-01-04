---
layout: page
title: Courses
permalink: /courses
---

# Courses

{% assign prevyear = "X" %}

{% for post in site.categories.course %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign lower = "January 1, 2018" | date: '%s' %}
  {% if postdate >= lower %}

{% assign postyear = post.date | date: "%Y" %}
{% if postyear != prevyear %} *{{ postyear }}* {% assign prevyear = postyear %} {% else %} &nbsp; {% endif %}

: [{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

([View all past courses](/allcourses))
