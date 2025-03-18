---
layout: default
permalink: /bio/
title: bio/cv
nav: true
nav_order: 2
cv_pdf: cv.pdf
---

<html>
    <div class="post">
        <header class="post-header">
        <h1 class="post-title">Biographical Sketch</h1>
        </header>
        <article>
        Maegan Tucker is an Assistant Professor at Georgia Tech, jointly appointed in Electrical and Computer Engineering and Mechanical Engineering (since January 2024). She earned her B.S. in Mechanical Engineering from Georgia Tech (2017) and her M.S. (2019) and Ph.D. (2023) from Caltech. In 2023, she was a postdoctoral researcher at Caltech and a Research Engineer at Walt Disney Imagineering R&D. Prof. Tucker's research focuses on the areas of hybrid system theory, robotic bipedal locomotion, human-robot interaction, and the biomechanics of lower-limb assistive technology. Ultimately, her work aims to develop personalized assistive devices to improve mobility for individuals with locomotor impairments. Prof. Tucker's awards and recognitions include the 2023 Centennial Prize for Best Thesis in Mechanical and Civil Engineering from Caltech, the 2022 Simoudis Discovery Prize from Caltech, and two "Best Paper" awards (Best Conference Paper and Best Paper in Human Robot Interaction) for the IEEE International Conference on Robotics and Automation (ICRA) in 2020.
        </article>
    </div>
    <br>
    <div class="post">
        <header class="post-header">
        <h1 class="post-title">CV</h1>
        </header>
        <object data="{{ page.cv_pdf | prepend: 'assets/pdf/' | relative_url }}#toolbar=1&navpanes=0" style="min-height:100vh;width:100%" type='application/pdf'/>
    </div>
</html>


