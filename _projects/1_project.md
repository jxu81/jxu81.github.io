---
layout: page
title: ATG Projects
description: R&D projects at UPS Advanced Technology Group
img: assets/img/nvidia5.jpg
importance: 1
category: work
related_publications: false
---
## 1. Interactive System for General-Purpose Robots
Robots (AGVs, AMRs, Quadcopters/Drones, Quadrupeds, Humanoids, and more), regardless its form factor, hold immense potential for addressing the global shortage of human labor and enhancing efficiency within the supply chain and logistics industry. A specific example (shown below) is the use case of a SPOT robot for last-mile delivery, designed and customized by the ATG team at UPS.  
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/spot1.png" title="SPOT - Outdoor" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Outdoor use case: last mile delivery
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/spot2.png" title="SPOT - Indoor" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/spot3.png" title="SPOT - Indoor" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Indoor use case
</div>


In the future, we envision a warehouse where human workers and robots work together collaboatively. To make this possible, we aim to create an interactive system that:

- Facilitates seamless conversation-based interaction between robots and human workers,
- Is adaptable for deployment on any robots within UPS facilities moving forward, and
- Incorporates a customized model built on UPS data and knowledge.

We put this idea into action by implementing the system design outlined below on the SPOT robot and conducted tests at the ATG office. During testing, we found that the latency of both the speech recognition and response models (LLM) is too long, significantly impacting the user experience. Our next step for this project is to deploy LLMs on edge devices to optimize latency.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/spot4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    System architecture of a voice-based interaction system for UPS robots.
</div>


## 2. Humanoid Robots
Humanoid robots have the potential to become the next widely adopted comsumer devices after smartphones. There are several potential benefits of incorporating humanoids in UPS warehouses, such as increased efficiency, enhanced safety, cost savings, etc.

This project aims to explore and evaluate the current state of reinforcement learning on humanoids robot. In particular, we trained Unitree Humanoid H1 to learn basic locommotion and manipulation skills (e.g. crawl, stand, walk) using [HumanoidBench by Sferrazza et al.](https://arxiv.org/abs/2403.10506). These agents are trained using TD-MPC algorithms on GPU for hours and results are shown below.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/stand_0.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
         <figcaption>Starting, 0 training steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/stand_100k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 100k steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/stand_200k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 200k steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/stand_1000k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 1000k steps</figcaption>
        </figure>
    </div>
</div>
<div class="caption">
    Train H1 robot to learn how to stand.
</div>


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/crawl_0.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
         <figcaption>Starting, 0 training steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/crawl_100k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 100k steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/crawl_200k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 200k steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/crawl_1000k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 1000k steps</figcaption>
        </figure>
    </div>
</div>
<div class="caption">
    Train H1 robot to learn how to crawl.
</div>


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/walk_0.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
         <figcaption>Starting, 0 training steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/walk_100k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 100k steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/walk_200k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 200k steps</figcaption>
        </figure>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <figure>
        {% include video.liquid path="assets/video/walk_1000k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
        <figcaption>After 1000k steps</figcaption>
        </figure>
    </div>
</div>
<div class="caption">
    Train H1 robot to learn how to walk.
</div>


## 3. A New Robot for Loading UPS Delivery Vehicle
[Package car loading/unloading](https://www.youtube.com/watch?v=m3tHZ_WxZsc) activity is not just a significant annual labor expense (approximately $1.8 billion) but also one of the most complex automation challenges for UPS and the logistics industry overall. Typically, this process involves a human worker retrieving a package from the conveyor belt, reading its label, identifying the corresponding package car, and then placing the package in the designated area within the car. To tackle this challenge, I devised a method that utilizes a lifting robot and a telescopic conveyor to automatically load packages from the metro belt. This invention has been submitted to the patent office under the title "Loading Objects into a Storage Area in an Automated or Semiautomated Manner."


## 4. Digital Twin of UPS Warehouse Operations using Nvidia Omniverse Platform
The goal of this project was to develop a robotics simulation that closely mimics actual UPS (United Parcel Service) operations. This simulation provides us with the ability to tackle advanced and complex robotics and automation problems within UPS that would otherwise be impossible due to the technology's immaturity and excessive costs. The potential benefits are
- Utilize the simulation as a tool for internal use case discussion and evaluation 
- Serve as a evaluation tool for testing solutions provied by external vendors 
- By utilizing our simulation environment owned by UPS, we can avoid vendors requesting additional funding for developing their own simulations as milestones. We can instead integrate their system into our simulation environment for evaluation purposes.
- Engage the research and open-source community to collaborate on finding solutions and foster collaborations with research labs in universities and institutes to leverage their expertise and resources.
- Potential for developing computer vision algorithms and synthetic data generation to enhance our robot capabilities.
- Assist in visualizing future scenarios and planning for long-term robotics projects to ensure strategic alignment and successful implementation. 

Previews of this project:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/nvidia1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulated Pre-load Operation: a fleet of humanoid robots(Digit) work together to load package car
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/nvidia2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulated Pre-load Operation: a fleet of humanoid robots(Digit) work together to load package car
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/nvidia3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/nvidia4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulated Pre-load Operation: a fleet of humanoid robots(Digit) work together to load package car
</div>




