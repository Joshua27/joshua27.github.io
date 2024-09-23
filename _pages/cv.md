---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Dr. rer. nat. in Computer Science, University of Düsseldorf, 2023 (magna cum laude)
* M.Sc. in Computer Science, University of Düsseldorf, 2017
* B.Sc. in Computer Science, University of Düsseldorf, 2015

Projects
======
  <ul>{% for post in site.portfolio %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
