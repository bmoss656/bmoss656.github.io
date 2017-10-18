---
layout: post
title: Snake Dev Diary
date: 18-10-2017
author: Brad Moss
categories:
  - Blog
  - Low-Level Programming
  - Snake
img: SnakeBanner.png
thumb: c_thumb.jpg
published: true
---

#### Planning

So, it has been just over a week since my last post and I’ve started to make some progress with the game. However before diving straight into coding the game, I first took some time to plan out how I wanted the core of the game to be and what sort of classes I would need to accomplish this.

My initial thoughts had me thinking of changes such as adding obstacles, difficulty levels, lives and a customisable grid just to name a few. For the actual game my plan is to include more of a level system which has the difficulty curve built straight into the levels so as you progress the game becomes harder. I will be keeping the option for the player to change difficulty in the sense that they will be able to choose how many lives they start with depending on how easy they want the game to be. The difficulty curve in the levels will come from the number and size of obstacles and I will also change the speed of the players character as the levels progress. Progressing from one level to another will require the player to collect/eat a certain amount of the collectables in the level within a time restraint. A potential feature that I’m not sure whether I will include yet is letting the player attack/destroy the obstacles, this adds another level of player interaction but I will decide on this soon. 

I had a rather good idea of how I wanted my game to play which meant I could move onto planning out the basic layout of my class structure and do some pseudocode to give myself a simple idea of how I might accomplish some of the things I want to do. The UML diagram below gives a very basic look at the classes I will implement for my game, these are not 100% accurate and will be subject to some change but it shows an overview of the classes I will need. These are of course on top of the already implemented Main and Game classes.

[![https://gyazo.com/258922f34b0ca992579ea1719fd328f9](https://i.gyazo.com/258922f34b0ca992579ea1719fd328f9.png)](https://gyazo.com/258922f34b0ca992579ea1719fd328f9)

#### Initial Planning

So, after a little bit of time starting to get familiar with how the ASGE works, I started to implement some basic features such as rendering the playing scene and player sprite. I then sorted some basic movement for the player, currently the player sprite moves constantly and you can change the direction with wasd, this is shown below.

[![https://gyazo.com/dc7dbe06ec699bec03fb66b5805e6730](https://i.gyazo.com/dc7dbe06ec699bec03fb66b5805e6730.gif)](https://gyazo.com/dc7dbe06ec699bec03fb66b5805e6730)

