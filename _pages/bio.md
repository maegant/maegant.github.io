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
        Maegan Tucker received the B.S. degree in Mechanical Engineering from the Georgia Institute of Technology (Georgia Tech) in 2017, and the M.S. and Ph.D. degrees in Mechanical Engineering from the California Institute of Technology (Caltech) in 2019 and 2023, respectively. In 2023, she was also a postdoctoral researcher for Caltech, as well as a Research Engineer for Walt Disney Imagineering Research and Development. In 2024, Maegan joined Georgia Tech as an Assistant Professor, with a joint appointment in both the School of Electrical and Computer Engineering, as well as the George W. Woodruff School of Mechanical Engineering. Her awards and recognitions include the 2022 Simoudis Discovery Prize from Caltech, the 2023 Centennial Prize for Best Thesis in Mechanical and Civil Engineering from Caltech, and two "Best Paper" awards (Best Conference Paper and Best Paper in Human Robot Interaction) for the IEEE International Conference on Robotics and Automation (ICRA) in 2020.
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


