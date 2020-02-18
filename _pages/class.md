---
title: "3D Vison Lab - Class"
layout: textlay
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /class/
---


### Current Classes
{% for class in site.data.classes_current %}
<!-- <div class="row"> -->
<div class="col-sm-12 clearfix">
  <h4><a href="{{class.page}}">{{ class.name }}</a>{: style="color:black; text-decoration:underline"}</h4>
</div>
{% endfor %}


### Past Classes
{% assign classes = (site.data.classes_past | sort: 'semester') | reverse %}
{% for class in classes %}
<!-- <div class="row"> -->
<div class="col-sm-12 clearfix">
  <h4><a href="{{class.page}}">{{ class.name }} ({{class.semester}})</a>{: style="color:black; text-decoration:underline"}</h4>
</div>
{% endfor %}
