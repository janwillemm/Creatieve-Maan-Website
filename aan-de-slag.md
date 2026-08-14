---
layout: page
title: Trainingen, workshops en presentaties
description: >-
  Boek een training of workshop bij Jan-Willem Manenschijn. Laaggeletterdheid,
  Een eigen thuis, Spelend impact maken en pragmatisch werken met AI.
hero: true
hero_label: Trainingen
hero_title: Inspirerende trainingen, workshops en presentaties
hero_text: Standaardproducten die je direct kunt boeken — op locatie of online, landelijk vanuit Houten.
permalink: /aan-de-slag/
last_modified_at: 2026-08-14
faq_key: aan_de_slag
service_id: trainingen
image: https://creatievemaan.nl/wp-content/uploads/2024/12/Creative-concept-developer-Jan-willem-Manenschijn-de-creatieve-maan-outline-768x768.png
---

{% include answer.html
  text="Bij Jan-Willem Manenschijn boek je standaard trainingen, workshops en presentaties. Direct inzetbaar zijn de workshop laaggeletterdheid, de workshop Een eigen thuis, de training Spelend impact maken en de training Effectief en pragmatisch werken met AI. Prijs volgt in het eerste gesprek."
%}

<p class="lead">
  Dit zijn sessies die je kunt inplannen zonder een heel ontwerptraject.
  Zoek je maatwerk — een nieuw spel of een e-learning — kijk dan bij
  <a href="{{ '/serious-games/' | relative_url }}">serious games</a>.
</p>

<h2>Welke trainingen en workshops kan ik boeken?</h2>
<p class="section-intro">
  Vier standaardproducten. Duur, groepsgrootte en locatie stemmen we af;
  de kern van elke sessie staat vast.
</p>

<div class="game-list game-list--featured">
  {% assign items = site.data.trainingen | sort: 'order' %}
  {% for item in items %}
  <article class="game-item game-item--featured">
    <span class="game-item__emoji" aria-hidden="true">{{ item.emoji }}</span>
    <div>
      <p class="game-item__type">{{ item.type }}{% if item.audience %} · {{ item.audience }}{% endif %}</p>
      <h3>{{ item.title }}</h3>
      <p>{{ item.description }}</p>
      {% if item.duration %}
      <p class="game-item__type">Duur: {{ item.duration }}</p>
      {% endif %}
      {% if item.highlights %}
      <ul class="game-item__highlights">
        {% for point in item.highlights %}
        <li>{{ point }}</li>
        {% endfor %}
      </ul>
      {% endif %}
      {% if item.links %}
      <p class="game-item__links">
        {% for lnk in item.links %}
        <a href="{{ lnk.url | relative_url }}"{% unless lnk.internal %} target="_blank" rel="noopener noreferrer"{% endunless %}>{{ lnk.label }} →</a>{% unless forloop.last %}<span class="game-item__sep">·</span>{% endunless %}
        {% endfor %}
      </p>
      {% endif %}
    </div>
  </article>
  {% endfor %}
</div>

<h2>Wat kost een training of workshop?</h2>
<p>
  De prijs hangt af van groepsgrootte, locatie, duur en of je een bestaande
  vorm of een lichte aanpassing wilt. In het eerste gesprek krijg je een
  duidelijk bedrag — geen open offerteproces.
</p>
<p>
  Presentaties over serious games, leren door te spelen of pragmatisch werken
  met AI zijn ook mogelijk. Zeg wat de setting is; dan volgt een voorstel.
</p>

<h2>Hoe boek ik een sessie?</h2>
<ol>
  <li><strong>Mail of bel</strong> — welk product, welke datumrange, hoeveel mensen.</li>
  <li><strong>Afstemming</strong> — duur, locatie of online, wat je nodig hebt op zaal.</li>
  <li><strong>Bevestiging</strong> — heldere prijs en wat ik meeneem of voorbereid.</li>
  <li><strong>Sessie</strong> — spelen of oefenen, daarna reflectie zodat het landt.</li>
</ol>

{% include faq.html key="aan_de_slag" %}

<div class="cta-band" style="margin-top: 3rem;">
  <h2>Plan een sessie</h2>
  <p>
    Benieuwd welke training of workshop bij jouw team, school of organisatie
    past? Mail of bel — dan denken we vrijblijvend mee.
  </p>
  <a class="btn btn--primary" href="mailto:{{ site.email }}">{{ site.email }}</a>
</div>
