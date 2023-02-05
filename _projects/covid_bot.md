---
layout: page
title: Smart Covid Robots
description: Autonomous ground robots for COVID disinfection.
img: assets/img/omniveyor.jpg
importance: 5
category: Purdue
---

Living with the ongoing COVID-19 pandemic presents unique challenges for daily interactions, businesses, and facility maintenance, especially in regards to maintaining a high level of cleanliness in shared spaces such as offices, schools, elevators, classrooms, and cafeterias. The traditional methods of indoor disinfection, such as ultraviolet light and chemical sprays, are problematic as they can irritate humans and can only be used when the facility is unoccupied.

While stationary air filtration systems are irritation-free and widely available, they have limitations in air circulation and diffusion, making it difficult to protect all occupants. To address this challenge, we developed a new collaborative robot (cobot) disinfection system equipped with a Bernoulli Air Filtration Module. The design of this system minimizes disruption to the surrounding airflow and allows for maximum coverage while navigating among occupants.

A Computational Fluid Dynamics (CFD) simulation was conducted to analyze the impact of robotic air filtration on the dose received by neighbors of a coughing source. Based on this analysis, a novel occupant-centric online rerouting algorithm was developed to guide the path of the cobot.


<div class="row justify-content-sm-center">
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.html path="assets/img/omniveyor.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/covidbot.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The omniveyor robot as smart conveyors (left) and covid patrol robot (right)
</div>

Similarly, we used the bases of these robots to develop a smart industrial conveyor system. A digital twin of the shop floor was created to enable users to dynamically generate behaviors by interacting with the simulation. 