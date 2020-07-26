---
layout: page
title: Publications
permalink: /publications
---

# Publications and other writing

{% assign thisyear = "now" | date: "%Y" | plus: 0 %}
{% assign pubsbydate = site.categories.publication | sort: "pubdate" | reverse %}

{% for post in pubsbydate %}

{% if post.pubdate <= thisyear %} {{ post.pubdate }} {% else %} ∞ {% endif %}

: [{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}
