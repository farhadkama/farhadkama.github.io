---
permalink: /
title: "Farhad Kamarei"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my website!!




About me
======

I'm a Ph.D. candidate at University of Illinois Urbana Champaign in the Civil and Environmental Engineering Depatrment. I am doing my Ph.D. under supervison of [Prof. Oscar Lopez-Pamies](https://pamies.cee.illinois.edu/).


<p align="center">
  <img src="/images/university_logo.png" alt="University Logo" width="250"/>
  <img src="/images/department_logo.png" alt="Department Logo" width="500"/>
</p>

<div style="text-align: justify;">
I develop mathematical models and computational frameworks for solving partial differential equations, with a focus on applications in mechanics and physics of soft solids.
</div>


My Reseach
======

<div style="text-align: justify;">
I am currently developing theoretical and numerical frameworks for the phase-field approach to fracture mechanics, under quasistatic and monotonically increasing loading conditions.
My doctoral research, titled "Nucleation and Propagation of Fracture in Viscoelastic Elastomers: A Complete Phase-Field Theory and Robust Numerical Implementation," presents a comprehensive theory and numerical framework for modeling crack nucleation and propagation in viscoelastic elastomers. This work advances our understanding of fracture behavior for a more general and  complex material behavior and provides robust computational tools for predicting fracture mechanisms.
</div>

<p align="center">
  <img src="/images/PS_web.jpeg" alt="Pure shear test" width="250"/>
</p>

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


