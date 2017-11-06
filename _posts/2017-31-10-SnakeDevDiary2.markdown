---
layout: post
title: Snake Dev Diary- Some Progress
date: 31-10-2017
author: Brad Moss
categories:
  - Blog
  - Low-Level Programming
  - Snake
img: SnakeBanner.png
thumb: c_thumb.jpg
published: true
---


#### Collision and Movement

Since my last post on here it has been about 10 days and I’ve spent a fair amount of time working on the game and trying to get the movement of the player working correctly. Last time I had the movement of just the first section of the snake working so the next step was obviously to try and get the second section of the snake to render/spawn after a collision with a collectable. The framework we are using does not have built in functions for creating bounding boxes or dealing with collision so I did some research of my own and worked out a way to manually handle a collision between objects. 
<!--more-->
The next step for me was to get a sprite to render after the collision occurs at the right position which depended on the direction of the player. I thought of a couple of different ways of doing this but the first and simplest way I thought of was having a Boolean for each direction which would allow you to render the next sprite ‘behind’ the player depending on which way you were moving, this worked effectively for me, so I used this method. The rendering of the sprite was simple enough, but getting it to move properly behind the player was more of a challenge... I spent a lot of time planning out how I would move the sprite effectively but when it got down to putting this into the code, it didn’t always work as planned. The simplicity of it eventually dawned on me, I just needed to make the second sprite move to wherever the player sprite previously was, and once I realised this I could get the movement of the second sprite working, as seen below.

[![https://gyazo.com/f950cc7ee066132a8c41f6399dd1f0c5](https://i.gyazo.com/f950cc7ee066132a8c41f6399dd1f0c5.gif)](https://gyazo.com/f950cc7ee066132a8c41f6399dd1f0c5)

#### Body issues

So after getting those two aspects working I moved on to getting the rest of the snake to render and move appropriately as the collectables are collided with. I initially wasn’t sure on the best way to store and render the sprites, but I figured that the best way would be to simply load the sprites into an array and render a certain amount of them depending on the amount of collectables collided with. This worked well enough for me to progress to the movement, which is where I’m currently having some issues. The way I’ve been handling the movement of the snake is causing some problems when the snake becomes longer because it updates the positions too frequently making it hard for the later sprites to follow their ‘parent’ sprite accurately. I may have to reconsider how I’ve done the movement and instead make the movement less fluid by introducing a more co-ordinate based movement system. Another option may be adding in some sort of delay function to slow down the movement updating, allowing the sprites to move more effectively to the last position. The gif below shows where I am currently, hopefully by next time I’ll have sorted the movement and once the movement is sorted, I shouldn’t have many problems finishing the game.

[![https://gyazo.com/c7fedffeb8f87d9426afe672f27a8f02](https://i.gyazo.com/c7fedffeb8f87d9426afe672f27a8f02.gif)](https://gyazo.com/c7fedffeb8f87d9426afe672f27a8f02)
