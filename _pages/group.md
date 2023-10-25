---
layout: default
permalink: /group/
title: group@GT
description:  
nav: true
nav_order: 2
---

<!-- ## Lab Members -->

{% assign all_people = site.people %}

{% assign all_roles = 'Research Team' | split: '|'  %}

{% for role in all_roles %}

  {% assign people_for_role = all_people | where: 'position',role %}


  <!-- <div class="people-title top">
    <h3>Principal Investigator</h3>
  </div> -->

  <div class="justify-content-center">
  {% include dynamicmobility.html %}
  </div>

  <hr class="people-group">

  <div class="people-title">
    <h3>Research Team</h3>
  </div>

  <div class="content list people">

    {% for person in all_people %}
      {% if person.position == 'researchengineer' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'postdoc' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'phd' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'gradstudent' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'undergrad' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'affiliate' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

  </div>


 <hr class="people-group">

 <!-- <div class="people-title mb-3">
    <h3>Alumni</h3>
 </div> -->

  <!-- <div class="content list people"> -->
	
  {% for person in all_people %}
      {% if person.position == 'alumni' %}
        {% include alumni.html position=person.position %}
      {% endif %}
    {% endfor %}
  <!-- </div> -->

{% endfor %}
<br>

