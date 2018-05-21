---
author: jeroenpenninck
comments: false
date: 2017-05-12 19:59:07+00:00
layout: page
title: Roadmap
description: Wat is er nog gepland voor Vubbi?
lang: nl
slug: docs
---

Wat is er nog gepland voor Vubbi?  Zeer veel... een overzicht:

Laat me zeker weten wat volgens jou belangrijk is!


### Blokjes voor:

  * instellingen doorgeven naar verschillende levels (nuttig voor menu's te maken)
  * geluidjes afspelen!
  * <del>te werken met de muispositie (zodat je kan slepen enzo) - raytracing vanaf cursor?</del>
**✓** _beschikbaar in versie 0.4 (muis positie & scherm positie blokjes)_
  * <del>3D physics (nu worden enkel 2D physics ondersteund)</del>
**✓ ** _beschikbaar in versie 0.4 (alle blokjes hebben 3D switch)_
  * te werken met andere invoer zoals joysticks, touch? ...
  * objecten te verbergen of doorzichtig te maken of te verkleuren
  * ondersteuning voor 3D tekst (nu kan je enkel 2D tekst aanpassen)
  * verschil tussen lokale/wereld positie van een object
  * FPS muis beweging (met gelockte muis)
  * meer raycast blokjes (ContactFilter2D, LayerMask, OverlapCircle, SphereCast)
  * Navmesh agent blokjes
  * ...

### Features:

  * open meerdere Unity projecten met Vubbi tegelijk. (nu kan je Vubbi maar 1 keer tegelijk openen)
  * knop om tijdelijke variabelen te verbergen in Unity
  * tooltips voor alle blokjes + duidelijker aangeven welke componenten je nodig hebt (RigidBody2D, UI.Text, ...)
=> Er is nu wel al [Documentatie](https://vubbiscript.wordpress.com/docs/)!
  * andere talen ondersteunen (niet enkel nederlands)
  * items omhoog en omlaag verplaatsen in het geheugen
  * tips in Vubbi?

### Documentatie...

  * Sushi cards voor eenvoudige dingen?
    * Hoe laat ik de camera de speler volgen in 2D?
    * Hoe maak ik een object dat kapotgaat als het te hard botst?
    * Hoe detecteer ik als de speler in een bepaald gebied komt?
    * Hoe maak ik een (2D?) auto met wielen die kunnen draaien?
    * Hoe hou ik score bij?
    * Hoe spawn ik nieuwe objecten?
    * Hoe laat ik iets ontploffen als het botst?
    * Hoe werk je met sprite animaties? (geen code)
    * Hoe werk je met UI?
  * Meer voorbeeldprojecten...
    * Asteroids?
    * Platformer?
    * Angry Birds?
    * ...


### Blokjes voor veelgebruikte combinaties (kan nu al, maar meer blokjes nodig):

Voor veelgebruikte operaties wil ik aparte blokjes maken.

  * start bewegen in willekeurige richting met snelheid
NU:
![Block_start_random.PNG](https://vubbiscript.files.wordpress.com/2017/05/block_start_random.png)
DOEL: 1 blokje?
  * <del>versnel tot snelheid (...)</del>
<del> Probleem is dat je waarschijnlijk niet door muren wilt kunnen gaan...</del>
<del> NU: moet je zelf iets doen met "geef mijzelf duw in richting"</del>
**✓** _beschikbaar in versie 0.4 (zet snelheid blokjes)_
  * beweeg mijzelf voorwaarts (lokaal assenstelsel)
NU:
![Block_move_forwards_local.PNG](https://vubbiscript.files.wordpress.com/2017/05/block_move_forwards_local.png)
DOEL: blokje "volgens rotatie" & "rotatie van mijzelf" niet meer nodig. In de plaats daarvan een dropdown met "mijn/wereld richting" (+ tegenover "ouder"?)
  * willekeurige positie in straal van ... rond ...!
  * maak kopie van ... op positie met rotatie
NU:
![Block_make_clone2.PNG](https://vubbiscript.files.wordpress.com/2017/05/block_make_clone2.png)
DOEL: één blokje die deze drie operaties combineert + geen geheugen nodig. (andere optie blijft wel bestaan)
  * zet x/y/z snelheid blokje (of blokjes om enkel de x/y/z/xy/... van een vector over te houden?) (nuttig voor: enkel horizontaal bewegen maar valsnelheid behouden! - nu onhandig)
  * zet x/y/z positie blokje (nuttig voor: camera volg script => z wil je niet aanpassen - nu onhandig)
  * draai "richt naar" blokje - kan eenvoudiger dan hoe het nu is...

### En nog later...

  * pen blokjes (?)
  * lijsten, dictionaries en lussen (?)
=> hoe vermijd je accidental infinite loops?
  * berichten sturen met extra informatie (stuur een dictionary??)
  * player controller component ondersteunen (?)
  * Coroutine lokale variablen
  * Particle System blokjes (?)
  * Procedures?
  * Meer physics blokjes? sleep? make joints?
  * Percent van rotatie? (slerp?)

### Bugs?

  * <del>rechterklik is onhandig... => browsermenu opent soms
</del>**✓ ** _gefixed in versie 0.4_
  * "datatypes" worden niet vertaald... "String" zou "Tekst" moeten worden, enz...
  * Berichtjes "score+1" en "score+5" worden met elkaar verward als ze omgezet worden naar methodenamen. (Worden omgezet naar dezelfde methodenaam)
  * <del>Volgorde van vermenigvuldigen na vermenigvuldigingen maakt wél uit in C# (en ik plaats geen haakjes in de veronderstelling dat vermenigvuldigen links-associatief is). Er was iets met rotaties en vectoren waarbij haakjes rond vermenigvuldigingen wel uitmaakten. (weet niet meer goed welke situatie)</del>
**✓ ** _gefixed in versie 0.4_
  * 2 keer een script met dezelfde naam aanmaken zet een " 1" achter de naam. De spatie in de naam is echter ongeldig.
