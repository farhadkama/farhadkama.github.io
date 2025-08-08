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
* Ph.D. in Civil Engineering — Computational Science and Engineering Concentration, University of Illinois Urbana-Champaign, 2026 (expected)
* M.Sc. in Mechanical Engineering, Amirkabir University of Technology (Tehran Polytechnic), 2022
* B.Sc. in Mechanical Engineering, Amirkabir University of Technology (Tehran Polytechnic), 2019

Research  experience
======

* Fall 2022 - Current: Graduate Research Assistant
  * Prof. Lopez-Pamies' Research Group

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
  
