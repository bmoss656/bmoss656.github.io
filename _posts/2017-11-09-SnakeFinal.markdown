---
layout: post
title: Snake Dev Diary- Finished game
date: 9-11-2017
author: Brad Moss
categories:
  - Blog
  - Low-Level Programming
  - Snake
img: SnakeBanner.png
thumb: Snake_thumb.png
published: true
---

#### Snake is Finished!

 So my snake game is finally done. I’m overall quite happy with the final game that I created, considering I was unsure of how to start it at all about a month ago. It was a bit of a learning curve using the ASGE due to having no prior experience with it and it having limited documentation to provide guidance meaning it was mostly all self-taught. 

<!--more-->

In my last post I said that I wanted to create a sort of level/difficulty scale which could be altered in a settings menu. As I started to work on implementing this I changed my mind and rather than having an adjustable difficulty setting, I decided to just have different levels that you could progress through which would be harder to complete each time. In order to have something that changed as the game got more difficult, I decided to act upon one of my initial ideas that I had back in my first ideas diary, I added in additional obstacles that you had to avoid. The obstacles are prevalent in all the levels and they spawn in over time depending on your score, but in the harder levels there is a larger amount of them that you will have to avoid. As well as the obstacles, I also made it so that as you progress though each level your speed slightly increases, which can make the final level quite challenging compared to the first, and I feel that this difficulty scale adds to the initial gameplay. The screenshots below show how the final game looked.


Main menu Screen:
[![https://gyazo.com/bddca45e80d3df1d17f107f741eb5b7b](https://i.gyazo.com/bddca45e80d3df1d17f107f741eb5b7b.png)](https://gyazo.com/bddca45e80d3df1d17f107f741eb5b7b)

Mid gameplay:
[![https://gyazo.com/316ce67be90d6b54d9524a998263449b](https://i.gyazo.com/316ce67be90d6b54d9524a998263449b.png)](https://gyazo.com/316ce67be90d6b54d9524a998263449b)

#### How did it go?

One major problem that I had which took up most of my time was the movement of the snake’s body. I initially tried to move the snake using slight incrementation each frame and spent a good deal of time trying to get this method to work for the body. I think that I knew there was a better way of doing it but was too stubborn to give up on my initial method, looking back on this I wish I had stopped and rethought the movement sooner. Once I had the movement sorted using the new method, I made fast progress adding in the rest of the features of the game and I feel if I had sorted the movement perhaps a week earlier, I would have had more time to add additional levels and features which could have improved my game further. So when I next work on a project I will know not to lock myself into one way of thinking and go through multiple possibilities first before diving into my first solution.
Code wise its not exactly the way I had imagined it, I would have liked to be able to spread my code out among another class or two rather than having a couple of large ones. The levels and the obstacles are what I would have most liked to have had their own classes but due to these being added in at a late stage I had to incorporate them into an already created class, which worked fine but would have been better if they were more encapsulated.

#### To finish

I am mostly quite proud of the final game that I created as I feel that the gameplay mechanics that I added increase the user experience a fair amount compared to the original snake game. This was what I set out to do at the beginning, create a game that kept the simple formula of the original snake but also add a few extra features to increase replayability and overall enjoyment of the game. I will be avoiding snake for a long time now as I feel more than suitably burned out from all the testing I have done of my own game. Now onto the next one.
