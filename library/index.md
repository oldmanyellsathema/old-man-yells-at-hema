---
layout: site
title: Salon
permalink: /library/salon/
---

<section class="deco-card">
  <span class="corner tl" aria-hidden="true"></span>
  <span class="corner tr" aria-hidden="true"></span>
  <span class="corner bl" aria-hidden="true"></span>
  <span class="corner br" aria-hidden="true"></span>

  <h2 class="invite-title" style="text-align:center;">Salon</h2>
  <p style="text-align:center; max-width:700px; margin:0 auto 1.2rem;">
    This is where others in the HEMA community can share their own discussions and thoughts.
    Please be respectful—or I’ll forcibly (but lovingly) remove you.
  </p>

  {% assign salon_posts = site.categories.Salon %}
  {% if salon_posts and salon_posts != empty %}
    <ul class="post-list">
      {% for post in salon_posts %}
        <li>
          <a class="post-link" href="{{ post.url | relative_url }}">
            <span class="post-title">{{ post.title }}</span>
            <time class="post-date" datetime="{{ post.date | date_to_xmlschema }}">
              {{ post.date | date: "%b %d, %Y" }}
            </time>
          </a>
        </li>
      {% endfor %}
    </ul>
  {% else %}
    <p>No Salon posts yet. Tag a post with <code>categories: [Salon]</code>.</p>
  {% endif %}
</section>
