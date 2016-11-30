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
<span class="post-meta"><span style="color:green">{{ post.categories }}</span> posted on {{ post.date | date: "%b %-d, %Y" }}</span>

{% endfor %}

**subscribe** via [rss]({{ site.baseurl }}/feed.xml)
