---
title: "3D Vision Lab - Publications."
layout: gridlay
excerpt: "3D Vision Lab -- Publications."
sitemap: false
permalink: /publications/
---


## Publications

{% for publi in site.data.publist %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0">
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>

</div>

{% endfor %}

