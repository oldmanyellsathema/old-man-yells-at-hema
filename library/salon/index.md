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
    Guest articles & community pieces. Be respectful—or I’ll forcibly (but lovingly) remove you.
  </p>

  {% assign items = site.salon | sort: 'date' | reverse %}
  {% if items and items != empty %}
    <ul class="post-list">
      {% for item in items %}
        <li>
          <a class="post-link" href="{{ item.url | relative_url }}">
            <span class="post-title">{{ item.title }}</span>
            {% if item.date %}
              <time class="post-date" datetime="{{ item.date | date_to_xmlschema }}">
                {{ item.date | date: "%b %d, %Y" }}
              </time>
            {% endif %}
          </a>
        </li>
      {% endfor %}
    </ul>
  {% else %}
    <p>No Salon entries yet. Add Markdown files to <code>_salon/</code>.</p>
  {% endif %}
</section>
