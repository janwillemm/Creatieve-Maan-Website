---
layout: page
title: Serious games boeken
description: >-
  Boek een serious game, workshop of maatwerksessie bij Jan-Willem Manenschijn.
  Onder meer laaggeletterdheid, Een eigen thuis, Preludens en Woordenweide.
hero: true
hero_label: Aan de slag
hero_title: Spellen die je bij mij kunt spelen
hero_text: Concrete spellen die ik begeleid of heb ontwikkeld — plus maatwerk en sessies op jouw vraag.
permalink: /aan-de-slag/
last_modified_at: 2026-08-14
faq_key: aan_de_slag
image: https://creatievemaan.nl/wp-content/uploads/2024/12/Creative-concept-developer-Jan-willem-Manenschijn-de-creatieve-maan-outline-768x768.png
howto:
  name: Samenwerken aan een serious game
  description: Van kennismaking tot speelbare sessie met Jan-Willem Manenschijn.
  steps:
    - name: Kennismaking
      text: We bespreken je vraag, doelgroep en gewenst effect.
    - name: Spelvorm
      text: Bordspel, kaartspel, digitaal of escape room — wat past het beste?
    - name: Spelen en reflecteren
      text: Jan-Willem begeleidt de sessie zodat de ervaring landt.
    - name: Vervolg
      text: Optioneel doorontwikkeling, training of een maatwerkconcept.
---

{% include answer.html
  text="Bij Jan-Willem Manenschijn boek je bestaande serious games of laat je maatwerk ontwerpen. Direct inzetbaar zijn onder meer de workshop laaggeletterdheid, het bordspel Een eigen thuis, Preludens-leerervaringen en Woordenweide. Sessie op locatie of online, landelijk vanuit Houten."
%}

<p class="lead">
  Hieronder staan spellen die je direct kunt inzetten. Daaronder manieren waarop
  ik je verder help — van serious games tot escape rooms en maatwerk.
  Nieuw met het onderwerp?
  <a href="{{ '/wat-is-een-serious-game/' | relative_url }}">Wat is een serious game?</a>
</p>

<h2>Welke serious games kan ik boeken?</h2>
<p class="section-intro">
  Deze spellen kun je bij mij boeken of via de genoemde links verkennen.
  Ik was bij elk van deze vormen betrokken als ontwerper, mede-ontwikkelaar of begeleider.
</p>

<div class="game-list game-list--featured">
  {% assign spellen = site.data.spellen | sort: 'order' %}
  {% for spel in spellen %}
  <article class="game-item game-item--featured">
    <span class="game-item__emoji" aria-hidden="true">{{ spel.emoji }}</span>
    <div>
      <p class="game-item__type">{{ spel.type }}{% if spel.audience %} · {{ spel.audience }}{% endif %}</p>
      <h3>{{ spel.title }}</h3>
      <p>{{ spel.description }}</p>
      {% if spel.highlights %}
      <ul class="game-item__highlights">
        {% for item in spel.highlights %}
        <li>{{ item }}</li>
        {% endfor %}
      </ul>
      {% endif %}
      {% if spel.links or spel.link or spel.contact %}
      <p class="game-item__links">
        {% if spel.links %}
          {% for lnk in spel.links %}
          <a href="{{ lnk.url | relative_url }}"{% unless lnk.internal %} target="_blank" rel="noopener noreferrer"{% endunless %}>{{ lnk.label }} →</a>{% unless forloop.last %}<span class="game-item__sep">·</span>{% endunless %}
          {% endfor %}
        {% elsif spel.link %}
        <a href="{{ spel.link | relative_url }}"{% unless spel.internal %} target="_blank" rel="noopener noreferrer"{% endunless %}>{{ spel.link_label | default: "Meer informatie" }} →</a>
        {% endif %}
        {% if spel.contact %}
        {% if spel.links or spel.link %}<span class="game-item__sep">·</span>{% endif %}
        <a href="mailto:{{ spel.contact }}">{{ spel.contact }}</a>
        {% endif %}
      </p>
      {% endif %}
    </div>
  </article>
  {% endfor %}
</div>

<h2>Welke maatwerkvormen zijn nog meer mogelijk?</h2>
<p class="section-intro">
  Past geen standaardspel? Dan kijken we samen welke vorm het beste werkt.
</p>

<div class="game-list">
  {% for game in site.data.games %}
  <article class="game-item">
    <span class="game-item__emoji" aria-hidden="true">{{ game.emoji }}</span>
    <div>
      <p class="game-item__type">{{ game.type }}</p>
      <h3>{{ game.title }}</h3>
      <p>{{ game.description }}</p>
    </div>
  </article>
  {% endfor %}
</div>

<h2>Hoe werken we samen aan een serious game?</h2>
<p>
  De samenwerking start met een kort gesprek. Daarna kiezen we de vorm, spelen
  we, en zorgen we dat de ervaring landt in jullie praktijk.
</p>
<ol>
  <li><strong>Kennismaking</strong> — We bespreken je vraag, doelgroep en gewenst effect.</li>
  <li><strong>Spelvorm</strong> — Bordspel, kaartspel, digitaal of escape room: wat past het beste?</li>
  <li><strong>Spelen &amp; reflecteren</strong> — Ik begeleid de sessie zodat de ervaring landt.</li>
  <li><strong>Vervolg</strong> — Optioneel: doorontwikkeling, training of maatwerkconcept.</li>
</ol>

{% include faq.html key="aan_de_slag" %}

<div class="cta-band" style="margin-top: 3rem;">
  <h2>Plan een gesprek</h2>
  <p>
    Benieuwd welk spel bij jouw team, school of organisatie past? Mail of bel — dan
    denken we vrijblijvend mee.
  </p>
  <a class="btn btn--primary" href="mailto:{{ site.email }}">{{ site.email }}</a>
</div>
