---
layout: docs
docs_id: detect
title: Documentation
description: Detect - description of the detection blocks in VubbiScript
lang: en
subtitle: Detect
slug: docs
---

TODO: TRANSLATION PENDING!

De categorie waarnemen bevat (nog) niet veel blokjes, maar deze kunnen zeer nuttig zijn.

{% include blocks/DocsDetectKey.xml align="img-left" %}

**"knop ... net ingedrukt"** is een blokje dat je veel zal gebruiken. Het geeft "waar" terug als die knop net was ingedrukt door de speler. Het is de bedoeling dat je dit elke frame oproept om te controleren of de speler iets doet. (Zie "elke frame opnieuw" blokje of de blokjes in categorie "Tijd")

Je kan ook **"knop ... nog steeds ingedrukt"** als je bijvoorbeeld wilt blijven versnellen zolang de speler een knop ingedrukt houdt.

{% include blocks/DocsDetectKey.xml align="img-left" key="Mouse0" %}

Dit blokje werkt ook met muisknoppen. Met **"knop Eerste muisknop net ingedrukt"** kan je testen of de gebruiker geklikt heeft. Het maakt hier niet uit waar hij klikt. Als je enkel wilt weten als de gebruiker op een knop geklikt heeft gebruik je beter de "wanneer een muisknop op ... mij" in categorie "Gebeurtenissen".

{% include blocks/DocsDetectRaycast.xml align="img-left" %}

Daarnaast is er ook een zeer complex blokje **"schiet een lazer ..."** waarmee je kan controleren of er zich een obstakel in een bepaalde richting bevindt. Je kan een lazer naar beneden schieten om te weten hoe ver je van de grond bent. Je kan een lazer naar recht schieten om te weten of er een muur is...

{% include blocks/DocsDetectMouseScene2D.xml align="img-left" %}

Met "positie van muis in scene met z=0" weet je waar de muis zich in het level bevindt. Je kan met dit blokje dus kanonnen of andere zaken richten met de muis. Of je kan gewoon de speler de muis laten volgen. Dit blokje werkt best in 2D maar kan ook nuttig zijn in 3D.

{% include blocks/DocsDetectMouseScreen.xml align="img-left" %}

Soms wil je echter niet weten waar de muis in het level is maar eerder waar ergens de muis op het scherm is. Dat kan je met deze blokjes. Zo kan je bijvoorbeeld de camera naar rechts bewegen als de muis aan de rechterzijde van het scherm is.