---
layout: default
title: Salon
permalink: /library/Salon/
---

<section class="deco-card">
  <span class="corner tl"></span><span class="corner tr"></span>
  <span class="corner bl"></span><span class="corner br"></span>

  <h2 class="invite-title" style="text-align:center;">Gallery</h2>

  <p>
    This space is where other people in the HEMA world can get some articals or thoughts out. It's not a freewheeling space, comport yourself with dignity.  
  </p>
  <p>
    I want you all to feel free to share your thoughts if you have issue or suggestions or funny thoughts share!
  </p>

  <ul class="post-list">
    {% assign salon = site.library | where: "section", "salon" %}
    {% for item in salon %}
      <li>
        <a class="post-link" href="{{ item.url | relative_url }}">
          <span class="post-title">{{ item.title }}</span>
        </a>
      </li>
    {% endfor %}
  </ul>
</section>
