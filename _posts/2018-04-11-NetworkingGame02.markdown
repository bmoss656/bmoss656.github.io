---
layout: post
title: Project Horde 02
date: 11-04-2018
author: Brad Moss
categories:
  - Blog
  - Low-Level Programming
  - Networking Game
img: Networking.png
thumb: horde_thumb.png
published: true
---
#### Progress

We have made a fair amount of progress on our game since last week, a large amount of work has been done on the networking side of things, as well as beginning to start on certain gameplay and UI elements. More detail on the progress can be read below.

<!--more-->

#### Networking

The networking side of our game is coming along nicely, with the majority of the core elements of it already implemented. This is largely thanks to one member of the team who focusses on the technical side of things more than myself (prefer to see myself as more gameplay orientated). What we have now is a way for us to send packets of data across the network which can then be converted into whatever data type we require, including custom data types such as game objects. This will allow us to easily send data to and from the server (we decided to take a client-server approach) meaning that we should be able to spend a good amount of time now focussing on the gameplay. 

#### Cursors and Camera

We decided that we wanted a custom cursor for our game, so I took it upon myself to start implementing it. I created a class for the cursor itself and thanks to a new feature in the ASGE which allows you to hide the standard cursor, it was rather simple to create a sprite that just followed the mouse’s current position. With some additional logic to smooth it out, I created a cursor that resembled a zombie hand and it would change when clicked or when hovering over certain UI elements which looks much nicer than the standard cursor.

For the camera we needed it to be slightly different to the system we created before as this game is going to be primarily controlled by the mouse (We haven’t decided on gamepad support yet) and we decided the camera itself should be able to move according to the mouse’s position. For example if the mouse is on the right edge of the screen, the camera should pan to the right. This can be seen below and well as the custom cursor in action. Note that the text does not move because it is locked in place for testing reasons, the movement can be seen from the sprite however.

[![https://gyazo.com/50c60d4c167c3ed72a094f9b201d76d5](https://i.gyazo.com/50c60d4c167c3ed72a094f9b201d76d5.gif)](https://gyazo.com/50c60d4c167c3ed72a094f9b201d76d5)

