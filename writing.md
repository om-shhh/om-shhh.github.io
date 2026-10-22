---
layout: default
title: writing
permalink: /writing/
---

# writing

<div class="grid-container">
  {% for essay in site.writing %}
    <a href="{{ essay.url | relative_url }}" class="card-link">
      <div class="card">
        <div>
          <h3>{{ essay.title | downcase }}</h3>
          <p>{{ essay.description }}</p>
        </div>
        <span class="meta-pill">{{ essay.date | date: "%b %Y" | downcase }}</span>
      </div>
    </a>
  {% endfor %}
</div>