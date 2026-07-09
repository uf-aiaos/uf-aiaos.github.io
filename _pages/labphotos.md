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

## 2026

#### The AIAOS Lab gathered to celebrate several exciting milestones! Blue Gill Quality Food, Gainesville. July 1. 
* Jin's PhD graduation.
* Fiona's successful Master's thesis defense.
* Angelo's First Place award in the Production Division PhD Poster Competition at the ADSA 2026 Annual Meeting.
* Zhou's completion of his postdoctoral training.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/grpsummer26.jpg" loading="lazy" width="70%"> 
</figure>

#### Yuxi (Fiona) successfully defended her Master's thesis. Congratulations! Department of Animal Sciences, University of Florida. June 29. 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/fionamsgrad.jpeg" loading="lazy" width="80%"> 
</figure>

#### The AIAOS Lab had a successful week at the ADSA 2026 Annual Meeting in Milwaukee, WI, June 21–24. 
* Dr. Yu presented an invited symposium talk and one oral presentation. 
* Our PhD student, Angelo, delivered one oral presentation and was awarded First Place in the Production Division PhD Poster Competition. Congratulations, Angelo!
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/adsa26.png" loading="lazy" width="80%"> 
</figure>

#### Congrats Jin on finishing her PhD! Department of Animal Sciences, University of Florida. May 15.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/jingraduation.png" loading="lazy" width="80%"> 
</figure>

#### Yu's lab attended and presented at the 2026 UF IFAS AI Summit. Emerson Alumni Hall, University of Florida. February 12.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ifas-ai-summit26.png" loading="lazy" width="70%"> 
</figure>

## 2025
#### Yu's lab attended the 11th UF/IFAS Animal Sciences Graduate Symposium held at the Austin Cary Forest Campus. 
* Jin, Yuxi, and Angelo presented their projects at the symposium – October 8.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ans-symposium-25.png" loading="lazy" width="70%"> 
</figure>

#### Dr. Rohan Fernando visited our lab and had a group discussion with our team – September 29. 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/rfernando-visit.png" loading="lazy" width="70%"> 
</figure>

#### Dr. Rodrigo Mezencio Godinho from Topigs Norsvin visited our lab – July 14.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/rodrigo-visit.png" loading="lazy" width="70%"> 
</figure>

#### Dr. Yu presented the research project led by Jin at the 2025 American Society of Animal Science (ASAS) meeting – July 9.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/asas2025.jpg" loading="lazy" width="70%"> 
</figure>

#### Yu's lab attended the 2025 US Precision Livestock Farming Conference – June. 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/plf2025.jpg" loading="lazy" width="60%"> 
</figure>

#### Dr. Dekkers gave a seminar in the ANS Department and had a group discussion with Yu's lab – April 3.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/dekkers-visit.jpg" loading="lazy" width="60%"> 
</figure>


## 2024
* End of year lab celebration. 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/endofyear24.jpg" loading="lazy" width="60%"> 
</figure>

#### Yu's lab attended the 10th UF/IFAS Animal Sciences Graduate Symposium in St. Augustine, FL. Jin and Angelo presented their projects at the symposium.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ans-symposium-24.jpg" loading="lazy" width="60%"> 
</figure>


#### Lab lunch at Ford's Garage Gainesville (Left to right: Yuecheng, Jin, Yuxi, Lucas, Angelo, and Haipeng)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/lablunch24.jpg" loading="lazy" width="60%"> 
</figure>

## 2023
* UF/IFAS Animal Sciences Christmas Party. Gainesville, FL. December 14. (Left to right: Alberta, Jin Wang, Yuechen Guo, Haipeng Yu, and Albert)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ANSChristmas23.jpg" loading="lazy" width="60%"> 
</figure>

#### UF/IFAS Animal Sciences 9th Graduate Symposium. St. Augustine, FL. October 12-13. (Jin Wang)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ANS-symposium23.jpg" loading="lazy" width="50%"> 
</figure>

#### Jin Wang and Yu Hu started the first image data collection experiment using our developed automatic image acquisition pipeline at the University of Florida Dairy Unit.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/DairyCollection.jpg" loading="lazy" width="50%"> 
</figure>

#### Future of Food Forum - Transforming Food Systems with Artificial Intelligence. Gainesville, FL. March 20. (Jin Wang)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/FFF23JIN.jpg" loading="lazy" width="50%"> 
</figure>

## 2022

#### UF/IFAS Animal Sciences 8th Graduate Symposium. St. Augustine, FL. October 6-7. (Left to right: Jin Wang, Haipeng Yu, Yue Li)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/labpics/ANSgradsymposium.jpeg" loading="lazy" width="50%"> 
</figure>


