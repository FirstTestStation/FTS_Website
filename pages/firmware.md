---
layout: page
show_meta: false
title: "Technical Information!"
subheadline: "Embedded Firmware Design"
header:
   image_fullwidth: "Interconnect_pcb.jpeg"
permalink: "/firmware/"
---
<ul>
    {% for post in site.categories.firmware %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>