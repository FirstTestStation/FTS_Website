---
layout: page
show_meta: false
title: "Technical content!"
subheadline: "Project Layouts"
header:
   image_fullwidth: "pcb.jpg"
permalink: "/design/"
---
<ul>
    {% for post in site.categories.design %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>