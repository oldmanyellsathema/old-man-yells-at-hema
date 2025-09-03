---
layout: gallery_index
title: Gallery
permalink: /gallery/
---

<section class="deco-card">
  <h1>{{ page.title }}</h1>

  {% assign coll = site[page.collection] %}
  {% if coll and coll.size > 0 %}
    {% assign items = coll | sort: "date" | reverse %}
    <ul class="post-list">
      {% for item in items %}
        <li class="post-excerpt">
          <a class="post-link" href="{{ item.url | relative_url }}">
            <span class="post-title">{{ item.title }}</span>
            {% if item.date %}
              <time class="post-date" datetime="{{ item.date | date_to_xmlschema }}">
                {{ item.date | date: "%b %-d, %Y" }}
              </time>
            {% endif %}
          </a>
          {% if item.excerpt %}<p>{{ item.excerpt | strip_html }}</p>{% endif %}
        </li>
      {% endfor %}
    </ul>
  {% else %}
    <p>No items yet.</p>
  {% endif %}
</section>
