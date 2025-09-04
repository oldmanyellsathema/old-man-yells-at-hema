---
layout: default
title: Gallery
permalink: /library/gallery/
---

<section class="deco-card">
  <span class="corner tl"></span><span class="corner tr"></span>
  <span class="corner bl"></span><span class="corner br"></span>
  <h2 class="invite-title" style="text-align:center;">Gallery</h2>

  <ul class="post-list">
    {% assign gallery = site.library | where: "section", "gallery" %}
    {% for item in gallery %}
      <li>
        <a class="post-link" href="{{ item.url | relative_url }}">
          <span class="post-title">{{ item.title }}</span>
        </a>
      </li>
    {% endfor %}
  </ul>
</section>
