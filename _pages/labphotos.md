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

# 2025
* Dr. Rodrigo Mezencio Godinho from Topigs Norsvin visited our lab.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/rodrigo-visit.png" width="70%"> 
</figure>

* Dr. Yu presented the research project led by Jin at the 2025 American Society of Animal Science (ASAS) meeting.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/asas2025.jpg" width="70%"> 
</figure>

* Yu's lab attended the 2025 US Precision Livestock Farming Conference. 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/plf2025.jpg" width="60%"> 
</figure>

* Dr. Dekkers gave a seminar in the ANS Department and had a group discussion with Yu's lab.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/dekkers-visit.jpg" width="60%"> 
</figure>


# 2024
* End of year lab celebration. 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/endofyear24.jpg" width="60%"> 
</figure>

* Yu's lab attended the 10th UF/IFAS Animal Sciences Graduate Symposium in St. Augustine, FL. Jin and Angelo presented their projects at the symposium.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ans-symposium-24.jpg" width="60%"> 
</figure>


* Lab lunch at Ford's Garage Gainesville (Left to right: Yuecheng, Jin, Yuxi, Lucas, Angelo, and Haipeng)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/lablunch24.jpg" width="60%"> 
</figure>

# 2023
* UF/IFAS Animal Sciences Christmas Party. Gainesville, FL. December 14. (Left to right: Alberta, Jin Wang, Yuechen Guo, Haipeng Yu, and Albert)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ANSChristmas23.jpg" width="60%"> 
</figure>

* UF/IFAS Animal Sciences 9th Graduate Symposium. St. Augustine, FL. October 12-13. (Jin Wang)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ANS-symposium23.jpg" width="50%"> 
</figure>

* Jin Wang and Yu Hu started the first image data collection experiment using our developed automatic image acquisition pipeline at the University of Florida Dairy Unit.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/DairyCollection.jpg" width="50%"> 
</figure>

* Future of Food Forum - Transforming Food Systems with Artificial Intelligence. Gainesville, FL. March 20. (Jin Wang)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/FFF23JIN.jpg" width="50%"> 
</figure>

# 2022
* UF/IFAS Animal Sciences 8th Graduate Symposium. St. Augustine, FL. October 6-7. (Left to right: Jin Wang, Haipeng Yu, Yue Li)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ANSgradsymposium.jpeg" width="50%"> 
</figure>


