---
layout: page
show_meta: false
title: "Technical Information!"
subheadline: "Test Software Design"
header:
   image_fullwidth: "Interconnect_pcb.jpeg"
permalink: "/software/"
---
<ul>
    {% for post in site.categories.software %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>