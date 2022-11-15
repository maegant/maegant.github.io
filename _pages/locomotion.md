---
layout: page
permalink: /research/locomotion
title: Bipedal Locomotion
header:
    image: images/papers/icra2021-hzd.png
description: Research thread aimed at developing systematic methods of achieving complex robotic behaviors, including stable and robust bipedal locomotion, by leveraging tools from nonlinear control theory.
nav: false
---

The field of nonlinear control has demonstrated success towards realizing complex robotic behaviors, including bipedal locomotion. Most importantly, nonlinear controllers account for the full system dynamics, allowing for theoretical guarantees. However, when a human is introduced into the system, our knowledge of the system dynamics decreases. Thus, a critical step to maintaining theoretic guarantees in cases when a human is part of the system, such as the case with lower-body assistive devices, is to better define the theoretical conditions underlying provably robust and stable locomotion. Once we better understand these notions, we can develop systematic methods of achieving robust and stable locomotion on a variety of bipedal platforms. 

To date, my research towards bipedal locomotion has included systematically tuning controller gains for a CLF-QP on Cassie, incorporating musculoskeletal models into a gait genreation framework to achieve natural multi-contact walking on the AMPRO3 dual-actuated prosthesis, generating robust limit cycles for both the Atalante exoskeleton and the AMBER-3M biped by leveraging Saltation matrices, and developing methods for active ankle stabilization on Atalante. 

<div class="publications">

{% bibliography -f papers -q @*[category=Locomotion]* %}

</div>