---
layout: page
title: Publications
permalink: /publications
---

# Publications and other writing

{% for post in site.categories.publication %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}