---
title: "3D Vision Lab - Class"
layout: textlay
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /class/
---
# <u>Workshops</u>

### Upcoming
{% for article in site.data.workshops_upcoming %}
<!-- <div class="row"> -->
<div class="col-sm-12 clearfix">
  {% if article.page == nil %}
  <h4>{{article.date}}: {{ article.headline }}</h4>
  {% else %}
  <h4>{{article.date}}: <a href="{{article.page}}">{{ article.headline }}</a></h4>
  {% endif %}
</div>
{% endfor %}
&nbsp;

### Past
{% for article in site.data.workshops_past %}
<!-- <div class="row"> -->
<div class="col-sm-12 clearfix">
  {% if article.page == nil %}
  <h4>{{article.date}}: {{ article.headline }}</h4>
  {% else %}
  <h4>{{article.date}}: <a href="{{article.page}}">{{ article.headline }}</a></h4>
  {% endif %}
</div>
{% endfor %}
&nbsp;



# <u>Classes</u>

### Current Classes
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
&nbsp;



### Past Classes
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
