---
title: "3D Vision lab - Openings"
layout: gridlay
excerpt: "3D Vision lab: Openings"
sitemap: false
permalink: /openings/
---
## Current Opening
{% assign number_printed = 0 %}
{% for internship in site.data.openings %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
  <div style="display: flow-root;">
  <br>

  <i>
    {{ internship.description }}
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
  </ul>
  <br>
  <i>
    <strong> Contact </strong>
  </i>
  <br>
Please contact Prof. Young Min Kim (<{{ internship.contact }}>) with your CV, transcript, and expected internship period. 

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