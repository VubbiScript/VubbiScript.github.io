---
author: jeroenpenninck
comments: false
date: 2017-11-19 16:21:09+00:00
layout: page
title: Problemen & Unity bugs?
description: Als je Vubbi niet kan installeren of gebruiken is er misschien één van de volgende zaken mis.
lang: nl
slug: getting-started
---

Als je Vubbi niet kan installeren of gebruiken is er misschien één van de volgende zaken mis.

Nog een andere probleem? Laat het mij weten!


# Installatieproblemen




## Windows: het Vubbi installatiebestand opent een nieuw Unity venster en installeert niet in mijn project.


**Probleembeschrijving: **
Ik heb zonet Unity geïnstalleerd en een nieuw Unity project gemaakt. Daarna heb ik Vubbi gedownload maar als ik op dat bestand klikt opent een nieuw Unity venster zonder project. Mijn Unity project staat open, waarom installeert Vubbi niet correct?

**Oorzaak:**
Waarschijnlijk komt dit omdat Unity en je webbrowser niet onder dezelfde windows gebruiker draaien. Tijdens de installatie van Unity heb je het wachtwoord van de administrator moeten ingeven, daarna werd het installatieproces als de administrator gebruiker uitgevoerd. Het installatieproces start op het einde Unity als administrator. Alle andere programma's op je computer draaien echter nog als gewone gebruiker.

**Oplossing:**
Je zal Unity moeten afsluiten en opnieuw openen, daarna zal alles wel werken.
MAAR PAS OP: aangezien Unity geopend is met een adminstrator user zal je waarschijnlijk daarna niet meer aan je opgeslagen Unity project kunnen zonder het administrator wachtwoord!! Je zal dus opnieuw moeten beginnen.


## Unity vraagt mij om opnieuw in te loggen, maar het blijft maar hangen


**Oorzaak:**
Waarschijnlijk een firewall probleem van de locatie waar je je bevindt. Heb dit al voorgehad in de gebouwen van Odisee Aalst (voor CoderDojo Aalst).

**Oplossing:**

  1. Zet je internet af
  2. Open Unity opnieuw
  3. Klik op "manueel" en sla het bestand op op je bureaublad
  4. Zet je internet aan
  5. Klik op de link in het Unity venster om naar de website te gaan (unity.../manual)
  6. Log in en upload het bestand dat je net op je bureaublad hebt geplaatst
  7. Download de file die je krijgt van de Unity website en plaats hem ook op het bureaublad
  8. In unity, klik op de knop om die file te selecteren.
  9. Als alles goed is gegaan zie je nu de lijst met je projecten en kan je verder werken.

# Unity problemen




## Ik kan geen afbeeldingen naar Unity slepen.


**Probleembeschrijving:**
Ik kan geen afbeeldingen van mijn computer naar mijn Unity project slepen.

**Oorzaak:**
Er kunnen verschillende oorzaken zijn:
1. Let op dat je afbeeldingen opgeslagen zijn om je computer en niet meer in je een zip zitten.
2. Heb je zonet Unity geïnstalleerd? Dan kan het zijn dat je Unity draait als administrator maar alle andere programma's op je computer als normale gebruiker.
3. Als slepen in Unity ook niet werkt kan het zijn dat een programma op je computer niet goed samenwerkt met Unity.

**Oplossing:**
1. Unzip de map
2. Herstart Unity.
MAAR PAS OP: aangezien Unity geopend is met een adminstrator user zal je waarschijnlijk daarna niet meer aan je opgeslagen Unity project kunnen zonder het administrator wachtwoord!! Je zal dus opnieuw moeten beginnen.
3. Geen idee. Ik heb dit nog niet kunnen oplossen...
Er zijn manieren om te werken zonder slepen in Unity maar deze zijn zeer onhandig en omslachtig.


## Ik heb een 2D project gekozen, maar mijn afbeeldingen importeren niet als sprites.


Je kan de instelling handmatig wijzigen in:
Edit -> Project Settings -> Editor -> Default Behavior:2D
