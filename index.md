---
layout: page
---

<img style="float:right;margin-left:10px" src="{{ site.baseurl }}/assets/dogsquaresmall.png" alt="dog icon" />

Department of Mathematics  
University College London  
25 Gordon Street  
London WC1H 0AY  
United Kingdom

Department of Mathematics  
Boise State University  
1910 University Dr  
Boise, ID 83725-1555  
United States

{{ site.email }}  

<div style="clear:both"></div>

# Recent activity

{% for post in site.posts limit: 6 %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' | strip }}  
<span class="post-meta">
{%- for category in post.categories -%}
<span class="category_name">{{category | split: "-" | join: " "}}</span>
{%- endfor %}
posted on {{ post.date | date: "%b %-d, %Y" }}
</span>

{% endfor %}

**subscribe** via [rss]({{ site.baseurl }}/feed.xml)

# Links

[Boise State set theory research](https://www.boisestate.edu/math/research/settheory/) in the BSU math department  
[Boise extravaganza in set theory](https://www.boisestate.edu/math/best/) conference web site  
[Pure math academy](https://www.puremathacademy.com/) boutique math courses for all  
[Set theory talks](http://settheory.mathtalks.org/) worldwide set theory announcements  
[Mathblogging.org](https://mathblogging.org/) curated collection of math blogs
