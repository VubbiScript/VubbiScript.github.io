---
layout: docs
docs_id: vectors
title: Documentation
description: Coordinates and directions - description of the blocks to work with coordinates and directions in VubbiScript
lang: en
subtitle: Coordinates and directions
slug: docs
---

TODO: TRANSLATION PENDING!

De "coördinaten en richtingen" categorie bevat blokjes om te rekenen met "coördinaten" (vectoren).

{% include blocks/DocsVectorBase.xml align="img-left" %}

Zo, heb je blokjes voor een hoop **simpele dingen met coördinaten & richtingen**:

  * een nieuwe coördinaat/richting maken of
  * de x,y,z van een coördinaat opvragen
  * de lengte van een coördinaat/richting berekenen

Voor richtingen kan je ook het blok met een aantal vooraf bepaalde richtingen gebruiken.

{% include blocks/DocsVectorRotate.xml align="img-left" %}

Het **"volgens rotatie"** blokje in de lijst laat je toe om te richtingen (zoals "omhoog", "omlaag", "links", "rechts", ...) te combineren met rotaties. Zo is de richting "links", "rechts", "omhoog", ... natuurlijk afhankelijk van hoe je gedraaid bent. Als je "de rechte kant van dit object" wilt, dan gebruik je dit blokje. Als je gewoon "rechts in de wereld" wilt, dan gebruik je dit blokje niet...


{% capture example %}

![Spaceship_forward.PNG]({{site.baseurl}}{% link assets/img/Spaceship_forward.PNG %}){:.img-right.img-sm}

**Voorbeeld** - "volgens rotatie" - een ruimteschip kan draaien en vliegt voorwaarts...

Als we het rechter pijltoetsje drukken moet het schip naar rechts draaien. Als we het linker pijltoetsje drukken naar links. En als we voorwaarts drukken moet vooruit bewegen. (in de "y-richting" van het ruimteschip)

De code ziet er uit als:
{% include blocks/DocsExampleSpaceShipMove.xml memforce="kracht" memtorque="draaikracht" %}
{% endcapture %}

<div class="exampleblock">{{example | markdownify}}</div>


{% include blocks/DocsVectorCalc.xml align="img-left" %}
Daarna hebben we allerhande wiskundige operaties om **richtingen te schalen** of **coördinaten (en/of richtingen) op te tellen**.

<div class="clear"></div>
&nbsp;
<div class="clear"></div>

{% include blocks/DocsVectorScreenSpaceTransform.xml align="img-left" %}
Als laatste hebben blokjes om te **rekenen met posities in pixels op het scherm**. Je kan deze met deze blokjes omrekenen naar posities in het level (=scene) of omgekeerd kan je berekenen waar iets in het level zich op het scherm bevindt. Om deze omrekening te doen moet je een camera meegeven. Zo kan je perfect meerdere camera's hebben als je een split-screen spel maakt.