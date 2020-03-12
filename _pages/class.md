---
title: "3D Vison Lab - Class"
layout: textlay
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /class/
---


## Current Classes
{% for class in site.data.classes_current %}
<!-- <div class="row"> -->
<div class="col-sm-12 clearfix">
  {% if class.page == nil %}
  <h4>{{class.semester}}: {{ class.name }}</h4>
  {% else %}
  <h4>{{class.semester}}: <a href="{{class.page}}">{{ class.name }}</a></h4>
  {% endif %}
</div>
{% endfor %}


## Past Classes
{% assign classes = (site.data.classes_past | sort: 'semester') | reverse %}
{% for class in classes %}
<!-- <div class="row"> -->
<div class="col-sm-12 clearfix">
  {% if class.page == nil %}
  <h4>{{class.semester}}: {{ class.name }}</h4>
  {% else %}
  <h4>{{class.semester}}: <a href="{{class.page}}">{{ class.name }}</a></h4>
  {% endif %}
</div>
{% endfor %}
