---
layout: page
---

<img style="float:right;margin-left:10px" src="{{ site.baseurl }}/assets/dogsquaresmall.png" alt="dog icon" />

Department of Mathematics  
Boise State University  
1910 University Dr  
Boise, ID 83725-1555  

Room 238-B  
{{ site.email }}

<div style="clear:both"></div>

# Recent activity

{% for post in site.posts limit: 6 %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' | strip }}  
<span class="post-meta"><span class="category_name">{{ post.categories }}</span> posted on {{ post.date | date: "%b %-d, %Y" }}</span>

{% endfor %}

**subscribe** via [rss]({{ site.baseurl }}/feed.xml)

# Links

[Set theory research](https://math.boisestate.edu/research/settheory) in the BSU math department  
[Set theory talks](http://settheory.mathtalks.org) worldwide set theory announcements  
[Mathblogging.org](https://mathblogging.org) curated collection of math blogs  
[Boise math circles](http://boisemathcircles.org) math for secondary students