---
layout: default
title: Recipes
permalink: /library/recipes/
---

<section class="deco-card">
  <span class="corner tl"></span><span class="corner tr"></span>
  <span class="corner bl"></span><span class="corner br"></span>
  <h2 class="invite-title" style="text-align:center;">Recipes</h2>
 <p style="text-align:center; max-width: 700px; margin: 0 auto 1.2rem;">
    This is where I share my tournament ideas — four fingers of violence with a splash of garnish.
  </p>
  <ul class="post-list">
    {% assign recipes = site.library | where: "section", "recipes" %}
    {% for item in recipes %}
      <li>
        <a class="post-link" href="{{ item.url | relative_url }}">
          <span class="post-title">{{ item.title }}</span>
        </a>
      </li>
    {% endfor %}
  </ul>
</section>
