---
layout: post
title:  "Mountains Gallery"
date:   2020-10-15
categories: [landscape]
thumbnail: mountains3.png
---

{% assign filenames = "mountains1.png,mountains2.png,mountains3.png,mountains4.png,mountains5.png,mountains6.png" | split: "," %}
<div class ="image-gallery">
{% for name in filenames %}
    <div class="box">
    <a href="{{ site.imagesurl }}{{ name }}">
      <img src="{{ site.thumbsurl }}{{ name }} " alt="{{ name }}"  class="img-gallery" /> 
     </a> 
    </div>
 {% endfor %}
</div>
