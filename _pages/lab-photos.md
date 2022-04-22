---
title: "NDS Lab - Pictures"
layout: piclay
excerpt: "NDS Lab -- Pictures"
permalink: /lab-photos/
---

# NDS Lab Photos

## NDS Lab and friends end of Summer 2021 BBQ

<!-- 
#### Example youtube video:
<iframe width="560" height="315" src="https://www.youtube.com/embed/idhere......" frameborder="0" allowfullscreen></iframe>
-->

<!-- Gallery -->
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_NDS %}

{% assign even_odd = number_printed | modulo: 1 %} 

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/photos/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>
{{ pic.title }}
  
{% assign number_printed = number_printed | plus: 1 %}
  
</div>

{% endfor %}


<p> &nbsp; </p>

