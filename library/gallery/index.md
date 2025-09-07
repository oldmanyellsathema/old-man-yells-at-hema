---
layout: default
title: Gallery
permalink: /library/gallery/
---

<section class="deco-card">
  <span class="corner tl"></span><span class="corner tr"></span>
  <span class="corner bl"></span><span class="corner br"></span>
  <h2 class="invite-title" style="text-align:center;">Gallery</h2>

   <p>
    This is where I drop images—some end up here, some end up on Instagram. 
    They don’t always overlap, so if you actually care you might want to check both.  
  </p>
  <p>
    Is all this art “great”? …no. Is it good? Maybe. Is it odd? Also maybe.  
    Look, art is the one spot where it’s not about what I think—it’s about what you do with it. 
    You can take it or leave it. Actually, don’t take it. It’s mine. But you can look.  
  </p>
</section>

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
