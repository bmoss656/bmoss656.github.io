---
layout: post
title: Runner Game Blog- Final
date: 14-12-2017
author: Brad Moss
categories:
  - Blog
  - Low-Level Programming
  - Runner Game
img: Runner2.png
thumb: Runner_thumb.png
published: true
---
#### Finished

I’ve now completed my runner game and I’m pretty happy with my final version. There are still things I would have liked to add given more time but I think it has enough content in order to be an enjoyable game and I’m proud of what I have created.

<!--more-->

#### Final Version

So the final version of my game unfortunately ended up quite different to my original plan, due to time constraints mostly. But the core idea of what I planned still exists in the game that I have created. Basically the game I have created is an endless runner where you have to collect coins in order to increase your score and navigate the platforms using a combination of single and double jumps. The score is also placed into a high score table on the main menu which can be seen in a screenshot below.

[![https://gyazo.com/8660cef21cd2b66cda37a4cae2d36767](https://i.gyazo.com/8660cef21cd2b66cda37a4cae2d36767.png)](https://gyazo.com/8660cef21cd2b66cda37a4cae2d36767)

#### What went well

Compared to when I used the ASGE to create snake, I felt much more confident using it this time due to my previous knowledge of it. This meant that I was able to make much quicker progress setting up basic things such as movement and changing between scenes due to having done similar movement before. Obviously in my runner game it is a bit more advanced because it involves jumping and more complex movement but I didn’t have too much trouble implementing it correctly. An improvement that was suggested for me over my snake game was to make use of the engine’s built in delta time, I did have a bit of trouble with this and I’m not 100% happy with the way I used it but I did implement and use it in my runner game which is a step in the right direction over my snake game. I also implemented some animation into my game which really brings it to life and makes it feel more like an actual game compared to when I had a static block moving around.

A major improvement and something I felt I did well, is the way I structured my code base. I took a much more OOP approach compared to last time and I feel that I have suitably abstracted my classes. I made a decision to have classes for different states of the game, e.g. - Menu, playing the game, game over etc. As well as having classes for the player and the game itself. This allowed me to put different logic in different classes depending on where it was needed rather than putting it all in one class. For example everything to do with the generation of my level is handled in the GameLevel.cpp class yet this class interacts with the Player.cpp class in order to do things such as collision.

#### Final thoughts

There are a lot of features that I would have liked to add to my game, such as different power ups, a variety of levels, different characters, just to name a few. I would have also liked to perhaps take my procedural generation and make it a bit more complex and slightly less predictable, but it is suitable for now and considering I had no previous knowledge of it, I think I did quite well. Overall I’m pretty happy with my final product and feel it has definitely helped my coding skills develop. The gif below gives a little glimpse into my final game.

[![https://gyazo.com/4c693d48c42a0e1b8f1dc92135471f39](https://i.gyazo.com/4c693d48c42a0e1b8f1dc92135471f39.gif)](https://gyazo.com/4c693d48c42a0e1b8f1dc92135471f39) 

