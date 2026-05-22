---
layout: page
title: Projecten
hero: true
hero_label: Projecten
hero_title: Projecten waar ik aan heb gewerkt
hero_text: Een selectie van organisaties en trajecten waarin serious games en conceptontwikkeling centraal stonden.
permalink: /projecten/
---

<div class="card-grid">
  {% assign projects_sorted = site.projects | sort: 'order' %}
  {% for project in projects_sorted %}
  <article class="card project-card">
    <div class="project-card__accent project-card__accent--{% cycle 'coral', 'mint' %}"></div>
    <p class="project-card__meta">{{ project.period }}</p>
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <p>{{ project.summary }}</p>
    {% if project.role %}
    <p><small><strong>Rol:</strong> {{ project.role }}</small></p>
    {% endif %}
    <a class="card__link" href="{{ project.url | relative_url }}">Lees het project →</a>
  </article>
  {% endfor %}
</div>
