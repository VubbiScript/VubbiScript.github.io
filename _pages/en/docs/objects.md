---
layout: docs
docs_id: objects
title: Documentation
description: Objects - description of the blocks to work with objects in VubbiScript
lang: en
subtitle: Objects
slug: docs
---

TODO: TRANSLATION PENDING!

Deze categorie bevat blokjes om te werken met "objecten".
Objecten zijn "donkergroen" (de uiteindes die ze teruggeven + waarin ze passen).

Met objecten kan je zeggen op WIE een bepaalde blok moet werken. Zo kan je de positie van "mijzelf" instellen, maar ook de positie van een object die je hebt gekregen via andere manieren.

{% include blocks/DocsObjectsSelf.xml align="img-left" %}
Zoals we al in veel vorige blokjes hebben gezien is er dus een object **"mijzelf"**.

<div class="clear"></div>

{% include blocks/DocsObjectsNull.xml align="img-left" %}
Daarnaast hebben we ook een blokje "niets". Dit blokje stelt **"geen object"** voor. Meestal wil je dit niet gebruiken maar het kan ook nuttig zijn. Zo kan je "niets" wel bijhouden in het geheugen en zal dat zelfs de waarde zijn als het geheugen nog niet ingevuld is. Zo kan je controleren of er iets in je geheugen zit.

{% include blocks/DocsObjectsTags.xml align="img-left" tagfind="scorebewaarder" tagcompare="vijand" %}
Daarna volgen een aantal **blokjes om te werken met tags**. Tags kan je instellen op een object vanuit Unity. Je kan tags gebruiken om snel een object terug te vinden, bijvoorbeeld via de "zoek GameObject met tag" blok. Zo kan je een object in de scene zoeken om er bijvoorbeeld berichtjes naar te sturen. Je kan ook de tag van een object opvragen. Zo kan je als je met een object botst controleren of het een vijand is of een muur or wat dan ook.

{% include blocks/DocsObjectsMainCam.xml align="img-left" %}
Bij de object blokjes vind je ook een blokje dat het object met de camera teruggeeft. Dit is handig omdat je bij sommige andere blokjes de camera moet meegeven. (zie blokjes in verband met coördinaten op het scherm in de sectie "coördinaten en richtingen")

{% include blocks/DocsObjectsCloning.xml align="img-left" %}
Verder hebben we blokjes om **objecten te klonen**. Je geeft een object mee om te klonen. Dit kan jezelf zijn of bijvoorbeeld een "kogel" object dat zich nog niet eens in het level bevindt. Daarnaast heb je een blokje waarmee je **elk object kan vernietigen**. Het hoeft niet eens gekloond te zijn.

<div class="clear"></div>
&nbsp;
<div class="clear"></div>

{% include blocks/DocsObjectsSetLook.xml align="img-left" %}
Als laatste hebben we een blokje waarmee je het **uiterlijk van een object kan veranderen**. Hiervoor heeft dat object een "SpriteRenderer" component nodig. Aan dit blokje moet je een "Sprite" meegeven. De enigste manier waarop je momenteel aan een sprite kan is via het geheugen.