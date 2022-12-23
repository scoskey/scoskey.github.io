---
layout: page
title: Students
permalink: /students
---

# Master's thesis students

{% for post in site.categories.masters-thesis %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}

# Senior thesis students

{% for post in site.categories.senior-thesis %}

{% if post.siteurl %}[{{ post.title }}]({{ post.siteurl }}){% else %}{{ post.title }}{% endif %}  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}