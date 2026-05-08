---
layout: page
title: Lecturing
permalink: /lecturing
---

# Lecturing

(Showing recent lecturing; [view all lecturing](/alllecturing))

{% assign prevyear = "X" %}

{% for post in site.categories.lecture %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign lower = "January 1, 2019" | date: '%s' %}
  {% if postdate >= lower %}

{% assign postyear = post.date | date: "%Y" %}
{% if postyear != prevyear %} *{{ postyear }}* {% assign prevyear = postyear %} {% else %} &nbsp; {% endif %}

: [{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}
