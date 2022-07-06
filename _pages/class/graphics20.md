---
title: "3D Vision Lab - Class"
layout: textlay
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /class/graphics20
---

<html>
<body>
{% for class in site.data.classes_graphics20 %}

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
  <h3>Syllabus</h3><br>
  <b>Class time</b> : {{ class.Syllabus.ClassTime }} <br>
  <b>Location</b> : {{ class.Syllabus.Location }} <br>
  <b>Textbooks</b> : {{ class.Syllabus.Textbooks }} <br>
  <b>Topics</b>    
    <ul>
      {% for topic in class.Syllabus.Topics %}
      <li> {{ topic }} </li>
      {% endfor %}
    </ul>
  <b>Prerequisites</b>
  <br>
    <ul>
      {% for course in class.Syllabus.Prerequisites %}
      <li> {{ course }} </li>
      {% endfor %}
    </ul>
  <b>Grading Policy</b>
    <ul>
      {% for item in class.Syllabus.GradingPolicy %}
      <li> {{item.name}}({{item.ratio}}%) : {{item.contents}} </li>
      {% endfor %}
    </ul>
</div>

<div class='section'>
  <h3>Final Project</h3>
  {% for video in class.Syllabus.FinalProject.Videos %}
  <br><li> {{video.studentName}} </li>
  <iframe width="750" height="450" src="https://www.youtube.com/embed/{{video.youtubeLinkId}}"  frameborder="0" allowfullscreen></iframe>
  {% endfor %}

  {% for image in class.Syllabus.FinalProject.Images %}
  <br><li> {{image.studentName}} </li>
    {% for img in image.photo %}
    <div class='class_student'>
      <img src="{{ site.url }}{{ site.baseurl }}/images/classpic/graphics20/{{ img }}">
    </div>
    {% endfor %}
  {% endfor %}

</div>

{% endfor %}


</body>
</html>