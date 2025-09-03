---
layout: default
title: Recipes (Tournament Ideas)
permalink: /library/recipes/
---

<section class="deco-card">
  <span class="corner tl"></span><span class="corner tr"></span>
  <span class="corner bl"></span><span class="corner br"></span>
  <h2>Recipes</h2>
  <p>Formats, scoring quirks, and ways to make people mad in a useful way.</p>
  <ul class="post-list">
    {% for r in site.recipes %}
      <li>
        <a class="post-link" href="{{ r.url | relative_url }}">
          {{ r.title }}
        </a>
      </li>
    {% endfor %}
  </ul>
</section>

