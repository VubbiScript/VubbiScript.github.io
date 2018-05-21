---
layout: docs
docs_id: move
title: Documentatie
description: Bewegen - beschrijving van de beweeg blokjes in VubbiScript
lang: nl
subtitle: Bewegen
slug: docs
---

De categorie Bewegen bevat vrij veel blokjes...

{% include blocks/DocsMovementMove.xml align="img-left" %}

De eerste groep blokjes gaat over de **positie van het object**. Je kan je positie in de wereld opvragen of je nieuwe positie in de wereld instellen. Je kan ook een klein beetje verschuiven met het "verspring ... meer naar ..." blokje. Merk op dat alle blokjes een "object blokje" bevatten dat standaard op "mijzelf" staat. Je kan dat blokje vervangen door een ander object dat je bijgehouden hebt in je geheugen om zo de positie van een ander object op te vragen of aan te passen. Merk op dat blokjes met een geel uiteinde "coördinaten" teruggeven. Het "positie van mijzelf" blokje heeft een geel uiteinde en ook het "x y z" blokje. Deze passen op alle plaatsen met een geel randje. Meer van deze gele blokjes en manieren om er mee te rekenen (zoals optellen) kunnen gevonden worden in de categorie "Coördinaten & richtingen".

{% include blocks/DocsMovementRotate.xml align="img-left" %}
Naast positie zijn er natuurlijk ook **blokjes voor rotatie**. Je kan de rotatie van jezelf opvragen of een bepaalde rotatie instellen. Het "rotatie van mijzelf" geeft een roos uiteinde. Zo'n roos uiteinde kan je opslaan als een rotatie om er daarna allerlei berekeningen op doen. Je kan het ook gewoon gebruiken in alle plaatsen met een roos randje. Blokjes om te rekenen met rotaties kan je vinden onder de categorie "Rotaties".

Als laatste hebben we **beweeg-blokjes in verband met physics**. Om deze te kunnen gebruiken heb je een Dynamic RigidBody nodig op je object!! Zo'n Dynamic RigidBody laat het object toe om te vallen, botsen, af te kaatsen van andere objecten, ... Het object heeft een snelheid en een draaisnelheid. Een wiel kan bijvoorbeeld van een helling rollen of een appel kan op de grond vallen. Deze blokjes laten je toe om de snelheden van de objecten op te vragen en aan te passen. Zo kan je een wiel bergop laten rollen of een appel laten springen...

{% include blocks/DocsMovementPhysicsMove.xml align="img-left" %}
{% include blocks/DocsMovementPhysicsRotate.xml align="img-left" %}

Op zo'n dynamic rigidbody kan je de "verspring" en "rotatie" blokjes ook gebruiken maar je doet dat meestal beter niet. Met het "verspring" blokje kan je bijvoorbeeld perfect in muren of andere objecten verspringen wat er zeer bizar kan gaan uitzien aangezien het object normaal botst met die objecten.

Merk op dat alle "coördinaten" die deze beweeg-blokjes gebruiken **in wereldcoördinaten** zijn. Als je dus wilt bewegen volgens "mijn rechts" en het object kan gedraaid zijn dan moet je eerst nog een ander blokje gebruiken, zie categorie "coördinaten en richtingen" voor het "volgens rotatie" blokje.