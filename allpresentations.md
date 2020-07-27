---
layout: page
title: All presenetationss
permalink: /allpresentations
---

# All presentations

{% assign prevyear = "X" %}

{% for post in site.categories.presentation %}

{% assign postyear = post.date | date: "%Y" %}
{% if postyear != prevyear %} {{ postyear }} {% assign prevyear = postyear %} {% else %} &nbsp; {% endif %}

: [{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}
