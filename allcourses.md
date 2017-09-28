---
layout: page
title: All courses
permalink: /allcourses
---
# All courses

{% for post in site.categories.course %}

[{{ post.title }}]({{ post.url }}) {{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}
