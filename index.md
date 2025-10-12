---
title: Idea Tree
layout: home
description: Idea Tree is a digital consultancy helping businesses grow through strategy, design, and technology.
intro_image: "images/illustrations/consulting-team.svg"
intro_image_absolute: true
intro_image_hide_on_mobile: true
show_call_box: true
---

# Welcome to Idea Tree 🌿

At **Idea Tree**, we help businesses thrive by turning ideas into actionable strategies. Our consultancy provides tailored solutions in **business growth**, **digital transformation**, and **online services** — helping you reach your goals with clarity and confidence.

Whether you’re launching a new venture or scaling an established brand, our team offers expert guidance every step of the way.

## Our Services

<ul class="services-list">
  {% for svc in site.services limit: site.home.limit_services %}
    <li class="service-card">
      <h3><a href="{{ svc.url | relative_url }}">{{ svc.title }}</a></h3>
      <p>{{ svc.excerpt | strip_html | truncate: 140 }}</p>
    </li>
  {% endfor %}
</ul>

<div class="hero-cta">
  <h2>Ready to grow?</h2>
  <p>Let’s talk about your next project.</p>
  <a class="btn" href="{{ "/contact/" | relative_url }}">Contact Us</a>
</div>
