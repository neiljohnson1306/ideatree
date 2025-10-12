---
title: Team
layout: page
---

# Our Team

<ul>
  {% for member in site.team %}
    <li>
      <h3>{{ member.title }}{% if member.position %} - {{ member.position }}{% endif %}</h3>
      <p>{{ member.content | strip_html | truncate: 200 }}</p>
    </li>
  {% endfor %}
</ul>
