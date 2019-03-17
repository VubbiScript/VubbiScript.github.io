---
layout: docs
docs_id: detect
title: Documentation
description: Detect - description of the detection blocks in VubbiScript
lang: en
subtitle: Detect
slug: docs
---

This category does not contain a lot of blocks yet, but the ones that are there can be very useful.

{% include blocks/DocsDetectKey.xml align="img-left" %}

**"button ... just pressed down"** is a block you will use a lot. It returns "true" if the button was just pressed by the player. Usually you call this block every frame to check if the user is doing something. (See the "repeat every frame" block under "Events" or the blocks in the category "Time")

You can also use the **"button ... still pressed down"** if you for example want to keep speeding up as long as the player is holding the button down.

{% include blocks/DocsDetectKey.xml align="img-left" key="Mouse0" %}

This block also works with mousebuttons. With the **"button first (primary) mouse button just pressed down"** you can test to see if the user clicked. For this block it does not matter where he clicks. If you want to know whether the player clicked on some object (e.g. a button) it is better to use the  "when a mousebutton ... on me" in the category "Events".

{% include blocks/DocsDetectRaycast.xml align="img-left" %}

Next to that we also have the more complicated block **"shoot a laser..."** which you can use to check if there is an obstacle in a certain direction. You can for example shoot a laser downwards to check how far you are from the ground. You can also shoot a laser to the right to check if there is a wall...

{% include blocks/DocsDetectMouseScene2D.xml align="img-left" %}

With "position of mouse in the scene with z=0 (2D)" you can find out where the mouse is in the level. You can use this block to aim things like cannonry or other things with the mouse. Or you can also just have the player follow the mouse. This block works best in 2D but could also be useful in 3D.

{% include blocks/DocsDetectMouseScreen.xml align="img-left" %}

Sometimes you don't want to know where the mouse is in the level but instead you want to know where the mouse is on the screen. You can find that out with these blocks. This way you can for example move the camera to the right if the mouse is on the right side of the screen.
