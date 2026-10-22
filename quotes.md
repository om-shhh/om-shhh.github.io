---
layout: default
title: Quotes
permalink: /quotes/
---

# Selected Quotes

<div class="grid-container">
  {% for q in site.data.quotes %}
    <div class="quote-card">
      <p>"{{ q.quote }}"</p>
      <div class="quote-author">— {{ q.author }}</div>
      {% if q.note %}
        <small style="color: #888;">Note: {{ q.note }}</small>
      {% endif %}
    </div>
  {% endfor %}
</div>