---
author: jeroenpenninck
comments: false
date: 2017-05-08 20:27:23+00:00
layout: page
title: Release info en oudere versies
description: Wat is er gewijzigd in vorige versies van VubbiScript?
lang: nl
slug: docs
---

### Versie 0.5.0 (01 sep 2018)

  * Introductie van Engelse versie! Vubbi is vanaf nu beschikbaar in zowel Engels als Nederlands.
  * Introductie van knopjes om de zichtbaarheid van geheugenvelden aan te passen. Zo kan je interne variablen verbergen in Unity.
  * Herwerkte website. De website is nu tweetalig. (Ik ben nog bezig met een aantal pagina's te vertalen)
  * Introductie van "enkel lezen" mode voor het weergeven van de blokjes in de documentatie op de website.
  * Een aantal kleinere wijzigingen...

### Versie 0.4.1 (19 nov 2017)

  * Code in het "gegenereerde code" voorbeeld venster heeft nu ook kleurtjes.
  * Bugfixes
    * Compatibiliteit met microsoft Edge - Bug opgelost i.v.m. incorrect HTTP response gestuurd door Vubbi die ervoor zorgde dat Vubbi niet werkte op microsoft Edge.
    * Fix in gegenereerde code - Bug opgelost i.v.m. ontbrekende cast in gegenereerde code als een "2D snelheid" blokje gebruikt werd in een "kijk naar" blokje.

### Versie 0.4.01 (06 okt 2017)
	
  * Bugfixes:
    * Bug in verband met ontbrekende afbeeldingen.

### Versie 0.4 (06 okt 2017)

[![Versie04]({{ site.baseurl }}{% link assets/img/releases/versie04.png %})]({{ site.baseurl }}{% link assets/img/releases/versie04.png %})
	
  * Introductie van 3D physics voor alle blokjes met physics via een klein knopje (2D/3D): "wanneer ik iets raak", "wanneer scharnier kapot springt", "wanneer iets in mijn triggergebied komt", "schiet een lazer, ...", "snelheid van ...", "geef mijzelf een duw", "draaisnelheid van ...", "geef mijzelf een draaikracht"
  * Nieuwe blokjes in verband met muispositie & scherm-coördinaten:
    * "positie van muis in scherm met z=0"
    * "pixelpositie van muis op scherm"
    * "grootte van scherm in pixels"
    * "hoofdcamera object"
    * "coördinaat in scene van pixelpositie"
    * "pixelpositie op scherm van coördinaat"
    * "richting in scene van pixelpositie"
  * Nieuwe blokjes in verband met snelheid:
    * "zet snelheid van dyn. rigidbody van mijzelf op ..."
    * "zet draaisnelheid van dyn. rigidbody van mijzelf op ..."
  * Kleine verbeteringen:
    * Kleine herstructurering van de toolbox: een groep "Wiskunde" geïntroduceerd en een aantal categorieën onder geplaatst.
    * Het is nu mogelijke om de UI text van een ander object in te stellen.
  * Bugfixes:
    * Bug i.v.m. browser contextmenu dat verscheen boven het Blockly context menu.
    * Opmerking popup toont niet langer een hoop witruimte buiten de popup
    * Probleem opgelost met associativiteit van vermenigvuldiging die niet van toepassing was als Quaternions met meerdere Vectors werden vermenigvuldigd.

### Versie 0.3 (10 mei 2017)

[![Versie03]({{ site.baseurl }}{% link assets/img/releases/versie03.png %})]({{ site.baseurl }}{% link assets/img/releases/versie03.png %})
	
  * Introductie blokjes om te werken met rotatie
  * Introductie "wacht", "wacht-herhaal" en "tijd sinds wacht" blokjes (coroutines)
  * Introductie van meer vector operatie blokjes, schalen, normaliseren, dot & cross product, plus, min, maal, ...
  * Introductie andere nuttige blokjes zoals "ga naar scene" of "heeft ... tag ... ?".
  * Werking "Geheugen" blok volledig herschreven (met automatische migratie). Je hebt nu veel minder flexibiliteit in initialisatie van geheugen, maar Vubbi kan geen "foutieve" code meer genereren.
  * Compleet nieuwe manier om te werken met Vubbi:
    Nu maak je eerst een nieuw "VubbiScript" bestand aan. Je kan dus nu dubbelklikken op zo een bestand om een script te bewerken. (vroeger moest je een bestand kiezen in de Vubbi editor)
    Ook gewijzigd:
    * Afbeelding voor "Vubbi Script Files" toegevoegd
    * Nieuwe migratie tool om oude projecten over te zetten naar deze nieuwe VubbiScript bestanden
    * Verwijderen van code voor bestanden te kiezen of verwijderen vanuit Vubbi.
  * Nieuw "sla op" icoontje gemaakt en toegevoegd
  * Bestandsnaam is verhuisd en menubalk in Vubbi is verdwenen
  * 2D/3D knop toegevoegd (maar werkt nog niet)
  * Functionaliteit van het openen van Vubbi in een Unity venster afgezet. (was onhandig) In de plaats opent Vubbi nu altijd in de browser.
  * Blokjes in de toolbox hebben nu meer ingevulde blokjes om te tonen wat mogelijk is.
  * Naamwijziging... Scratchity => Vubbi.
  * Bugfixes...

### Versie 0.2 (26 dec 2016)

[![Versie02]({{ site.baseurl }}{% link assets/img/releases/versie02.png %})]({{ site.baseurl }}{% link assets/img/releases/versie02.png %})
	
  * Nieuwe bestanden hebben nu automatisch al een "Doe als ik start" en "Doe elke keer opnieuw" blok.
  * Code voor "code generatie" is volledig herschreven. De nieuwe versie heeft een hoop fixes waaronder correcte variable naam conflict behandeling, verbeterde plaatsing van haakjes.
    **Pas op:** Scripts die gebruik maken van "berichten" moeten opnieuw opgeslagen worden. De gegenereerde code is een beetje verschillend.
  * Nieuwe blokken: "klik muis gebeurtenis", "collision gebeurtenis", "joint kapot gebeurtenis", "vind object via tag", "vraag tag van object", "raycast", "simpele vector selectie", "aangepaste C# code blokjes", "voeg tekst toe aan", "maak tekst van ... (met correcte conversie voor nummers)"
    **Pas op:** Scripts die gebruik maakten van de oude "als ik bots met" blokken kunnen problemen ondervinden. (er zijn blokken verdwenen)
  * Nieuwe velden: type specifieke variable velden en optionele output blokken
  * Herwerkte UI voor zijbar en verbeteringen in top bar
  * Er is nu een zijpaneel met live code preview
  * Bevat basis voor vertaling van VubbiScript
  * Volledige hersortering van blokken in nieuwe categorieën
  * "hoedjes" geïntroduceerd voor gebeurtenis blokken
  * Verbeterde laadsnelheid (alles wordt gebuild tot 1 bestand + http keep alive + thread leak fix)
  * VubbiScript is open source geworden ([github repository](https://github.com/jeroenpx/scratchity/)).

### Versie 0.1 (22 Okt 2016)

[![Versie01]({{ site.baseurl }}{% link assets/img/releases/versie01.png %})]({{ site.baseurl }}{% link assets/img/releases/versie01.png %})
	
  * Zeer eenvoudig te installeren (!)
  * Nieuw blokje om tekst in te stellen van een UI Text component
  * Nieuw blokje voor de positie op te halen of in te stellen
  * Een aantal bugfixen

### Versie 0.0

Eerste versies van Vubbi.

### Geschiedenis... voor versie 0... was er project Ninjacode

29 Maart 2015: Starten met schrijven aan project Ninjacode.

20 Sept 2015: Gestopt met project Ninjacode...

Resultaat:

<figure>
  <a href="{{ site.baseurl }}{% link assets/img/releases/scratchity_v1_day24_scrollbars_and_arrow.png %}">
    <img src="{{ site.baseurl }}{% link assets/img/releases/scratchity_v1_day24_scrollbars_and_arrow.png %}"> 
  </a>
  <figurecaption>Screenshot van project Ninjacode (ook wel Scratchity versie 1)</figurecaption>
</figure>

Merk op dat alles zelf geprogrammeerd was, blokjes tekenen, slepen.
Project Ninjacode kon ook bestaande C# scripts lezen en aanpassen!

Wat ik geleerd heb van project Ninjacode...
Te veel werk om alles zelf te schrijven (blokjes tekenen, blokjes slepen, code generatie, tooltips, code parsing, ...) + inbouwen in Unity als een editor plugin is een niet eenvoudig door de weinige documentatie.

Doordat ik bestaande code lees had ik ook veel minder opties om de code simpel voor te stellen. Operaties zoals een variable naam wijzigen werden ook zeer complex...

25 Mei 2017: Alles weggooien en opnieuw beginnen aan Vubbi.
