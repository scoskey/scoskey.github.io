---
layout: page
title: Students
permalink: /students
---

# Master's projects

{% for post in site.categories.masters-thesis %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}

# Undergraduate projects

{% for post in site.categories.senior-thesis %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}