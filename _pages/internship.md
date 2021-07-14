---
title: "3D Vision lab - Openings"
layout: gridlay
excerpt: "3D Vision lab: Openings"
sitemap: false
permalink: /openings/
---
## No current openings
[comment]: <> (## We have two current openings!)

[comment]: <> (<br>)

[comment]: <> ({% assign number_printed = 0 %})

[comment]: <> ({% for internship in site.data.openings %})

[comment]: <> ({% assign even_odd = number_printed | modulo: 2 %})

[comment]: <> ({% if even_odd == 0 %})

[comment]: <> (<div class="row">)

[comment]: <> ({% endif %})

[comment]: <> (#### &#40;{{internship.date}}&#41; <strong>{{internship.name}}</strong>)

[comment]: <> (<div class="col-sm-12 clearfix">)

[comment]: <> (  <div style="display: flow-root;">)

[comment]: <> (  <br>)

[comment]: <> (  <i>)

[comment]: <> (    3D Vision Lab works on the exciting intersection of computer graphics, computer vision and robotics. We are currently recruiting students to conduct research in)

[comment]: <> (    <strong> {{ internship.name }}</strong>.<br>)

[comment]: <> (  </i>)

[comment]: <> (  <br>)

[comment]: <> (  <i>)

[comment]: <> (    <strong> Candidate Qualifications </strong>)

[comment]: <> (  </i>)

[comment]: <> (  <ul style="overflow: hidden">)

[comment]: <> (  {% for qual in internship.qualifications %})

[comment]: <> (  <li> {{ qual }} </li>)

[comment]: <> (  {% endfor %})

[comment]: <> (  <li> Experiences with one or more of the following is a plus: </li>)

[comment]: <> (    <ul style="overflow: hidden">)

[comment]: <> (    {% for experience in internship.experiences %})

[comment]: <> (    <li> {{ experience }} </li>)

[comment]: <> (    {% endfor %})

[comment]: <> (    </ul>)

[comment]: <> (  <li> Having taken classes related to the following topics is a plus: </li>)

[comment]: <> (    <ul style="overflow: hidden">)

[comment]: <> (    {% for class in internship.classes %})

[comment]: <> (    <li> {{ class }} </li>)

[comment]: <> (    {% endfor %})

[comment]: <> (    </ul>)

[comment]: <> (</ul>)

[comment]: <> (  <i>)

[comment]: <> (    <strong> Related Works </strong>)

[comment]: <> (  </i>)

[comment]: <> (  {% for work in internship.related_works %})

[comment]: <> (  * [{{work}}]&#40;{{work}}&#41;)

[comment]: <> (    {% endfor %})

[comment]: <> (<i>)

[comment]: <> (<strong> Working Hours </strong>)

[comment]: <> (</i>)

[comment]: <> (<ul style="overflow: hidden">)

[comment]: <> (<li> {{internship.working_hours}} </li>)

[comment]: <> (</ul>)

[comment]: <> (  <i>)

[comment]: <> (    <strong> Contact </strong>)

[comment]: <> (  </i>)

[comment]: <> (  <br>)


[comment]: <> (* Please contact Prof. Young Min Kim&#40;[{{ internship.contact }}]&#40;{{ internship.contact }}&#41;&#41; with your CV, transcript, and expected internship period. )

[comment]: <> (<br>)

[comment]: <> (<br>)

[comment]: <> (<br>)

[comment]: <> (</div>)

[comment]: <> (</div>)

[comment]: <> ({% assign number_printed = number_printed | plus: 1 %})

[comment]: <> ({% if even_odd == 1 %})

[comment]: <> (</div>)

[comment]: <> ({% endif %})

[comment]: <> ({% endfor %})

[comment]: <> ({% assign even_odd = number_printed | modulo: 2 %})

[comment]: <> ({% if even_odd == 1 %})

[comment]: <> (</div>)

[comment]: <> ({% endif %})
