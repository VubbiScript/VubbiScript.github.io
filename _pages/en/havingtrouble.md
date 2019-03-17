---
author: jeroenpenninck
comments: false
date: 2017-11-19 16:21:09+00:00
layout: page
title: Problems & Unity bugs?
description: When you cannot install or use Vubbi, one of the following things could be wrong.
lang: en
slug: getting-started
---

If you cannot install or use VubbiScript one of the following things could be wrong.

Do you have a different problem? Let me know!

# Install problems

## Windows: the Vubbi install file opens a new Unity window and does not install in my project.

**Problem:**
I just installed Unity and created a new project. After that I downloaded Vubbi but when I click on the file it opens a new Unity window without project. My Unity project is open, why doesn't Vubbi install correctly?

**Cause:**
This is probably because Unity and you webbrowser are not running under the same windows user. During installation of Unity you had to enter the password of the administrator after which the install process started running under the administrator user. At the end of the install process Unity is started under the adminstrator user. Other programs on your computer are still running as a normal user though.

**Solution:**
You will have to restart Unity, afterwards everything will work as expected.
BUT WATCH OUT: since Unity is running under the administrator user you will have trouble accessing your saved Unity project afterwards without the administrator password. You might need to restart completely.

## Unity asks to re-login, but keeps "waiting".

**Cause:**
Probably a firewall problem of the location you are currently. I had this in the buildings of Odisee Aalst (CoderDojo Aalst)

**Solution:**

  1. Turn off your internet
  2. Re-open Unity
  3. Click "manual" and save the file on your desktop
  4. Turn on the internet again
  5. Click the link in the Unity window to go to the website (unity.../manual)
  6. Log in and upload the file you just put on your desktop
  7. Download the file you get from the Unity website and also place it on your desktop
  8. Inside unity, click the button to select the new file
  9. If everything went ok you will now see your list with projects again and you can continue working.

# Unity problemen

## I cannot drag images to Unity

**Problem:**
I cannot drag images from my computer to Unity.

**Cause:**
There are multiple possible causes:
1. Make sure the images you are trying to drag are not inside a zip
2. Did you just install Unity? It could be Unity is running as an administrator but other programs on your computer are running as a normal user.
3. If dragging inside Unity also doesn't work it could be something on your computer not working together very well with Unity.

**Solution:**
Depending on the cause (see above):
1. Unzip the folder before trying to drag
2. Restart Unity, but WATCH OUT: since Unity was opened under the administrator user you will most likely lose your saved Unity project. You will not be able to access it without the administrator password. You might need to start from an empty project again.
3. No clue. I did not manage to solve this when I had it. There are ways to use Unity without dragging but they are not very practical.

## I have chosen a 2D project but my images are no importing as sprites.

You can change the default behavior in:
Edit -> Project Settings -> Editor -> Default Behavior:2D
