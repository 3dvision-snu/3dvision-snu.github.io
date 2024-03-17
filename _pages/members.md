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
  <div style="display: flow-root;">
  <i>
    <strong> {{ member.info }}<br></strong>
    <!-- <a href="{{member.email_link}}" onclick="popup=window.open({{member.email_link}},'mailhidepopup','width=580,height=635'); return false;"> <strong> Email </strong> </a> <br> -->
    <strong> Email : </strong>
    <a href = "mailto: {{member.email}}"> {{member.email}} </a>
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
  </ul>
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
## Ph.D Students
{% assign number_printed = 0 %}
{% for member in site.data.members_phd %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
[comment]: <> (  {% if member.page == nil %})
[comment]: <> (  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />)
[comment]: <> (  {% else %})
[comment]: <> (  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>)
[comment]: <> (  {% endif %})
[comment]: <> (  <h4>{{ member.name }}</h4>)
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.page == nil %}
  <h4>{{ member.name }}</h4>
  {% else %}
  <h4> <a href="{{member.page}}"> {{ member.name }} </a> </h4>
  {% endif %}
  <div style="display: flow-root;">
  <i>
    <!-- <a href="{{member.email_link}}" onclick="popup=window.open({{member.email_link}},'mailhidepopup','width=580,height=635'); return false;"> <strong> Email </strong> </a> <br> -->
    <strong> Email : </strong>
    <a href = "mailto: {{member.email}}"> {{member.email}} </a><br>
    <strong> Research Interests: </strong> {{member.research_interests}}<br>
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
  </ul>
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
## M.S Students
{% assign number_printed = 0 %}
{% for member in site.data.members_ms %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
[comment]: <> (  {% if member.page == nil %})
[comment]: <> (  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />)
[comment]: <> (  {% else %})
[comment]: <> (  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>)
[comment]: <> (  {% endif %})
[comment]: <> (  <h4>{{ member.name }}</h4>)
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.page == nil %}
  <h4>{{ member.name }}</h4>
  {% else %}
  <h4> <a href="{{member.page}}"> {{ member.name }} </a> </h4>
  {% endif %}
  <div style="display: flow-root;">
  <i>
    <!--<a href="{{member.email_link}}" onclick="popup=window.open({{member.email_link}},'mailhidepopup','width=580,height=635'); return false;"> <strong> Email </strong> </a> <br>-->
    <strong> Email : </strong>
    <a href = "mailto: {{member.email}}"> {{member.email}} </a><br>
    <strong> Research Interests: </strong> {{member.research_interests}}
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
  </ul>
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

## Researchers
{% assign number_printed = 0 %}
{% for member in site.data.members_researcher %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
[comment]: <> (  {% if member.page == nil %})
[comment]: <> (  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />)
[comment]: <> (  {% else %})
[comment]: <> (  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>)
[comment]: <> (  {% endif %})
[comment]: <> (  <h4>{{ member.name }}</h4>)
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.page == nil %}
  <h4>{{ member.name }}</h4>
  {% else %}
  <h4> <a href="{{member.page}}"> {{ member.name }} </a> </h4>
  {% endif %}
  <div style="display: flow-root;">
  <i>
    <!--<a href="{{member.email_link}}" onclick="popup=window.open({{member.email_link}},'mailhidepopup','width=580,height=635'); return false;"> <strong> Email </strong> </a> <br>-->
    <strong> Email : </strong>
    <a href = "mailto: {{member.email}}"> {{member.email}} </a><br>
    <strong> Research Interests: </strong> {{member.research_interests}}
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
  </ul>
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

## Visitors
{% assign number_printed = 0 %}
{% for member in site.data.members_visitor %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
[comment]: <> (  {% if member.page == nil %})
[comment]: <> (  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />)
[comment]: <> (  {% else %})
[comment]: <> (  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>)
[comment]: <> (  {% endif %})
[comment]: <> (  <h4>{{ member.name }}</h4>)
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.page == nil %}
  <h4>{{ member.name }}</h4>
  {% else %}
  <h4> <a href="{{member.page}}"> {{ member.name }} </a> </h4>
  {% endif %}
  <div style="display: flow-root;">
  <i>
    <!--<a href="{{member.email_link}}" onclick="popup=window.open({{member.email_link}},'mailhidepopup','width=580,height=635'); return false;"> <strong> Email </strong> </a> <br>-->
    <strong> Email : </strong>
    <a href = "mailto: {{member.email}}"> {{member.email}} </a><br>
    <strong> Research Interests: </strong> {{member.research_interests}}
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
  </ul>
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

## Interns
{% assign number_printed = 0 %}
{% for member in site.data.members_intern %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
[comment]: <> (  {% if member.page == nil %})
[comment]: <> (  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />)
[comment]: <> (  {% else %})
[comment]: <> (  <a href="{{member.page}}"><img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /></a>)
[comment]: <> (  {% endif %})
[comment]: <> (  <h4>{{ member.name }}</h4>)
  <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.page == nil %}
  <h4>{{ member.name }}</h4>
  {% else %}
  <h4> <a href="{{member.page}}"> {{ member.name }} </a> </h4>
  {% endif %}
  <div style="display: flow-root;">
  <i>
    <!--<a href="{{member.email_link}}" onclick="popup=window.open({{member.email_link}},'mailhidepopup','width=580,height=635'); return false;"> <strong> Email </strong> </a> <br>-->
    <strong> Email : </strong>
    <a href = "mailto: {{member.email}}"> {{member.email}} </a><br>
    <strong> Research Interests: </strong> {{member.research_interests}}
  </i>
  <ul style="overflow: hidden">
  {% for educ in member.educations %}
  <li> {{ educ }} </li>
  {% endfor %}
  </ul>
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
## Alumni
#### **Graduate Students**
<div class="row">
{% for member in site.data.members_alumni_graduate %}
<div class="col-xs-12 clearfix">
{% if member.page == nil %}
**{{ member.name }}** (~{{member.end}}) <span style="color:grey">Now {{member.status}}</span>
{% else %}
**<a href="{{member.page}}"> {{ member.name }} </a>** (~{{member.end}}) <span style="color:grey">Now {{member.status}}</span>
{% endif %}
</div>
{% endfor %}
</div>
#### **Undergraduate Students**
<div class="row">
{% for member in site.data.members_alumni_under_graduate %}
<div class="col-xs-12 clearfix">
{% if member.page == nil %}
**{{ member.name }}** (~{{member.end}}) <span style="color:grey">Now {{member.status}}</span>
{% else %}
**<a href="{{member.page}}"> {{ member.name }} </a>** (~{{member.end}}) <span style="color:grey">Now {{member.status}}</span>
{% endif %}
</div>
{% endfor %}
</div>
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