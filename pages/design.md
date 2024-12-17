---
layout: page
show_meta: false
title: "DESIGN LAYOUTS"
subheadline: "Design Project Plan"
header:
   image_fullwidth: "Interconnect_pcb.jpeg"
permalink: "/design/"
---
<ul>
    {% for post in site.categories.design %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>