---
author: jeroenpenninck
comments: false
date: 2017-05-07 21:18:52+00:00
layout: page
title: Start with Vubbi!
description: Get started fast with Vubbi. Install Unity, make a new project en install Vubbi in your new project.
lang: en
slug: getting-started
---

### Step 1: Download and install Unity3D
![Unity Logo]({% link assets/img/other/unity-logo-rgb.png %}){:.img-right.img-sm}

You can download the free version of Unity at:
[https://store.unity.com/download?ref=personal](https://store.unity.com/download?ref=personal)

Note that the Unity3D editor does not work on Linux! Games you make with Unity can be played on Linux though.

🕓 This step usually takes half an hour or more!


### Step 2: Make a new Unity project

**Tip:** Unity is hard to start with. For your first Unity project it is best to start in 2D.

<figure>
  <img src="{{ site.baseurl }}{% link /assets/img/gifs/gif_unity_asteroids_new.gif %}" class="img-sm"/>
  <figcaption>Making a new Unity project</figcaption>
</figure>

### Step 3: Install Vubbi into your new project

Make sure your Unity project is opened. If it is, Unity will ask automatically whether you want to import VubbiScript into your open project when opening the downloaded file. 

{% include util/downloadbtn.html
  label="Download Vubbi"
  version="v0.5.02"
  url="https://drive.google.com/uc?export=download&id=1EduHwM9s0mj3h6MnRo7s9nEnYePeEre1" %}

The installation is simple. Simple click "Import" after opening the file.

 - [Problems? click here!]({{ site.baseurl }}{% link _pages/en/havingtrouble.md %})
 - [How do I upgrade to a newer version of Vubbi?]({{ site.baseurl }}{% link _pages/en/upgrade-info.md %})
 - [release info and older versions]({{ site.baseurl }}{% link _pages/en/release-notes.md %})


### How to use Vubbi?

First you make a new VubbiScript (Create > VubbiScript), edit it and save.

<figure>
  <img src="{{ site.baseurl }}{% link /assets/img/gifs/gif_vubbi_make_script.gif %}" class="img-sm"/>
  <figcaption>Making a new VubbiScript</figcaption>
</figure>

When you save a C# file is also created. This script can then be used inside Unity.


### So, what's next?

**Before you start with VubbiScript you should actually have some basic knowledge of how Unity works.** You can try making something simple in Unity with the Standard Assets in Unity + Unity Terrain (you could try making a first person shooter for example) without coding! Once you know how to do that you can easily start programming with VubbiScript.

{% comment %}
You can start with a [Short introduction to Unity]({{ site.baseurl }}{% link _pages/en/short-introduction-to-unity.md %}).
{% endcomment %}

To start with Vubbi you can have a look at the overview of available blocks. You can find this overview in the [Documentation]({% link _pages/en/docs.md %}). Next to that there are also [Example projects]({% link _pages/en/example-projects.md %}) you can start from.

