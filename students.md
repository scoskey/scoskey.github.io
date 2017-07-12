---
layout: page
title: Students
permalink: /students
---

# Master's thesis students

{% for post in site.categories.masters-thesis %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}

# Senior thesis students

{% for post in site.categories.senior-thesis %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}