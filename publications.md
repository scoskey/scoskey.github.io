---
layout: page
title: Publications
permalink: /publications
---

# Research publications

{% assign pubsbydate = site.categories.publication | sort: "pubdate" | reverse %}

{% for post in pubsbydate %}
  {% if post.selected %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

# Further publications and products

{% for post in pubsbydate %}
  {% unless post.selected %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endunless %}
{% endfor %}