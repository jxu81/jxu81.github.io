---
layout: page
title: Human-Robot Collaboration
description: a game-theoretical approach to human-robot interaction
img: assets/img/6.bayes.png
importance: 4
category: work
related_publications: true
---

Humans frequently engage in activities with others in shared spaces, such as driving in traffic, shopping at a grocery store, or cooking in a shared kitchen. These activities are typically characterized by the presence of individual goals rather than being purely competitive or purely cooperative. We refer to such activities, where individually motivated agents perform tasks in shared environments, as parallel play. As robots become increasingly prevalent in our daily lives, it is essential for them to be capable of participating in parallel play activities with humans, seamlessly integrating into these shared spaces and contributing to the dynamic yet individually driven nature of these tasks. In this work, we explore game-theoretical approaches to solve multi-agent interaction problems with a focus on efficiency and safety. We developed Bayes–Nash, a Bayesian inference algorithm for Nash equilibrium selection in human-robot interaction. Our findings indicate that using this Bayesian approach can significantly reduce collisions and improve task efficiency compared to traditional methods. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/driving.png" title="Scenario 1: driving in traffic scenario" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/shopping.png" title="Scenario 2: shopping at a grocery store" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/cooking.png" title="Scenario 3:cooking in a shared kitchen" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Applications of the Bayes-Nash Algorithm: navigating traffic (left),  shopping at a grocery store (middle), cooking in a shared kitchen (right).
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/6.Bayes2.png" title="Overview image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    In a collaborative pick-and-place task scenario, multiple agents, whether human or artificial, work together to select objects from one location and transport them to another predetermined location. This task often requires coordination, communication, and cooperation among the agents to successfully accomplish the goal.
</div>


For more information, please check out our talk at [RSS 2020](https://roboticsconference.org/2020/program/papers/42.html) and our publications {% cite bansal2022bayes isbell:pplayw:2021 bansal2020bayesian %} 





