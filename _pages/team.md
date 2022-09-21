---
title: "AIAOS Lab - Team"
layout: gridlay
excerpt: "Team"
sitemap: false
permalink: /team/
---
<!--
When adding new section (e.g., gradaute student), copy the interns.yml file and copy the interns section below. 
-->

## Principal Investigator
{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>
	  email: <{{ member.email }}><br>
	  CV: <a href="{{ member.CV }}" target="_blank">yu_cv.pdf</a> </i>
	  
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
  
  <div class="social-links"> 
  {% if member.website != 0 %} <a href="{{ member.website }}" target="_blank"> <i class="fa fa-link"></i></a> {% endif %} {% if member.scholar != 0 %} <a href="{{ member.scholar }}" target="_blank"> <i class="ai ai-google-scholar ai-lg"></i></a> {% endif %} {% if member.linkedin != 0 %} <a href="{{ member.linkedin }}" target="_blank"> <i class="fa fa-linkedin"></i></a> {% endif %} {% if member.github != 0 %} <a href="{{ member.github }}" target="_blank"> <i class="fa fa-github"></i></a> {% endif %} {% if member.twitter != 0 %} <a href="{{ member.twitter }}" target="_blank"> <i class="fa fa-twitter"></i></a> {% endif %} {% if member.publons != 0 %} <a href="{{ member.publons }}" target="_blank"> <i class="ai ai-publons ai-lg"></i></a> {% endif %} {% if member.orcid != 0 %} <a href="{{ member.orcid }}" target="_blank"> <i class="ai ai-orcid ai-lg"></i></a> {% endif %} 
</div>
  
  
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
<br>




## Lab members

- <span style="color:blue"> **We are looking for PhD students and Postdocs to join our team in Spring/Fall 2023. See details in the <a href="../openings">Openings</a> section.** </span>


## Interns

{% assign number_printed = 0 %}
{% for member in site.data.interns %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} </i>
	  
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
  <!-- KEY NOTES: THE FIRST ACADEMIC ICON MUST BE FILLED, OTHERWISE IT WILL CAUSE TROUBLE-->
  <div class="social-links"> 
  {% if member.github != 0 %} <a href="{{ member.github }}" target="_blank"> <i class="fa fa-github"></i></a> {% endif %} 
  {% if member.linkedin != 0 %} <a href="{{ member.linkedin }}" target="_blank"> <i class="fa fa-linkedin"></i></a> {% endif %} {% if member.website != 0 %} <a href="{{ member.website }}" target="_blank"> <i class="fa fa-link"></i></a> {% endif %} {% if member.scholar != 0 %} <a href="{{ member.scholar }}" target="_blank"> <i class="ai ai-google-scholar ai-lg"></i></a> {% endif %} {% if member.twitter != 0 %} <a href="{{ member.twitter }}" target="_blank"> <i class="fa fa-twitter"></i></a> {% endif %} {% if member.publons != 0 %} <a href="{{ member.publons }}" target="_blank"> <i class="ai ai-publons ai-lg"></i></a> {% endif %} {% if member.orcid != 0 %} <a href="{{ member.orcid }}" target="_blank"> <i class="ai ai-orcid ai-lg"></i></a> {% endif %} 
</div>
  
  
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
<br>
