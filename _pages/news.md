---
title: "News"
layout: textlay
excerpt: "Animal Artificial Intelligence Lab at UF."
sitemap: false
permalink: /news.html
---

# News

<!--
{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
-->

{% for article in site.data.news %}

{% if article.headline == "YEAR" %}
  <h3><b>{{ article.date }}</b></h3>
{% else %}
  {{ article.date }}<br>
  <div style="margin-left: 6px">
  <em>{{ article.headline }}</em><br style="line-height: 20px" />
  </div>
{% endif %}

{% endfor %}
