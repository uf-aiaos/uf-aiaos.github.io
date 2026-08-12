---
title: "News"
layout: textlay
excerpt: "Animal Artificial Intelligence Lab at UF."
sitemap: false
permalink: /news.html
---

# News

<div class="news-archive" markdown="0">
{% assign current_year = "" %}
{% for article in site.data.news %}
{% assign article_year = article.date | strip_html | slice: -4, 4 %}

{% if article_year != current_year %}
{% unless forloop.first %}
</div>
</section>
{% endunless %}

<section class="news-year">
<button class="news-year-toggle{% unless forloop.first %} collapsed{% endunless %}"
        type="button" data-toggle="collapse"
        data-target="#news-{{ article_year }}"
        aria-expanded="{% if forloop.first %}true{% else %}false{% endif %}"
        aria-controls="news-{{ article_year }}">
  <span>{{ article_year }}</span>
  <span class="news-year-icon" aria-hidden="true"></span>
</button>
<div id="news-{{ article_year }}"
     class="collapse news-year-content{% if forloop.first %} in{% endif %}">

{% assign current_year = article_year %}
{% endif %}

<article class="news-archive-item">
  <div class="news-archive-date">{{ article.date }}</div>
  <span class="news-badge news-badge--{{ article.category }}">{{ article.category }}</span>
  <div class="news-archive-headline">{{ article.summary | default: article.headline }}</div>
</article>

{% if forloop.last %}
</div>
</section>
{% endif %}
{% endfor %}
</div>
