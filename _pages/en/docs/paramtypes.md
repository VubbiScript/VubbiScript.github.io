---
layout: docs
docs_id: paramtypes
title: Documentation
description: Types of parameters - which types of parameters exist in Vubbi?
lang: en
subtitle: Types of parameters
slug: docs
---

TODO: TRANSLATION PENDING!

Alle parameters en resultaten van blokjes in Unity hebben een type.
Er zijn momenteel 7 datatypes in Vubbi:

{% include blocks/DataTypesTable.html data=site.data.datatypes.nl %}

<p><div>Elk type heeft een kleur. Die kleur zie je terugkomen in een aantal plaatsen maar het meest belangrijke is dat je daardoor kan zien welk soort type een object teruggeeft... 
Zo geeft het volgende blokje {% include blocks/DocsReturnTypesGet.xml type="Number" varname="item" align="blocks-align-inline" %} een nummer terug (donkerblauw) en blokje {% include blocks/DocsReturnTypesGet.xml type="Vector3" varname="item" align="blocks-align-inline" %} een coördinaat/richting (geel). 
Dit kan je zien aan het linkeruiteinde van de blok.</div></p>

<p><div>Verder kan je ook zien welk type argumenten een bepaald blokje verwacht. Zo verwacht het volgende blokjes een nummer
{% include blocks/DocsReturnTypesSet.xml type="Number" varname="item" align="blocks-align-inline" %} en blokje
{% include blocks/DocsReturnTypesSet.xml type="Vector3" varname="item" align="blocks-align-inline" %}
een coördinaat/richting.
Dit kan je zien aan de donkerblauwe/gele "uitholling".</div></p>

Als je een blokje probeert in te vullen waar het niet past zal dit niet lukken.

**Waarom werkt Vubbi met typing?** Vubbi zet de code om naar C# code voor Unity. C# code voor Unity is echter object oriënted en static typed en dit merk je dus ook deels in de blokjes.