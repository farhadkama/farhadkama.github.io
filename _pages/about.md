---
permalink: /
title: "Farhad Kamarei"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my website!! It is currently under development




About me
======
I'm a Ph.D. candidate at University of Illinois Urbana Champaign in the Civil and Environmental Engineering Depatrment. I am doing my Ph.D. under supervison of [Prof. Oscar Lopez-Pamies](https://pamies.cee.illinois.edu/).

<p align="center">
  <img src="/images/university_logo.png" alt="University Logo" width="250"/>
  <img src="/images/department_logo.png" alt="Department Logo" width="500"/>
</p>
I am interesed in solving partial differential equations, both numerically and theoretically, with application to applied mechanics.

My Reseach
======
My research focuses on the theory of fracture in dissipative material via the phase-field regularization. Specefically, my thesis title is


Publications
======
Here is a list of my recent publications:

<ol>
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for pub in pubs limit:5 %}
  <li>
    <strong>{{ pub.title }}</strong><br>
    <em>{{ pub.authors }}</em><br>

    {% if pub.paperurl %}
      <a href="{{ pub.paperurl }}" target="_blank" class="btn-doi"> doi</a>
    {% endif %}
    
    {% if pub.researchgate %}
      <a href="{{ pub.researchgate }}" target="_blank" style="background:#0cb;color:white;padding:2px 6px;border-radius:4px;text-decoration:none;font-size:0.85em;">ResearchGate</a>
    {% endif %}

    <br><small>{{ pub.venue }}, {{ pub.date | date: "%Y" }}</small>
  </li>
{% endfor %}
</ol>

<a href="{{ '/publications/' | relative_url }}">See all publications →</a>


