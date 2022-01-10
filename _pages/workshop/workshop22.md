---
title: "3D Vision Lab - Workshop"
layout: textlay
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /workshop/workshop22
---

<html>
<body>
{% for workshop in site.data.workshop.workshop22 %}

<div class='workshop_head'>
<h1 style="color:#3384C1;"> <b> {{workshop.name}} </b> </h1>
<h4 style="text-align:right"> {{workshop.sub_name}} </h4>
</div>

<div class='workshop_date'>
{{workshop.date}} <br>
{{workshop.time}} <br>
</div>

<div class='section'>
{{workshop.description}} <a href="{{workshop.link}}">Zoom Link</a>
</div>

<div class='section'>
  <h3> Schedule </h3>
  {% for content in workshop.Content %}
    <br>
    {% if content.type == "invited" %}
    <p style="font-size:16px;color:#16598B;"> <b> {{content.time}} Invited speaker : {{content.speaker.name}} </b> </p>
      <div class='speakers'>
        <img src="{{ site.url }}{{ site.baseurl }}/images/workshoppic/{{ content.speaker.photo }}">
      </div>
    <div class='invited'>
      <b style="font-size:18px;"> Title : {{content.title}} </b> <br>
      <p> Abstract : {{content.abstract}} <br> </p>
      <p> Bio : {{content.bio}} <br> </p>
    </div>
    {% else %}
    {% if content.type == "student" %}
      <p style="font-size:16px;color:#16598B;"> <b> {{content.time}} Student talks </b> </p>
      {% for talks in content.talks %}
      {{talks.speaker}} | {{talks.title}} <br>
      {% endfor %}
    {% else %}
      <p style="font-size:16px;color:#16598B;"> <b> {{content.time}} Break </b> </p> <br>
    {% endif %}
    {% endif %}
  {% endfor %}

</div>

<div class='remarks'>
{{workshop.Support}} <br>
Contact : Young Min Kim (<a href="mailto:youngmin.kim@snu.ac.kr">youngmin.kim@snu.ac.kr</a>) <br> 
</div>

<div class='banners'>
{% for banner in workshop.Banners %}
<img src="{{ site.url }}{{ site.baseurl }}/images/workshoppic/{{ banner.photo }}">
{% endfor %}
</div>

{% endfor %}


</body>
</html>