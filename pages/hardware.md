---
layout: page
show_meta: false
title: "HARDWARE LAYOUTS"
subheadline: "Hardware Design Plan"
header:
   image_fullwidth: "Interconnect_pcb.jpeg"
permalink: "/hardware/"
---
<ul>
    {% for post in site.categories.hardware %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>