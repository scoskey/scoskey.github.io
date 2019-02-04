---
layout: page
title: Publications
permalink: /publications
---

# Publications and other writing

{% for post in site.categories.publication %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}