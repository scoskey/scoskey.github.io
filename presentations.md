---
layout: page
title: Presentations
permalink: /presentations
---
# Selected presentations

{% for post in site.categories.presentation %}
  {% if post.selected %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

You can also view [all presentations](/allpresentations).
