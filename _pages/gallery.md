---
layout: page
permalink: /gallery/
title: gallery
description: Photos with robots.
nav: true
nav_order: 9
---

<div class="gallery-grid">
  {% assign photos = "Jin+ICRA.png|Jin+NAO.jpg|Jin+OSU.jpg|Jin+Robojacket.jpg|Jin+Robojacket2.jpg|Jin+UPS.jpeg" | split: "|" %}
  {% for photo in photos %}
    {% include figure.liquid path="assets/img/gallery/{{ photo }}" class="img-fluid rounded z-depth-1" zoomable=true %}
  {% endfor %}
</div>

<style>
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 1rem;
}
.gallery-grid figure {
  margin: 0;
}
</style>
