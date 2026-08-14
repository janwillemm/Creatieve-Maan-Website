---
layout: page
title: Projecten serious games en tools
description: >-
  Projecten van Jan-Willem Manenschijn: serious games, digitale tools,
  trainingen, Preludens, Jump en Raccoon Serious Games.
hero: true
hero_label: Projecten
hero_title: Projecten waar ik aan heb gewerkt
hero_text: Cases bij de drie diensten, plus eerdere organisaties waarin serious games en conceptontwikkeling centraal stonden.
permalink: /projecten/
last_modified_at: 2026-08-14
image: https://creatievemaan.nl/wp-content/uploads/2024/12/Creative-concept-developer-Jan-willem-Manenschijn-de-creatieve-maan-outline-768x768.png
---

{% include answer.html
  text="Jan-Willem Manenschijn werkt aan serious games, digitale tools en trainingen. Cases zijn onder meer PWN, de AI Game, laaggeletterdheid, Een eigen thuis, de EMDR-toolkit en deze website. Eerder was hij medeoprichter van Raccoon Serious Games en werkt hij bij Jump Serious Games."
%}

<h2>Serious games</h2>
<p class="section-intro">
  Maatwerkervaringen en e-learnings.
  <a href="{{ '/serious-games/' | relative_url }}">Meer over deze dienst →</a>
</p>
{% include cases.html dienst="serious-games" limit=12 %}

<h2>Tools</h2>
<p class="section-intro">
  Digitale hulpmiddelen, vaak met AI.
  <a href="{{ '/tools/' | relative_url }}">Meer over deze dienst →</a>
</p>
{% include cases.html dienst="tools" limit=12 %}

<h2>Samenwerkingen en eerder werk</h2>
<p class="section-intro">
  Organisaties en periodes die de achtergrond vormen — geen losse producten
  om te boeken.
</p>
<div class="card-grid">
  {% assign background = site.projects | where_exp: "p", "p.dienst == nil or p.dienst == empty" | sort: "order" %}
  {% for project in background %}
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
