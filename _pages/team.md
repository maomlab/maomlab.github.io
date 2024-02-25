---
title: "Maom Lab - Team"
layout: gridlay
excerpt: "Maom Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

## Members
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
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

## Rotation Trainees
{% assign number_printed = 0 %}
{% for member in site.data.rotation_trainees %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <ul style="overflow: hidden">

  {% if member.number_trainee == 1 %}
  <li> {{ member.trainee1 }} </li>
  {% endif %}

  {% if member.number_trainee == 2 %}
  <li> {{ member.trainee1 }} </li>
  <li> {{ member.trainee2 }} </li>
  {% endif %}

  {% if member.number_trainee == 3 %}
  <li> {{ member.trainee1 }} </li>
  <li> {{ member.trainee2 }} </li>
  <li> {{ member.trainee3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.trainee1 }} </li>
  <li> {{ member.trainee2 }} </li>
  <li> {{ member.trainee3 }} </li>
  <li> {{ member.trainee4 }} </li>
  {% endif %}

  {% if member.number_trainee == 5 %}
  <li> {{ member.trainee1 }} </li>
  <li> {{ member.trainee2 }} </li>
  <li> {{ member.trainee3 }} </li>
  <li> {{ member.trainee4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  {% if member.number_trainee == 6 %}
  <li> {{ member.trainee1 }} </li>
  <li> {{ member.trainee2 }} </li>
  <li> {{ member.trainee3 }} </li>
  <li> {{ member.trainee4 }} </li>
  <li> {{ member.trainee5 }} </li>
  <li> {{ member.trainee6 }} </li>
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



## Alumni
{% assign number_printed = 0 %}
{% for member in site.data.team_alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
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

  {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
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


## Collaborators
{% assign number_printed = 0 %}
{% for lab in site.data.team_collaborators %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ lab.name }}</h4>
  {{ lab.research }}<br/>
  <i>{{ lab.affiliation }}</i>
  <ul style="overflow: hidden">

 {% if lab.number_member == 1 %}
  <li> {{ lab.member1 }} </li>
  {% endif %}

  {% if lab.number_member == 2 %}
  <li> {{ lab.member1 }} </li>
  <li> {{ lab.member2 }} </li>
  {% endif %}

  {% if lab.number_member == 3 %}
  <li> {{ lab.member1 }} </li>
  <li> {{ lab.member2 }} </li>
  <li> {{ lab.member3 }} </li>
  {% endif %}

  {% if lab.number_member == 4 %}
  <li> {{ lab.member1 }} </li>
  <li> {{ lab.member2 }} </li>
  <li> {{ lab.member3 }} </li>
  <li> {{ lab.member4 }} </li>
  {% endif %}

  {% if lab.number_member == 5 %}
  <li> {{ lab.member1 }} </li>
  <li> {{ lab.member2 }} </li>
  <li> {{ lab.member3 }} </li>
  <li> {{ lab.member4 }} </li>
  <li> {{ lab.member5 }} </li>
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


