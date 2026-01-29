---
title: "3D Vision Lab - Publications."
layout: gridlay
excerpt: "3D Vision Lab -- Publications."
sitemap: false
permalink: /publications/
---


## Publications
<br>
<br>
<h3><span style="color:black">  2026 </span></h3>
{% for publi in site.data.publist2026 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.page %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% else %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% endif %}
</div>
{% endfor %}

<br>
<h3><span style="color:black">  2025 </span></h3>
{% for publi in site.data.publist2025 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.page %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% else %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% endif %}
</div>
{% endfor %}

<br>
<h3><span style="color:black">  2024 </span></h3>
{% for publi in site.data.publist2024 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.page %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% else %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% endif %}
</div>
{% endfor %}

<br>
<h3><span style="color:black">  2023 </span></h3>
{% for publi in site.data.publist2023 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.page %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% else %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% endif %}
</div>
{% endfor %}

<br>
<h3><span style="color:black">  2022 </span></h3>
{% for publi in site.data.publist2022 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.page %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% else %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% endif %}
</div>
{% endfor %}

<br>
<h3><span style="color:black">  2021 </span></h3>
{% for publi in site.data.publist2021 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.page %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% else %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% endif %}


</div>
{% endfor %}

<br>
<h3><span style="color:black">  2020 </span></h3>
{% for publi in site.data.publist2020 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.page %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.page }}">[project page]</a></strong>
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% else %}

  {% if publi.link.code %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}

  {% else %}

  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}

  {% endif %}

  {% endif %}
</div>
{% endfor %}

<br>
<h3><span style="color:black">  2019 </span></h3>
{% for publi in site.data.publist2019 %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.code %}
  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}
  {% else %}
  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}
  {% endif %}
</div>
{% endfor %}

<br>
<h3><span style="color:black">  before 2019 </span></h3>
{% for publi in site.data.publist2019prev %}
<div class="pub" style="display: inline-block; width: 100%; margin: 20px 0 20px 0"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}"/>
  <pubtit>{{ publi.title }}</pubtit>
  <em>{{ publi.authors }} </em><br />
  <strong>{{ publi.link.display }}</strong><br/>
  {% if publi.link.code %}
  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.code }}">[code]</a></strong>
  {% endif %}
  {% else %}
  {% if publi.link.video %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  <strong><a href="{{ publi.link.video }}">[video]</a></strong>
  {% else %}
  <strong><a href="{{ publi.link.url }}">[pdf]</a></strong>
  {% endif %}
  {% endif %}
</div>
{% endfor %}

