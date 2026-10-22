---
layout: default
title: quotes
permalink: /quotes/
---

# quotes

<div class="grid-container">
  {% for q in site.data.quotes %}
    <div class="quote-card">
      <p>“{{ q.quote }}”</p>
      <div class="quote-author">— {{ q.author | downcase }}</div>
      {% if q.note %}
        <div style="margin-top: 8px;"><span class="meta-pill">{{ q.note | downcase }}</span></div>
      {% endif %}
    </div>
  {% endfor %}
</div>