---
layout: post
title: Tic Tac Toe Redesign
date: 15-10-2017
author: Brad Moss
categories:
  - Blog
  - Play and Games  
  - Board Games
img: TicTacToePicture.jpg
thumb: BoardGameTN.png
published: true
---

#### Initial Thoughts

So, as a design exercise on my games technology course, we spent some time looking at and redesigning the classic game tic tac toe in small groups (Group of 4, for us). 

In order to see how we could change this classic game, we first had to play and analyse what was wrong with it. Obviously one of the clear things wrong (and also right with) with this game was the simplicity of it. For younger children and for a quick time passer, the simplicity of this game works just fine, but we were looking to add a bit more depth and longevity to it. 

<!--more-->

#### Making Changes

We realized the basic issue was that if two players played perfectly, the game would always end in a draw because the tactics of the game are very simple. So we started with the obvious changes such as increasing the grid size, however this had no real impact on the game and it still ended the same way the original did, quick and always in a draw or win. 

After a few changes like this we came up with the idea of limiting the number of players moves, aka it meant that the players could only place three noughts or crosses in total. However, the player was instead able to move their 3 pieces around after they had been placed but only to an adjacent grid square. This meant that instead of the grid filling up and ending in a draw, it added a bit more depth to the game and required a little more thought as to where you would put or move your pieces to. A basic example of how this works is shown below.

[![https://gyazo.com/f65b13f2db1914a5526c5bff6486e88a](https://i.gyazo.com/f65b13f2db1914a5526c5bff6486e88a.png)](https://gyazo.com/f65b13f2db1914a5526c5bff6486e88a)

We initially had it so you could also move diagonally, however this caused an endless loop of blocking the win and therefore took what we were trying to do in extending the game a bit far! To solve this we simply took out the ability to move diagonally and this created a much more balanced game which we found to be much more enjoyable and engaging than the basic tic tac toe.
