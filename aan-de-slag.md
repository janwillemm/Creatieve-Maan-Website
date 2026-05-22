---
layout: page
title: Aan de slag
hero: true
hero_label: Aan de slag
hero_title: Spellen die je bij mij kunt spelen
hero_text: Van serious game sessies tot escape rooms en maatwerk — samen kiezen we de vorm die past bij jouw vraag.
permalink: /aan-de-slag/
---

<p class="lead">
  Bij mij huur je geen standaard workshop van de plank. We kijken samen wat je
  wilt bereiken — en welk spel of welke ervaring daar het beste bij past.
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
    Benieuwd welk spel bij jouw team of organisatie past? Mail of bel — dan
    denken we vrijblijvend mee.
  </p>
  <a class="btn btn--primary" href="mailto:{{ site.email }}">{{ site.email }}</a>
</div>
