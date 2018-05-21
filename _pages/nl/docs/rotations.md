---
layout: docs
docs_id: rotations
title: Documentatie
description: Rotaties - beschrijving van de blokjes om te werken met rotaties in VubbiScript
lang: nl
subtitle: Rotaties
slug: docs
---

De volgende blokjes werken met "rotaties". Deze rotaties kunnen gebruikt worden op alle plaatsen met een roze randje en alle blokjes met een roos uiteinde geven rotaties terug.

{% include blocks/DocsRotateIdentity.xml align="img-left" %}
Het eerste blokje is **"niet gedraaid"**. Dit blokje geeft een rotatie terug maar de rotatie doet eigenlijk niets. Je kan dit blokje gebruiken als de rotatie van een object wil terugzetten. Je kan deze rotatie op vele andere manieren ook maken, bijvoorbeeld door "0° (2D)" te gebruiken (zie volgend blokje).

{% include blocks/DocsRotate2D.xml align="img-left" %}
Met het volgende blokje **kan je elke 2D rotatie voorstellen** als je de hoek weet. Negatieve getallen zijn ook toegestaan en stellen de omgekeerde rotatie voor.

{% include blocks/DocsRotate2DGetAngle.xml align="img-left" %}
Het "2D richting (0°-360°) van" doet het omgekeerde van het net vermelde "_... _° (2D)" blokje. Het **geeft de 2D hoek terug** van een willekeurig rotatie object. Zo kan je perfect de hoek opvragen van "rotatie van mijzelf" of van elke andere rotatie. Merk op dat je altijd een positief getal terugkrijgt.

{% include blocks/DocsRotate3D.xml align="img-left" %}
Het blokje "getal ° rond vector" is een **uitbreiding van het 2D rotatie blokje**. Als je de richting op "achterwaarts (diepte)" laat staan, dan doet dit hetzelfde als het vorige blokje. Je kan de richting ook aanpassen. De richting stelt de lijn voor waarrond je draait.

{% include blocks/DocsRotateAdd.xml align="img-left" %}
"draai eerst ... en dan ..." laat je toe **om rotaties op te tellen**. Zo kan je eerst 10° draaien en dan 15° of kan je zelfs 2D rotaties met andere (3D) rotaties optellen.

{% include blocks/DocsRotateInvert.xml align="img-left" %}
Het "omgekeerde draaiing van" blokje **geeft de omgekeerde draaiing terug** van de rotatie die je meegeeft. Voor 2D draaiing kan je dit natuurlijk ook makkelijk doen via de hoek. Als je een draaiing van 37° hebt zal je een draaiing van -37° terugkrijgen.

{% include blocks/DocsRotatePointTowards.xml align="img-left" %}
Het laatste blokje ziet er zeer complex uit maar is zeer nuttig. Dit blokje **laat je toe om een object te laten kijken/wijzen naar een ander object** (werkt in 2D en 3D). Zo zou je een kanon altijd kunnen laten mikken naar een vijand of naar de muis... Als je het blokje in 2D wilt gebruiken gebruik je "achterwaarts" als "as" (zoals bij de 2D draaiing hierboven).
