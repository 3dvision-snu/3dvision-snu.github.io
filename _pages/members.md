---
title: "3D Vision lab - Members"
layout: gridlay
excerpt: "3D Vision lab: Team members"
sitemap: false
permalink: /members/
---

 <!-- **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!** -->


<!-- Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors). -->
## Professor
{% assign number_printed = 0 %}
{% for member in site.data.members_professor %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-8 clearfix">
  {% if member.page == nil %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% else %}
  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>
  {% endif %}
  <h4>{{ member.name }}</h4>
  <i>
    <strong> {{ member.info }}<br></strong>
    <strong>Email: </strong><{{ member.email }}>
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
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

## Ph.D Students
{% assign number_printed = 0 %}
{% for member in site.data.members_phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.page == nil %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% else %}
  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>
  {% endif %}
  <h4>{{ member.name }}</h4>
  
  <i>
    <strong> Email: </strong> <{{ member.email }}> <br>
    <strong> Research interests: </strong> {{member.research_interests}}
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
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


## M.S Students
{% assign number_printed = 0 %}
{% for member in site.data.members_ms %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.page == nil %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% else %}
  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>
  {% endif %}
  <h4>{{ member.name }}</h4>
  
  <i>
    <strong> Email: </strong> <{{ member.email }}> <br>
    <strong> Research interests: </strong> {{member.research_interests}}
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
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


## B.S Students
{% assign number_printed = 0 %}
{% for member in site.data.members_bs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.page == nil %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% else %}
  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>
  {% endif %}
  <h4>{{ member.name }}</h4>
  <i>
    <strong> Email: </strong> <{{ member.email }}> <br>
    <strong> Research interests: </strong> {{member.research_interests}}
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
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
{% for member in site.data.members_alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.page == nil %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% else %}
  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>
  {% endif %}
  <h4>{{ member.name }}</h4>
  <i>
    <strong> Email: </strong> <{{ member.email }}>
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
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


<!-- <div class="col-sm-4 clearfix">
<h4>Bachelor Students</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}
{% endfor %}
</div>

</div> -->

<!-- 
## Administrative Support
<a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van Rijsewijk</a> is helping us (and other groups) with administration. -->
