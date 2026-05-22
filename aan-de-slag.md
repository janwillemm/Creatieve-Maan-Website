---
layout: page
title: Aan de slag
hero: true
hero_label: Aan de slag
hero_title: Spellen die je bij mij kunt spelen
hero_text: Concrete spellen die ik begeleid of heb ontwikkeld — plus maatwerk en sessies op jouw vraag.
permalink: /aan-de-slag/
---

<p class="lead">
  Hieronder vind je spellen die je direct kunt inzetten. Daaronder staan
  manieren waarop ik je verder kan helpen — van serious games tot escape rooms
  en maatwerk.
</p>

<h2>Spellen</h2>
<p class="section-intro">
  Deze spellen kun je bij mij boeken of via de genoemde links verkennen.
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

<h2>Ook mogelijk</h2>
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

<h2>Zo werken we samen</h2>
<ol>
  <li><strong>Kennismaking</strong> — We bespreken je vraag, doelgroep en gewenst effect.</li>
  <li><strong>Spelvorm</strong> — Bordspel, kaartspel, digitaal of escape room: wat past het beste?</li>
  <li><strong>Spelen &amp; reflecteren</strong> — Ik begeleid de sessie zodat de ervaring landt.</li>
  <li><strong>Vervolg</strong> — Optioneel: doorontwikkeling, training of maatwerkconcept.</li>
</ol>

<div class="cta-band" style="margin-top: 3rem;">
  <h2>Plan een gesprek</h2>
  <p>
    Benieuwd welk spel bij jouw team, school of organisatie past? Mail of bel — dan
    denken we vrijblijvend mee.
  </p>
  <a class="btn btn--primary" href="mailto:{{ site.email }}">{{ site.email }}</a>
</div>
