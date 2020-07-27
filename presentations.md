---
layout: page
title: Presentations
permalink: /presentations
---

# Presentations

(Showing selected presentations; [view all presentations](/allpresentations))

{% assign prevyear = "X" %}

{% for post in site.categories.presentation %}
  {% if post.selected %}

{% assign postyear = post.date | date: "%Y" %}
{% if postyear != prevyear %} {{ postyear }} {% assign prevyear = postyear %} {% else %} &nbsp; {% endif %}

: [{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

