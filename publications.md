---
layout: page
title: Publications
permalink: /publications
---

# Publications and other writing

{% assign curdate = "today" | date: "%Y-%m-%d" %}
{% assign prevdisplaydate = "X" %}
{% assign pubsbydate = site.categories.publication | sort: "pubdate" | reverse %}

{% for post in pubsbydate %}

{% assign pubdate = post.pubdate | date: "%Y-%m-%d" %}

{% if pubdate <= curdate %}
  {% assign displaydate = pubdate | date: "%Y" %}
{% else %}
  {% assign displaydate = "∞" %}
{% endif %}

{% if displaydate != prevdisplaydate %} *{{ displaydate }}* {% assign prevdisplaydate = displaydate %} {% else %} &nbsp; {% endif %}

: [{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

{% endfor %}
