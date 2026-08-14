---
layout: page
title: Projecten serious games
description: >-
  Projecten van Jan-Willem Manenschijn: Preludens, Jump Serious Games en
  Raccoon Serious Games — serious games, training en leerervaringen.
hero: true
hero_label: Projecten
hero_title: Projecten waar ik aan heb gewerkt
hero_text: Een selectie van organisaties en trajecten waarin serious games en conceptontwikkeling centraal stonden.
permalink: /projecten/
last_modified_at: 2026-08-14
image: https://creatievemaan.nl/wp-content/uploads/2024/12/Creative-concept-developer-Jan-willem-Manenschijn-de-creatieve-maan-outline-768x768.png
---

{% include answer.html
  text="Jan-Willem Manenschijn werkte als medeoprichter van Raccoon Serious Games (2018–2025), als conceptontwikkelaar bij Jump Serious Games (2024–heden) en als oprichter van Preludens. De rode draad: serious games en leerervaringen met maatschappelijke impact."
%}

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
