---
layout: page
title: Courses
permalink: /courses
---

# Current courses

{% for post in site.categories.course %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign lower = "August 1, 2016" | date: '%s' %}
  {% if postdate >= lower %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

# Fall 2014 &ndash; Spring 2016

{% for post in site.categories.course %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign lower = "August 1, 2014" | date: '%s' %}
  {% assign upper = "August 1, 2016" | date: '%s' %}
  {% if postdate >= lower and postdate < upper %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

# Fall 2012 &ndash; Spring 2014

{% for post in site.categories.course %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign lower = "August 1, 2012" | date: '%s' %}
  {% assign upper = "August 1, 2014" | date: '%s' %}
  {% if postdate >= lower and postdate < upper %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}

# Prior to Boise State

{% for post in site.categories.course %}
  {% assign postdate = post.date | date: '%s' %}
  {% assign upper = "August 1, 2012" | date: '%s' %}
  {% if postdate < upper %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}

  {% endif %}
{% endfor %}
