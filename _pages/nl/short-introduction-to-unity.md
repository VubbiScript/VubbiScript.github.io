---
author: jeroenpenninck
comments: false
date: 2017-05-12 19:16:30+00:00
layout: page
title: Korte introductie tot Unity
description: Wat je moet weten om te starten in Unity?
lang: nl
slug: getting-started
---

Wat je moet weten om te starten in Unity?


### Basis objecten in Unity:


**Sprites en Textures:** gewoon afbeeldingen. Kunnen dus geen scripts bevatten.

**Scripts:** doen niets op zichzelf... Je moet ze eerst toevoegen aan een object!

**Objecten:** kunnen allerhande componenten en scripts bevatten en doen iets!
=> Tip: één manier om een object te maken is door een sprite (afbeelding) naar het hiërarchievenster te slepen...
=> Tip: je kan objecten bewerken in het Inspector venster als je ze geselecteerd hebt

**Prefabs:** zijn herbruikbare objecten (zeer nuttig)
Je maakt deze aan door een Object van de hiërarchievenster naar het projectvenster te slepen
Voorbeelden:

  * de speler die je wilt hergebruiken in alle levels
  * een kogel die je meerdere keren wilt aanmaken
  * een vijand die meerdere keren in dezelfde Scene voorkomt...

_**Waarom?**_ Je kan de vijand ook meerdere keren kopiëren, maar dan moet je ze allemaal aanpassen als je iets wijzigt

### Wat kan je toevoegen aan een object?

**Scripts:** natuurlijk**!** Als je een script gemaakt hebt met Vubbi kan je dit toevoegen aan een object!

**SpriteRenderer of MeshRenderer:** zodat je het object ook echt kan zien...
=> Een object zelf is onzichtbaar, maar je kan er een afbeelding aan toevoegen met een SpriteRenderer

**RigidBody2D (zeer nuttig):** als je object (1)beweegt en moet (2)botsen met andere objecten heb je een RigidBody component nodig!
Heeft veel opties:

  * hoe sterk de zwaartekracht er op werkt... (gravity scale) => 0 in de ruimte!
  * hoe sterk het terugkaatst van andere objecten?  (0% - 100%)
  * hoe snel het vertraagt als je er geen krachten op uitvoert (linear drag)
  * je kan zorgen dat het niet kan draaien maar wel bewegen en botsen...
  * kan het object verplaatst worden doordat een ander object ertegen botst?
Nee? dan zet je het best "kinematic"
  * ...

**Box/Circle/...Collider2D:** duid aan wat de randen van je objecten zijn waarmee je botst. Als iets moet kunnen (1)botsen tegen dit object heb je dit nodig!
Muren hebben dit nodig en alle objecten met een RigidBody2D normaal ook!
Waarom? Wel, weet je nog dat objecten onzichtbaar kunnen zijn?

**Enz**...

### Vensters in Unity:

**Project venster:** hier staan al je afbeeldingen, scripts, herbruikbare objecten, ...
Alle dingen die je over **_meerdere levels (=Scenes)_** nodig kan hebben komen hier!

**Hierarchie venster:** hier staan alle objecten die in het **_huidige level_** zitten (=Scene)

**Scene venster:** hier zie je het _**huidige level**_ (=Scene)

**Game venster:** als je het _**huidige level**_ speelt zie je dat hier

**Inspector venster:** hier kan je aanpassen wat je _**geselecteerd**_ hebt (en bijvoorbeeld scripts toevoegen)


### Extra Tips:

**Vergeet niet om het spel te stoppen voor je aanpassingen doet!!**
Terwijl je het spel speelt kan je alles aanpassen in de Scene... maar als je het spel stopt zijn al die wijzigingen weer weg! Je stopt dus best het spel voor je iets aanpast!
