---
layout: docs
docs_id: time
title: Documentatie
description: Tijd - beschrijving van de blokjes om te werken met tijd in VubbiScript
lang: nl
subtitle: Tijd
slug: docs
---

{% include blocks/DocsTimeWait.xml align="img-left" %}
In de "tijd" categorie hebben we **de "wacht" blokjes**. Het **"wacht tot volgende frame"** wacht een frame (zie "doe elke frame opnieuw"). Het **"wacht ... seconde(n)"** blokje wacht een gekozen tijd in seconden.

Deze "wacht" blokjes **kunnen gebruikt worden op ELKE plaats** waar je een gewoon blokje kan gebruiken! Je kan ze gebruiken in het "wanneer ik start", het "elke frame opnieuw" blokje of zelfs in bericht blokjes en "wanneer ik net iets raak" blokjes. Je kan ze gebruiken in een deel van de "als-dan" enzovoort...
Hou er wel rekening mee dat zolang je aan het wachten ben, die "groep" blokjes niet meer uitgevoerd zullen worden. Zo zal "elke frame opnieuw" natuurlijk niet meer elke frame opnieuw zijn als je ineens beslist om een seconde te wachten. Je kan wel meerdere "elke frame opnieuw" blokjes hebben. Als je in één van die blokjes wacht zullen de andere wel nog "elke frame opnieuw" worden uitgevoerd. Dit is voornamelijk belangrijk voor "wanneer ik net iets raak". Dit blokje zal dan niet uitgevoerd worden als je iets nieuw raakt en je nog aan het wachten bent (maar meestal wil je dat ook niet). Tip: als je wel alle botsingen wilt ontvangen tijdens het wachten kan je nog een ander "wanneer ik net iets raak" blokje maken of kan je het "wanneer ik net iets raak" blokje combineren met een "elke frame opnieuw" blokje en het geheugen (en dan wachten in het "elke frame opnieuw" blokje.

{% include blocks/DocsTimeGet.xml align="img-left" %}
Daarnaast hebben we blokjes die ons **informatie geven over de tijd**. Deze hebben een blauw uiteinde en geven dus een getal terug. Dit getal is in seconden. Met deze blokjes kan je een "timer" bouwen (via "tijd sinds start van het level") of kan beter werken met snelheden (via "delta tijd") (bijvoorbeeld snelheden uitdrukken in afstand per seconde in plaats van afstand per frame).

{% include blocks/DocsTimeRepeat.xml align="img-left" %}
De **"herhaal elke frame"** blokjes doen bijna hetzelfde als het "wacht tot volgende frame" blokje, maar voeren eerst een stuk code uit, wachten dan en blijven dit gewoon herhalen.

Ze doen ook bijna hetzelfde als het "elke frame opnieuw" gebeurtenis blokje maar je kan ze op elke plaats gebruiken en je kan ze laten stoppen met herhalen. Aan het tweede blokje kan je namelijk een blokje met een oranje uiteinde meegeven dat "onwaar" kan worden als het herhalen moet stoppen. (voor blokjes die "oranje" dingen teruggeven, zie categorie "logica")

{% include blocks/DocsTimeRepeatTime.xml align="img-left" %}
Als laatste hebben we een blokje dat de tijd aangeeft sinds we gestart zijn met de herhaal-lus. Dit blokje kan je dus enkel gebruiken in de "herhaal elke frame" blokjes hierboven.