---
layout: docs
docs_id: events
title: Documentation
description: Events - description of the event blocks in VubbiScript
lang: en
subtitle: Events
slug: docs
---

TODO: TRANSLATION PENDING!

Deze blokjes zijn de beginblokjes van een stuk code.

{% include blocks/DocsEventStart.xml align="img-left" %}

**"wanneer ik start"** wordt opgeroepen wanneer het spel start of als het object toen nog niet bestond, dan wanneer het object pas is aangemaakt (bijvoorbeeld een kogel die net afgeschoten is).

{% include blocks/DocsEventUpdate.xml align="img-left" %}

**"elke frame opnieuw"** wordt elke frame opgeroepen. Typisch is dit 60 keer per seconde in Unity. Er zijn ook andere manieren om dingen te herhalen over een bepaalde tijd in Vubbi of om met tijd te werken. Zie categorie "Tijd".

{% include blocks/DocsEventsMouse.xml align="img-left" %}

**"wanneer de muis ..."** kan je gebruiken om met de muis te werken. Om deze blokjes te kunnen gebruiken heeft je object een Collider nodig! De Collider wordt gebruikt om aan te duiden waar je object is.

{% include blocks/DocsEventMessages.xml messagename="doe iets" align="img-left" %}

**"wanneer ik bericht ... ontvang" / "zend bericht ... naar"** kunnen gebruikt worden om objecten te laten praten met elkaar. Een kogel kan bijvoorbeeld naar elk object dat het raakt "ga dood" sturen. Als je een muntje verzamelt kan dat muntje naar de score tekst op je scherm sturen dat er een punt is bijgekomen. Er zijn veel manieren om aan dat andere object te komen. Als je botst weet je waarmee je gebotst bent. Als het altijd hetzelfde object is kan je ook vanuit Unity dit object instellen of je kan gebruik maken van het blokje "zoek GameObject met tag" (zie categorie "Objecten").



{% capture example %}
**Voorbeeld** - "Berichtjes" - score bijhouden en tonen...

![Scorekeeper.PNG]({{site.baseurl}}{% link assets/img/Scorekeeper.PNG %}){:.img-right.img-sm}
Als je een punt scoort stuurt een bepaald object een bericht "score" naar de "scorekeeper" (in bovenstaand spel stuurt de juist vernietigde asteroïde het bericht).

<div class="clear"></div>

{% include blocks/DocsExampleScoreSend.xml messagename="score" tagname="scorebewaarder" %}

De "scorebewaarder" die de score toont ontvangt dit bericht, telt 1 op bij de score en toont de score op zijn UI tekst component.

{% include blocks/DocsExampleScoreReceive.xml messagename="verhoog score" scoretext="Score" varname="huidige_score" %}
{% endcapture %}

<div class="exampleblock">{{example | markdownify}}</div>



{% include blocks/DocsEventOnCollision.xml align="img-left" %}

**"wanneer ik net iets raak"** kan gebruikt worden om te controleren of je je op de grond bevindt. Je kan het blokje ook gebruiken om botsingen te detecteren met bijvoorbeeld kogels om zo een leven te verliezen.
Door op het "plusje" te klikken kan je de snelheid waarmee je botst of het object waarmee je botst opslaan in het geheugen en er zo andere dingen mee doen zoals bijvoorbeeld een berichtje naar sturen...

Je kan er ook mee implementeren dat iets kapot gaat als het valt... zoals in het voorbeeld hieronder.



{% capture example %}

![vubbi_falldamage.gif]({{site.baseurl}}{% link assets/img/gifs/vubbi_falldamage.gif %}){:.img-right.img-sm}

**Voorbeeld** - "wanneer ik net iets raak" - een blokje kapot laten gaan als het hard valt...

Hoe werkt dit? Eerst en vooral hebben we een natuurlijk een "wanneer ik net iets raak" blokje nodig. We willen het ook meer kapot laten gaan als er iets met meer snelheid tegen botst. We houden een soort van "leven" bij per blokje. Als het blokje dan nog 75% of meer leven heeft ziet het er nog goed uit. Als het tussen 75% en 50% leven heeft zie je al een scheur. En zo verder... Als het minder dan 0% leven heeft maken we een effectje en vernietigen we het blokje.

De code ziet er uit als:
{% include blocks/DocsExampleFallDamage.xml 
  memlifestart="levenBegin"
  memlifenow="levenNu"
  memsprite25="uiterlijk25procent"
  memsprite50="uiterlijk50procent"
  memsprite75="uiterlijk75procent"
  memcollspeed="botsingSnelheid"
  memobjexplosion="prefabExplosie"
  memobjcreatedexplosion="nieuweExplosie"
%}
{% endcapture %}

<div class="exampleblock">{{example | markdownify}}</div>



Met de 2D/3D knop kan je wisselen tussen 2D en 3D physics. Let op dat je ook de juiste componenten toevoegt aan je object.

{% include blocks/DocsEventOnJointBreak.xml align="img-left" %}
**"wanneer scharnier kapot springt"** wordt opgeroepen als een "Joint" kapot gaat. "Joints" kan je aanmaken in Unity en laten toe om objecten op bepaalde manieren aan elkaar te hangen... Hangbruggen, kettingen, wielen van een auto, ... Deze kun je maken met Joints. Je kan ook instellen in Unity wanneer deze kapot springen.

{% include blocks/DocsEventOnTrigger.xml align="img-left" %}
**"wanneer iets net in mijn triggergebied komt"** is bijna hetzelfde als "wanneer ik iets raak" alleen zal deze worden opgeroepen als je de botsing hebt ingesteld als "trigger" in Unity. "trigger" heeft als effect dat de objecten niet zullen botsen maar door elkaar gaan. Zo kan je bepalen of een speler voor een bepaalde deur loopt zonder dat hij tegen de deur moet lopen.