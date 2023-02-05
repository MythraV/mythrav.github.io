---
layout: page
title: Coaching by Demonstration
description: Learning policies from demonstrations and sparse online corrections (coaching)
img: assets/img/cbd.jpg
importance: 1
category: Purdue
---

Human experts commonly teach their fellow collaborators to perform tasks via a small
number of demonstrations, often followed by episodes of coaching that refine the trainee’s
execution during practice. This task refinement through sporadic feedback improves learning
performance and efficacy. State-of-the-art methods for robot learning use imitation learning which is just learning from a large set of demonstrations. 

These approaches are not only limited by availability of demonstrations but have high variability with noise or ambiguity in the demonstation data. To overcome these limitations, the proposed method employs online task correction (coaching) by an expert similar to human tutelage. Unlike RLHF methods with focus on evaluative feedback, the coaching by demonstration (CbD) framework leverages corrective feedback to reshape policies. CbD combines a novel LfD based practice with online policy corrections for improving task performance and learning efficiency. 

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/cbd_framework_new.jpg" title="The CbD framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Coaching by Demonstration (CbD) framework.
</div>

The coaching dynamics is formalized as a partially observable process where the agent's policy 
$$\pi_\phi(s)$$ is different from true policy $$\pi_{\phi^*}(s)$$. The online point corrections can be propogated across the trajectory by smoothing using objectives such as minimum-jerk or minimum-snap. Further the policy reward can be combined with new coach reward based on the corrections. The agent needs to learn a weighting over these rewards, based on observations of corrective actions. This can essentially be formalized as a partially observable Markov process where the agent learns the true policy and reward weight parameters ($$\theta^*$$). This reduces to a formulation similar to the one presented in [1] in the context of phyiscal HRI and [2] for shared autonomy.

As solving POMDP in intractable in high-dimensional cases we reduce this to a policy shaping problem. The policy shaping in CbD is acheived by perturbing the policy at the coached states to match the distribution of policy under these states to the coached actions. This is performed by online updates using a KL loss. 

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/coach_pomdp.jpg" title="The CbD framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The coaching approach using partially observable model.
</div>


[1]Bajcsy, A., Losey, D. P., O’malley, M. K., & Dragan, A. D. (2017, October). Learning robot objectives from physical human interaction. In Conference on Robot Learning (pp. 217-226). PMLR.

[2]Pellegrinelli, S., Admoni, H., Javdani, S., & Srinivasa, S. (2016, October). Human-robot shared workspace collaboration via hindsight optimization. In 2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) (pp. 831-838). IEEE.