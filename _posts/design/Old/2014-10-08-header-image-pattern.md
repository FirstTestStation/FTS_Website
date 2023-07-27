---
layout: page
title:  "First TestStation Projects"
subheadline:  "Block Diagram"
teaser: "First TestStation plans to provide, free of charge, a starting test solution for testing electronic production boards or electronic systems."
categories:
    - design
tags:
    - design
    - pattern
    - header
header:
    image: FirstTestStation.png
    pattern: pattern_concrete.jpg
    caption: This is the block diagram of the First test Station
    caption_url: https://unsplash.com/
---
It's so easy to do. Just define in front matter an image and a pattern image. Instead of a pattern you can also use a color. Have a look at the [example with a background color]({{ site.url }}{{ site.baseurl }}/design/header-image-color/).
<!--more-->

## Front Matter Code

~~~
header:
    image:  "header_unsplash_2-970x.jpg"
    pattern:  "pattern_concrete.jpg"
    caption: This is a caption for the header image with link
    caption_url: https://unsplash.com/
~~~



### All Header-Styles 
{: .t60 }

{% include list-posts tag='header' %}