---
layout: page
title: All courses
permalink: /allcourses
---

# All courses

{% assign prevyear = "X" %}

{% for post in site.categories.course %}

{% assign postyear = post.date | date: "%Y" %}
{% if postyear != prevyear %} *{{ postyear }}* {% assign prevyear = postyear %} {% else %} &nbsp; {% endif %}

: [{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}
