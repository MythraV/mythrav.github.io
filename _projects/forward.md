---
layout: page
title: Remote Semi-autonomous Tele-surgery
description: A delay tolerant remote system for semi-autonomous robotic surgery
img: assets/img/forward_2.png
importance: 3
category: Purdue
---

Semi-autonomous teleoperation has been proposed as a solution for robotic assistance in austere environments. Nevertheless, having a remote teleoperator makes the system vulnerable to delays and cyber-attacks. The goal of the FORwARD project is to develop a semi-autonomous teleoperation framework that can effectively deal with delays. We propose a system where the surgeon performs a procedure in a realistic simulator uninterrupted. The actions of the surgeon are automatically recognized and sent as high level commands to the real robot, where these instructions are performed semi autonomously. Furthermore, we also propose a model for skill transfer between robots. This model is comprised of a robot agnostic framework with the ability of recognizing and performing surgical steps that have been learned in other domains. This framework significantly reduces the amount of visual and kinematic information that needs to be transmited for teleoperation, with minimal changes to the user experience of the surgeon.


<div class="row justify-content-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/forward.jpg" title="The CbD framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Semi-autonomous remote surgery framework
</div>

DESK Dataset
We have createda a DESK (DExterous Surgical SKills) dataset which comprises a set of surgical robotic skills collected during a surgical training task using five robotic platforms: the Taurus II robot, the Taurus II simulated robot, the YuMi robot, the YuMi simulated robot, the da Vinci surgical robot. We conducted extensive experiments with three supervised learning models and provided baselines in each of these scenarios. Results show that using simulation data during training enhances the performance on the real robots, where limited real data is available.

The dataset can be accessed <a href="https://purdue0-my.sharepoint.com/personal/gonza337_purdue_edu/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fgonza337%5Fpurdue%5Fedu%2FDocuments%2FForward%2FData%20Collection&ga=1"><b>here</b></a>

<div class="row justify-content-center">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.html path="assets/img/desk_all.png" title="The CbD framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The robots in the DESK dataset
</div>