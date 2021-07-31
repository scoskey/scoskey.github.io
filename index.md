---
layout: page
---

<img style="float:right;margin-left:10px" src="{{ site.baseurl }}/assets/dogsquaresmall.png" alt="dog icon" />

Department of Mathematics  
Boise State University  
1910 University Dr  
Boise, ID 83725-1555  

{{ site.email }}  
Office MB 238-B


<div style="clear:both"></div>

# Recent activity

{% for post in site.posts limit: 6 %}

[{{ post.title }}]({% if post.siteurl %}{{ post.siteurl }}{% else %}{{ post.url }}{% endif %})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' | strip }}  
<span class="post-meta"><span class="category_name">{{ post.categories }}</span> posted on {{ post.date | date: "%b %-d, %Y" }}</span>

{% endfor %}

**subscribe** via [rss]({{ site.baseurl }}/feed.xml)

# Links

[Boise State set theory research](https://www.boisestate.edu/math/research/settheory/) in the BSU math department  
[Boise extravaganza in set theory](https://www.boisestate.edu/math/best/) conference web site  
[Boise math circles](https://www.boisestate.edu/math/circles/) math for secondary students  
[Pure math academy](https://www.puremathacademy.com/) boutique math courses for all  
[Set theory talks](http://settheory.mathtalks.org/) worldwide set theory announcements  
[Mathblogging.org](https://mathblogging.org/) curated collection of math blogs
