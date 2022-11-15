---
layout: default
permalink: /research/
title: research
categories: [Locomotion, HRI, Rehab.]
description:  
nav: true
nav_order: 1
dropdown: true
children: 
    - title: "Overview"
      permalink: /research/
    - title: "Thread 1: Locomotion"
      permalink: /research/locomotion
    - title: "Thread 2: HRI"
      permalink: /research/hri
    - title: "Thread 3: Assistance"
      permalink: /research/assistive-devices
    - title: All Publications
      permalink: /publications/
---

<center>    
    <h4> My research aims to develop and unify techniques from both <br> <i>nonlinear control theory</i> and <i>machine learning</i> <br>to systematically achieve stable and robust robotic-assisted locomotion. This includes developing efficient methods of user customization via human-robot interaction as well as studying the efficacy of assisted locomotion in clinical settings. 
    <!-- <b>Bipedal Locomotion</b>, <b>Human Robot Interaction</b>, and <b>Lower-Body Assistive Devices</b>. -->
    </h4>
</center>


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="images/papers/icra2021-hzd.png" class="img-fluid rounded z-depth-1" overlay="Bipedal Locomotion" 
            overlay-url="/research/locomotion" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="images/papers/cospar.png" class="img-fluid rounded z-depth-1" overlay="Human-Robot Interaction" 
        overlay-url="/research/hri" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="images/papers/spinal.png" class="img-fluid rounded z-depth-1" overlay="Lower-Body Assistive Devices" 
        overlay-url="/research/assistive-devices" %}
    </div>
</div>

<!-- _pages/publications.md -->
<div class="publications">

{%- for c in page.categories %}
  <a id="Test">
  <h2 class="year">{{c}}</h2>
  {% bibliography -f papers -q @*[category={{c}}]* %}
  </a>
{% endfor %}

</div>

