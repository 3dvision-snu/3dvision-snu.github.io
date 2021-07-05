---
title: "3D Vision lab - Openings"
layout: gridlay
excerpt: "3D Vision lab: Openings"
sitemap: false
permalink: /openings/
---

## We have two current openings!
<br>
{% assign number_printed = 0 %}
{% for internship in site.data.openings %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}
#### ({{internship.date}}) <strong>{{internship.name}}</strong>
<div class="col-sm-12 clearfix">
  <div style="display: flow-root;">
  <br>
  <i>
    3D Vision Lab works on the exciting intersection of computer graphics, computer vision and robotics. We are currently recruiting students to conduct research in
    <strong> {{ internship.name }}</strong>.<br>
  </i>
  <br>
  <i>
    <strong> Candidate Qualifications </strong>
  </i>
  <ul style="overflow: hidden">
  {% for qual in internship.qualifications %}
  <li> {{ qual }} </li>
  {% endfor %}
  <li> Experiences with one or more of the following is a plus: </li>
    <ul style="overflow: hidden">
    {% for experience in internship.experiences %}
    <li> {{ experience }} </li>
    {% endfor %}
    </ul>
  <li> Having taken classes related to the following topics is a plus: </li>
    <ul style="overflow: hidden">
    {% for class in internship.classes %}
    <li> {{ class }} </li>
    {% endfor %}
    </ul>
</ul>
  <i>
    <strong> Related Works </strong>
  </i>

  {% for work in internship.related_works %}
  * [{{work}}]({{work}})
    {% endfor %}
<i>
<strong> Working Hours </strong>
</i>
<ul style="overflow: hidden">
<li> {{internship.working_hours}} </li>
</ul>
  <i>
    <strong> Contact </strong>
  </i>
  <br>


* Please contact Prof. Young Min Kim([{{ internship.contact }}]({{ internship.contact }})) with your CV, transcript, and expected internship period. 

<br>
<br>
<br>
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
