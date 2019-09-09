---
layout: page
title: Presentations
permalink: /presentations
---
# Selected presentations

(You can also [view all presentations](/allpresentations))

{% for post in site.categories.presentation %}
  {% if post.selected %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

