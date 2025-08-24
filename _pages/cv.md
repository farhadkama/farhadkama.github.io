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

Research experience
======
* Fall 2022 - Current: Graduate Research Assistant  
  * Prof. Lopez-Pamies' Research Group

Publications
======
<ul style="list-style: none; padding-left: 0; font-size: 0.9em;">
  {% assign total_pubs = site.publications | size %}
  {% for post in site.publications reversed %}
    <li style="margin-bottom: 0.6em;">
      [{{ total_pubs | minus: forloop.index0 }}]
      <strong>{{ post.title }}</strong>.
      {{ post.date | date: "%Y" }}.
      {{ post.citation | remove: post.title }} 
      <em>{{ post.venue }}</em>{% if post.issue %}, {{ post.issue }}{% endif %}{% if post.pages %}, {{ post.pages }}{% endif %}.
    </li>
  {% endfor %}
</ul>






Talks
======
<ul style="list-style: none; padding-left: 0; font-size: 0.9em;">
  {% assign total_talks = site.talks | size %}
  {% for post in site.talks reversed %}
    <li style="margin-bottom: 0.6em;">
      [{{ total_talks | minus: forloop.index0 }}] 
      <strong>{{ post.title }}</strong>,
      {{ post.date | date: "%B %d, %Y" }},
      {{ post.venue }},
      {{ post.location }}
    </li>
  {% endfor %}
</ul>

Teaching
======
<ul style="list-style: none; padding-left: 0; font-size: 0.9em;">
  {% for post in site.teaching reversed %}
    <li style="margin-bottom: 0.6em;">
      <strong>{{ post.title }}</strong>,
      {{ post.date | date: "%B %Y" }},
      {{ post.venue }}
    </li>
  {% endfor %}
</ul>

