---
layout: page
title: Indy Autonomous Challenge
description: Full scale autonomous racing at high speeds (>100mph)
img: assets/img/iac.jpg
importance: 4
category: Purdue
---


Driving at high speeds comes with several challenges related to update frequency, braking conditions. Especially in racing conditions where dynamic passing and collision safety is critical to performance. The <a href="https://www.indyautonomouschallenge.com/"><b>Indy Autonomous Challenge</b></a> is a competition to advance autonomous driving technologies and deployments of advanced driver assistant systems (ADAS) to increase safety and performance.  

As part of Purdue team, I developed a hierarchical safety controller to safely bring the vehicle to stop in case on emergencies. In addition, a fall back PD controller was created to run the vehicle if the main controller fails.

The dynamic planning for the vehicle was implemented using a Frenet frame planner to achieve rapid generation of paths for dynamic passing at high speeds.

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/iac.jpg" title="The Purude IAC vehicle" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Purdue IAC vehicle
</div>
