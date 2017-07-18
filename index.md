---
layout: page
---

<img style="float:right;margin-left:10px" src="{{ site.baseurl }}/assets/dogsquaresmall.jpg" alt="dog icon" />

Department of Mathematics  
Boise State University  
1910 University Dr  
Boise, ID 83725-1555  

Room 237-A  
scoskey@nylogic.org

<div style="clear:both"></div>

# Recent activity

{% for post in site.posts limit: 6 %}

[{{ post.title }}]({{ post.url }})  
{{ post.excerpt | remove: '<p>' | remove: '</p>' | strip }}  
<span class="post-meta"><span class="category_name">{{ post.categories }}</span> posted on {{ post.date | date: "%b %-d, %Y" }}</span>

{% endfor %}

**subscribe** via [rss]({{ site.baseurl }}/feed.xml)

# Links

[Boise State University set theory research](https://math.boisestate.edu/research/settheory)  
[Set theory talks, worldwide set theory announcements](http://settheory.mathtalks.org)
[Mathblogging, curated collection of math blogs](https://mathblogging.org)