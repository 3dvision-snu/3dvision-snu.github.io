---
title: "3D Vision Lab - Workshops"
layout: textlay
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /workshops/
---

# Workshops

## Upcoming
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

## Past
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