---
title: "About"
layout: gridlay
sitemap: false
permalink: /about/
---

## About 

{% for member in site.data.pi %}
<div class="jumbotron">
<div class="row">
<div class="col-sm-4">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-8">
  <h3>{{ member.name }}</h3>
  <h4><i>{{ member.info }}</i></h4>
  {% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-3x"></i></a> {% endif %}
  {% if member.cv %} <a href="{{ member.cv }}" target="_blank"><i class="ai ai-cv-square ai-3x"></i></a> {% endif %}
  {% if member.scholar %} <a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square ai-3x"></i></a> {% endif %}
  {% if member.github %} <a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-3x"></i></a> {% endif %}
  {% if member.researchgate %} <a href="{{ member.researchgate }}" target="_blank"><i class="ai ai-researchgate-square ai-3x"></i></a> {% endif %}
</div>
</div>
</div>
<div class="row">
<div class="col-sm-6 col-xs-12">
## Education
<div class="jumbotron">
  <ul style="overflow: hidden">
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education2 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education3 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education3 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education4 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education3 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education4 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education5 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_educ == 6 %}
  <li> {{ member.education1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education3 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education4 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education5 | replace: "-","&#8211;"}} </li>
  <li> {{ member.education6 | replace: "-","&#8211;"}} </li>
  {% endif %}
  </ul>
</div>
</div>

<div class="col-sm-6 col-xs-12">
## Experience
<div class="jumbotron">
  <ul style="overflow: hidden">
  {% if member.number_expe == 1 %}
  <li> {{ member.experience1 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_expe == 2 %}
  <li> {{ member.experience1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience2 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_expe == 3 %}
  <li> {{ member.experience1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience3 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_expe == 4 %}
  <li> {{ member.experience1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience3 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience4 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_expe == 5 %}
  <li> {{ member.experience1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience3 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience4 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience5 | replace: "-","&#8211;"}} </li>
  {% endif %}
  {% if member.number_expe == 6 %}
  <li> {{ member.experience1 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience2 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience3 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience4 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience5 | replace: "-","&#8211;"}} </li>
  <li> {{ member.experience6 | replace: "-","&#8211;"}} </li>
  {% endif %}
  </ul>
</div>
</div>
</div>

{% endfor %}


<!-- 
{% if site.data.grants %}
<div class="jumbotron">
### Grants
<ul>
{% for grant in site.data.grants %}
 <li> {{ grant.name }} </li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.awards %}
<div class="jumbotron">
### Awards
<ul>
{% for award in site.data.awards %}
 <li> {{ award.name | replace: "-","&#8211;"}} </li>
{% endfor %}
</ul>
</div>
{% endif %}


{% if site.data.people %}
<div class="jumbotron">
### Students and mentoring
<ul>
{% for student in site.data.people %}
 <li> {{ student.name }}, {{student.location}} ({{student.degree}}, {{student.year}}) </li>
{% endfor %}
</ul>
</div>
{% endif %}


{% if site.data.collaborators %}
<div class="jumbotron">
### Collaborators
<ul>
{% for collab in site.data.collaborators %}
 <li> <a href="{{collab.url}}" target="_blank">{{collab.name}}</a> ({{collab.title}})</li>
{% endfor %}
</ul>
</div>
{% endif %}


<div class="jumbotron">
  <h4>Sponsors</h4>
  <div style='display:block; text-align:center; margin-left:auto; margin-right:auto;'>
 {% for funder in site.data.funders %}<a href="{{ funder.url }}" target="_blank"><img src='{{ site.url }}{{ site.baseurl }}/images/logopic/{{ funder.image }}' style='max-height: 80px; max-width: 200px; margin: 1%'/></a>{% endfor %}
  </div>
</div> -->
