---
layout: default
title: Cheng Shao
images:
  - image_path: /assets/img/touring.jpg
    title: Apple Pie
  - image_path: /assets/img/touring.jpg
    title: Birthday Cake
  - image_path: /assets/img/touring.jpg
    title: Black Forest
---

<ul class="photo-gallery">
  {% for image in page.images %}
    <li><img src="{{ image.image_path }}" alt="{{ image.title}}"/></li>
  {% endfor %}
</ul>
