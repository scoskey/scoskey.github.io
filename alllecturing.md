---
layout: page
title: All lecturing
permalink: /alllecturing
---

# All lecturing

{% assign prevyear = "X" %}

{% for post in site.categories.lecture %}

{% assign postyear = post.date | date: "%Y" %}
{% if postyear != prevyear %} *{{ postyear }}* {% assign prevyear = postyear %} {% else %} &nbsp; {% endif %}

: [{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}
