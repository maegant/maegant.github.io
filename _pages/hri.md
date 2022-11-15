---
layout: page
permalink: /research/hri
title: Human-Robot Interaction
header:
    image: images/papers/cospar.png
description: Research thread aimed at customizing robotic assistance by learning directly from human feedback.
nav: false
---

In order to realize complex robotic behaviors in the real world, human operators often have to manually tune various parameters ranging from low-level controller gains to high-level features. For example, the constraints of gait generation optimization problems are often manually tuned to obtain walking gaits that result in stable, robust, and visually-appealing bipedal locomotion. Also, for locomotion on lower-body exoskeletons, gait features such as step length and step duration are typically tuned until the resulting gait is comfortable for an individual user. Thus, to speed up this process of user-customization and enable faster realization of stable experimental locomotion, my research aims to develop a systematic method of customization by learning directly from subjective human feedback. Importantly, the resulting robotic behavior still enjoys theoretic guarantees since the learning merely shapes the control theoretic approaches from the field of bipedal locomotion. Lastly, the importance of leveraging only *subjective* human feedback is that humans have a natural inclination for what is *good* behavior in ways that are not able to be captured numerically. 

To date, my research towards human-robot interaction has included developing human-in-the-loop preference-based learning algorithms for optimizing and characterizing user preference. These algorithms were demonstrated on the Atalante exoskeleton to optimize user comfort, on the AMBER-3M biped to obtain operator-preferred spring-foot and point-foot walking gaits directly in the gait generation framework, and on the Unitree A1 quadruped to achieve both safe and performant locomotion by tuning parameters of a control barrier function.

<div class="publications">

{% bibliography -f papers -q @*[category=HRI]* %}

</div>