---
title: "AAI Lab - Team"
layout: gridlay
excerpt: "AAI Lab: Team"
sitemap: false
permalink: /team/
---

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
  <i>{{ member.info }} <br>email: <{{ member.email }}><br>CV: <{{ member.CV }}></i>
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



## Graduate Students
{% assign number_printed = 0 %}
{% for member in site.data.grad %} 

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>

  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 0 %}
  {% endif %}

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
<br>




<!--

## Affiliated PhD Mentees
{% assign number_printed = 0 %}
{% for member in site.data.affiliated %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>

  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 0 %}
  {% endif %}

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
  {% if member.website != 0 %} <a href="{{ member.website }}"> <i class="fa fa-link"></i></a> {% endif %} {% if member.linkedin != 0 %} <a href="{{ member.linkedin }}"> <i class="fa fa-linkedin"></i></a> {% endif %} {% if member.github != 0 %} <a href="{{ member.github }}"> <i class="fa fa-github"></i></a> {% endif %} {% if member.twitter != 0 %} <a href="{{ member.twitter }}"> <i class="fa fa-twitter"></i></a> {% endif %} 
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
<br>











## Masters
{% assign number_printed = 0 %}
{% for member in site.data.ms %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
  
<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}  <br>email: <{{ member.email }}></i> 
  <ul style="overflow: hidden">
  {% if member.number_educ == 0 %}
  {% endif %}
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
  </ul>
    
  <div class="social-links"> 
  {% if member.linkedin != 0 %} <a href="{{ member.linkedin }}"> <i class="fa fa-linkedin"></i></a> {% endif %} {% if member.github != 0 %} <a href="{{ member.github }}"> <i class="fa fa-github"></i></a> {% endif %}
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
<br>











## Undergraduates
{% assign number_printed = 0 %}
{% for member in site.data.bs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}


<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i> 
  <ul style="overflow: hidden">

  {% if member.number_educ == 0 %}
  {% endif %}

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
  {% if member.linkedin != 0 %} <a href="{{ member.linkedin }}"> <i class="fa fa-linkedin"></i></a> {% endif %} {% if member.github != 0 %} <a href="{{ member.github }}"> <i class="fa fa-github"></i></a> {% endif %}
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
<br>






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
  <i>{{ member.info }} email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 0 %}
  {% endif %}

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
  {% if member.linkedin != 0 %} <a href="{{ member.linkedin }}"> <i class="fa fa-linkedin"></i></a> {% endif %} {% if member.github != 0 %} <a href="{{ member.github }}"> <i class="fa fa-github"></i></a> {% endif %}
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
<br>


-->



<!--
## Former Interns
{% assign number_printed = 0 %}
{% for member in site.data.former_intern %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i> 
  <ul style="overflow: hidden">

  {% if member.number_educ == 0 %}
  {% endif %}

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
  {% if member.linkedin != 0 %} <a href="{{ member.linkedin }}"> <i class="fa fa-linkedin"></i></a> {% endif %} {% if member.github != 0 %} <a href="{{ member.github }}"> <i class="fa fa-github"></i></a> {% endif %}
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


-->




<!--
## Master and Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}  <br>email: <{{ member.email }}></i> 
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
  </ul>
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
-->

<!--
## Alumni
{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/members/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Role: {{ member.info }}</i>
  <ul style="overflow: hidden">
  </ul>
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
-->


<!--
## Former visitors, BSc/ MSc students
<div class="row">
<div class="col-sm-4 clearfix">
<h4>Visitors</h4>
{% for member in site.data.alumni_visitors %}
{{ member.name }}
{% endfor %}
</div>
<div class="col-sm-4 clearfix">
<h4>Master students</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}
{% endfor %}
</div>
<div class="col-sm-4 clearfix">
<h4>Bachelor Students</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}
{% endfor %}
</div>
</div>
-->
