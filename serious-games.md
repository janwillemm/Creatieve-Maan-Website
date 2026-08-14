---
layout: page
title: Serious games en e-learnings
description: >-
  Maatwerk serious games en e-learnings van Jan-Willem Manenschijn. Vast
  proces, duidelijke prijs, één aanspreekpunt. Vanuit Houten, landelijk.
hero: true
hero_label: Serious games
hero_title: Fysieke & digitale ervaringen die je bijblijven
hero_text: Maatwerk serious games en e-learnings — met een vast proces, een duidelijke prijs en één aanspreekpunt.
permalink: /serious-games/
last_modified_at: 2026-08-14
faq_key: serious_games
service_id: serious-games
image: https://creatievemaan.nl/wp-content/uploads/2024/12/Creative-concept-developer-Jan-willem-Manenschijn-de-creatieve-maan-outline-768x768.png
howto:
  name: Samenwerken aan een serious game of e-learning
  description: Vast proces van kennismaking tot overdracht met Jan-Willem Manenschijn.
  steps:
    - name: Kennismaking
      text: We bespreken je vraag, doelgroep en gewenst effect. Eén aanspreekpunt vanaf het eerste gesprek.
    - name: Vraag scherp
      text: Welk gedrag of gesprek moet er ná afloop anders zijn? Daarop volgt de vorm, niet andersom.
    - name: Concept en prototype
      text: Een speelbaar concept dat je kunt voelen — bord, escape, digitaal of e-learning.
    - name: Testen
      text: Spelen met echte mensen uit de doelgroep. Feedback landt in het ontwerp.
    - name: Productie
      text: Uitwerking met een team van creatieve zzp’ers en partnerorganisaties.
    - name: Overdracht
      text: Oplevering, handleiding of begeleiding — zodat de ervaring blijft werken zonder mij.
---

{% include answer.html
  text="Jan-Willem Manenschijn ontwerpt maatwerk serious games en e-learnings: fysieke en digitale ervaringen die complexe vraagstukken invoelbaar maken. Je werkt met één aanspreekpunt, een vast proces en een duidelijke prijs na de intake — met 10+ jaar ervaring en een netwerk van makers."
%}

<p class="lead">
  Een presentatie legt uit. Een serious game laat mensen het zelf meemaken.
  Dat is het verschil: ná de sessie kijken, praten of handelen ze anders —
  niet alleen weten ze meer.
  <a href="{{ '/wat-is-een-serious-game/' | relative_url }}">Wat is een serious game?</a>
</p>

<h2>Wat krijg je bij een maatwerk serious game?</h2>
<p class="section-intro">
  Een ervaring die past bij jullie vraag, doelgroep en setting. De vorm volgt
  het doel: soms een bordspel aan één tafel, soms een escape voor vijftig
  mensen, soms een e-learning in jullie eigen leeromgeving.
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

<p>
  Digitale leerervaringen met stripverhalen en MicroGames lopen via
  <a href="{{ '/preludens/' | relative_url }}">Preludens</a>: Short Stories
  en volledige MicroGame Stories, inzetbaar in jullie eigen leeromgeving.
</p>

<h2>Waarom dit traject zo insteken?</h2>
<div class="card-grid proof-grid">
  <article class="card">
    <h3>Vast proces</h3>
    <p>Zes stappen van kennismaking tot overdracht. Je weet waar je aan toe bent.</p>
  </article>
  <article class="card">
    <h3>Duidelijke prijs</h3>
    <p>Vaste prijs na intake. Geen open einde, geen uurtje-factuurtje.</p>
  </article>
  <article class="card">
    <h3>Eén aanspreekpunt</h3>
    <p>Je belt of mailt mij. Ik houd het overzicht, ook als er meer makers meewerken.</p>
  </article>
  <article class="card">
    <h3>10+ jaar en een netwerk</h3>
    <p>Ervaring sinds 2015, plus creatieve zzp’ers en organisaties die het product scherp maken.</p>
  </article>
</div>

<h2>Hoe werkt het proces?</h2>
<p>
  De samenwerking start met een kort gesprek. Daarna maken we de vraag scherp,
  prototypen we, testen we met echte mensen en produceren we met het netwerk.
</p>
{% include proces.html %}

<h2>Wat kost een serious game of e-learning?</h2>
<p>
  Prijzen hangen af van vorm en omvang. Voor e-learnings via Preludens geldt
  een vaste indicatie. Voor fysiek of digitaal maatwerk volgt een vaste prijs
  na de intake — als de scope helder is.
</p>
<table class="compare-table">
  <caption>Indicatie investering serious games en e-learnings</caption>
  <thead>
    <tr>
      <th>Vorm</th>
      <th>Wat je krijgt</th>
      <th>Indicatie</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Short Story</td>
      <td>Compacte dilemma-interventie (2–5 keuzes) in jullie leeromgeving</td>
      <td>Circa € 1.500 per verhaal</td>
    </tr>
    <tr>
      <td>MicroGame Story</td>
      <td>Volledige storyline: circa 7 hoofdstukken en 5 MicroGames</td>
      <td>Circa € 10.000 per storyline</td>
    </tr>
    <tr>
      <td>Fysiek of digitaal maatwerk</td>
      <td>Bordspel, escape, digitale game of hybride ervaring</td>
      <td>Vaste prijs na intake</td>
    </tr>
  </tbody>
</table>
<p>
  Meer over de e-learningproducten staat op
  <a href="{{ '/preludens/' | relative_url }}">Preludens</a>.
</p>

<h2>Welke voorbeelden zijn er?</h2>
<p class="section-intro">
  Onder meer PWN, een AI-game, de ervaring rond laaggeletterdheid en het
  bordspel Een eigen thuis.
</p>
{% include cases.html dienst="serious-games" %}

{% include faq.html key="serious_games" %}

<div class="cta-band" style="margin-top: 3rem;">
  <h2>Plan een gesprek</h2>
  <p>
    Heb je een thema of leerdoel dat mensen moeten voelen, niet alleen horen?
    Mail of bel — dan denken we vrijblijvend mee over vorm en investering.
  </p>
  <a class="btn btn--primary" href="mailto:{{ site.email }}">{{ site.email }}</a>
</div>
