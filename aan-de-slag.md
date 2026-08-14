---
layout: page
title: Trainingen, workshops en presentaties
description: >-
  Boek een training, workshop of serious game bij Jan-Willem Manenschijn.
  Onder meer laaggeletterdheid, Een eigen thuis, Reality Check, Vluchtelingenkamp
  en Juwelenroof.
permalink: /aan-de-slag/
last_modified_at: 2026-08-14
faq_key: aan_de_slag
service_id: trainingen
image: https://creatievemaan.nl/wp-content/uploads/2024/12/Creative-concept-developer-Jan-willem-Manenschijn-de-creatieve-maan-outline-768x768.png
---

{% include answer.html
  text="Bij Jan-Willem Manenschijn boek je standaard trainingen, workshops en serious games. Direct inzetbaar zijn onder meer de workshop laaggeletterdheid, Een eigen thuis, Reality Check, Vluchtelingenkamp, Juwelenroof, de training Spelend impact maken en de training Effectief en pragmatisch werken met AI. Prijs volgt in het eerste gesprek."
%}

<p class="lead">
  Dit zijn sessies die je kunt inplannen zonder een heel ontwerptraject.
  Zoek je maatwerk — een nieuw spel of een e-learning — kijk dan bij
  <a href="{{ '/serious-games/' | relative_url }}">serious games</a>.
</p>

<h2>Welke trainingen en workshops kan ik boeken?</h2>
<p class="section-intro">
  Standaardproducten. Duur, groepsgrootte en locatie stemmen we af;
  de kern van elke sessie staat vast.
</p>

{% assign eigen = site.data.trainingen | where_exp: "item", "item.group != 'jump'" | sort: 'order' %}
{% include boekbaar.html items=eigen %}

<h2>Welke spellen kan ik nog meer boeken?</h2>
<p class="section-intro">
  Drie fysieke serious games die ik begeleid: vertrouwen, multidisciplinair
  samenwerken, en overleg onder tijdsdruk.
</p>

{% assign jump_spellen = site.data.trainingen | where: "group", "jump" | sort: 'order' %}
{% include boekbaar.html items=jump_spellen %}
<p class="partner-note">
  Deze drie spellen begeleid ik in samenwerking met
  <a href="https://jumpseriousgames.nl" target="_blank" rel="noopener noreferrer">Jump Serious Games</a>.
</p>

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
