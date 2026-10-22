---
layout: default
title: Writing
permalink: /writing/
---

# Writing

Click any essay tile below to read the full piece:

<div class="grid-container">
  {% for essay in site.writing %}
    <a href="{{ essay.url | relative_url }}" class="card-link">
      <div class="card">
        <h3>{{ essay.title }}</h3>
        <p>{{ essay.description }}</p>
        <small style="color: #888;">{{ essay.date | date: "%b %Y" }}</small>
      </div>
    </a>
  {% endfor %}
</div>