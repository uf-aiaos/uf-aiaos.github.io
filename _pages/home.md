---
title: "AIAOS Lab - Home"
layout: homelay
excerpt: "Artificial Intelligence in Animal Omics Sciences."
sitemap: false
permalink: /
---


Welcome to the Artificial Intelligence in Animal Omics Sciences (AIAOS) Lab in the [Department of Animal Sciences](https://animal.ifas.ufl.edu/){:target="_blank"} at the [University of Florida](https://www.ufl.edu/){:target="_blank"}.

Our overall research focuses on using artificial intelligence and statistical modeling to integrate high-dimensional, heterogeneous omics data to advance animal agriculture. Our first research area focuses on developing artificial intelligence models and open-source software tools to capture and extract digital phenotypes of animals to support data-driven decisions that improve animal health, production, welfare, and other management practices in livestock farming systems. Our second research area centers on developing artificial intelligence and statistical models to integrate these digital phenotypes with genomic and other omics data to enhance the genetic improvement of animals.

<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="8000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li> 
    </ol>
    
    <div class="carousel-inner" markdown="0">

        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/carousel/team2024.webp" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/labpics/rfernando-visit.webp" alt="Slide 2" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/carousel/uf-ans.webp" alt="Slide 3" />
        </div>
    </div>
    
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

<section class="lab-highlights" aria-labelledby="lab-highlights-title" markdown="0">
  <div class="lab-highlights-heading">
    <h2 id="lab-highlights-title">Lab highlights</h2>
  </div>
  <div class="lab-highlights-timeline">
    {% assign highlight_categories = "funding,milestone,award" | split: "," %}
    {% for highlight_category in highlight_categories %}
    {% assign category_items = site.data.news | where: "category", highlight_category %}
    {% assign highlighted_category_items = category_items | where: "highlight", true %}
    {% if highlighted_category_items.size > 0 %}
    <article class="lab-highlight-item lab-highlight-item--{{ highlight_category }}">
      <div class="lab-highlight-marker" aria-hidden="true"></div>
      <div class="lab-highlight-content">
        <div class="lab-highlight-meta">
          <span class="news-badge news-badge--{{ highlight_category }}">{{ highlight_category }}</span>
        </div>
        {% for item in highlighted_category_items %}
        <div class="lab-highlight-entry">
          <span class="lab-highlight-date">{{ item.date }}</span>
        <h3><a href="{{ item.highlight_url | default: '/news.html' }}"{% if item.highlight_url contains 'http' %} target="_blank" rel="noopener noreferrer"{% endif %}>{% if item.highlight_title %}{{ item.highlight_title }}{% else %}{{ item.category | capitalize }} update{% endif %}</a></h3>
        <p>{{ item.highlight_text | default: item.summary }}</p>
        </div>
        {% endfor %}
      </div>
    </article>
    {% endif %}
    {% endfor %}
  </div>
</section>

<!--
We are grateful for funding from the [Institute of Food and Agricultural Sciences (IFAS)](https://ifas.ufl.edu/), [Department of Animal Sciences](https://animal.ifas.ufl.edu/) at the [University of Florida](https://www.ufl.edu/).
-->
<!--
<figure class="fourth">
  
  <img src="{{ site.url }}{{ site.baseurl }}/images/uf-logo/as.png" style="width: 180px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/uf-logo/uf-ifas.jpg" style="width: 180px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/uf-logo/uf.png" style="width: 210px">
</figure>
-->
