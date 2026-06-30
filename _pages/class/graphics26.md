---
title: "3D Vision Lab - Class"
layout: textlay
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /class/graphics26
---

<html>
<body>
{% for class in site.data.classes_graphics26 %}

<h2> {{class.name}} </h2> <br>

<div class='section'>
<h3> Course Description </h3> <br>
{{class.CourseDescription}}
</div>

<div class='section'>
  <div class='instructor-section'>
    <h3>Instructor</h3>
    <div class='instructor'>
      <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ class.instructor.photo }}">
      <div>{{ class.instructor.name }}</div>
    </div>
  </div>
  <div class='instructor-section'>
    <h3>Teaching Assistants</h3>
    {% for ta in class.TAs %}
    <div class='ta'>
      <img src="{{ site.url }}{{ site.baseurl }}/images/memberspic/{{ ta.photo }}">
      <div>{{ ta.name }}</div>
    </div>
    {% endfor %}
  </div>
</div>


<div class='section'>
  <h3>&#127881; &#127881; Final Project Winners &#127881; &#127881;</h3>
  <li><b>1st Place: </b> Team3 김용석 김영현 문성빈 이준하</li>
  <li><b>2nd Place: </b> Team6 김세희 양준호 한주환 이정환 / Team10 노치윤 정승훈 / Team13 김수홍 이상화 황민호</li>

  <h3>Final Project</h3>
  {% for project in class.Syllabus.FinalProject.Projects %}
  <br><li> {{project.studentName}} </li>
  {% if project.youtubeLinkId %}
  <iframe width="750" height="450" src="https://www.youtube.com/embed/{{project.youtubeLinkId}}" frameborder="0" allowfullscreen></iframe>
  {% elsif project.photo %}
    {% for img in project.photo %}
    <div class='class_student'>
      <img src="{{ site.url }}{{ site.baseurl }}/images/classpic/graphics26/{{ img }}" style='height:auto;width:750px'>
    </div>
    {% endfor %}
  {% endif %}
  {% endfor %}

</div>

{% endfor %}


</body>
</html>
