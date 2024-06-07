---
layout: page
title: Multi-agent Robot Learning
description: Zero-shot Human-AI coordination
img: assets/img/3.overcook.png
importance: 3
category: work
related_publications: true
---

Recent advances in multiagent reinforcement learning have enabled artificial agents to work together effectively in complex environments. However, these agents often face difficulties when collaborating with humans. This is partly because they make assumptions about how humans make decisions and behave, which may not always be accurate.

Our research focuses on addressing the challenge of coordinating between humans and AI without prior knowledge of human behavior in a given task. We explore the problem of zero-shot human-AI coordination, where an agent is paired with a human partner in a cooperative task without access to data on human behavior. We explore using known cognitive and behavioral biases (e.g. Confirmation Bias, Anchoring Bias, Loss Aversion) to generate a set of agents to help enable the best response agent to coordinate with humans.

We employ the Overcooked environment developed by [Carroll et al.](https://arxiv.org/abs/1910.05789). This environment offers a mix of strategy and motion coordination challenges, making it particularly suitable for training deep reinforcement learning algorithms.

For more information, please check out our recent publications {% cite isbell:pplay:2022 %}. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/overview-overcooked.JPEG" title="Overview image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Zero-shot human-AI coordination problem in the Overcooked environment.
</div>
