---
title: "AIAOS Lab - Photos"
layout: piclay
excerpt: "LabPhotos"
permalink: /labphotos/
---

# Pictures

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}


{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

# 2022
UF/IFAS Animal Sciences 8th Graduate Symposium. St. Augustine, FL. October 6-7. (Left to right: Jin Wang, Haipeng Yu, Yue Li)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ANSgradsymposium.jpeg" width="80%"> 
</figure>


<!--
2020 VT Science Festival - September 29, October 1, October 6 
<a href="https://icat.vt.edu/science-festival/exhibitors/do-you-know-what-i-m-looking-at--tracking-eye-movements-during-m.html">Do you know what I'm looking at? Tracking eye movements during math games </a>
(Koeun Choi, Caroline Hornburg, Ally Copeland, Taylor Covington, Bethany Grocock, Jisun Kim, Ava Bir, Caroline Kammer, Molly Simek, Brianna Whitmore, Breanne De Vera, Shawnice Johnson, Anvitha Metpally, Katie Johnson, Eman Ayaz, Michelle Tran)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpic/VTSciFest_2020_0929.png" width="70%">
</figure>
-->
