---
title: "3D Vision Lab - Gallery"
layout: piclay
excerpt: "3D Vision Lab -- Gallery"
permalink: /gallery/
---

## Gallery
{% assign number_printed = 0 %}
{% for pic in site.data.gallery %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<figure>
<span>{{ pic.title }}</span>
<img src="{{ site.url }}{{ site.baseurl }}/images/mainpic/{{ pic.image }}" class="img-responsive" width="100%" style="float: left"/>
</figure>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 0 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>
