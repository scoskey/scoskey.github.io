---
layout: page
---

# Contact

<img style="float:right;margin-left:10px" src="{{ site.baseurl }}/assets/dogsquaresmall.png" alt="dog icon" />

Department of Mathematics  
University College London  
25 Gordon St  
London WC1H 0AY  
United Kingdom

[{{ site.email }}](mailto:{{ site.email }})

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

[[rss]({{ site.baseurl }}/feed.xml)]

# Links

[UCL mathematics](https://ucl.ac.uk/maths/) department home page  
[Boise mathematics](https://boisestate.edu/math/) department home page  
[Set theory in the United Kingdom](https://www.dpmms.cam.ac.uk/~dbl25/STUK/) meetings network  
[Set theory talks](https://settheory.mathtalks.org/) worldwide set theory announcements  
[Booles’ Rings](https://boolesrings.org/) collated set theory blogs  
[Mathblogging](https://mathblogging.org/) collated math blogs
