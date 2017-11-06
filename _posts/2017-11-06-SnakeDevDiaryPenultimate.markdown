---
layout: post
title: Snake Dev Diary- Almost there
date: 6-11-2017
author: Brad Moss
categories:
  - Blog
  - Low-Level Programming
  - Snake
img: SnakeBanner.png
thumb: c_thumb.jpg
published: true
---

#### Progress Since Last Diary
The last time I posted here was last week before the weekend and back then I was having a lot of trouble with the snake body movement still. Since then I have made a huge amount of progress and have pretty much got the whole core game working now. This is due to the fact that after my post last week I took some time to think about what I was doing wrong and I just realised the code I was using to move my snake was causing me a lot of hassle. This led me to rethink how I did the movement and I realised a much more efficient way of doing it. The only problem with the more efficient way was that it changed how the snake looked as it moved, as I said in a previous post I wanted the snake to move fluidly around the game area rather than jumping from point to point. It has sort of ending up as a compromise between the two being much less fluid than I initially had planned but I still do like the new way it looks as it moves instead.

<!—more-->

In order to change the movement I had to do some research about creating a sort of delay for the core movement functions. I found a method online that could be used to effectively create a delay for however many seconds you wanted, I then adapted this method to suit my own code. So instead of constantly updating the snakes position slightly, I used this delay method to update the snakes main position by a certain amount every tenth of a second (This number can easily be changed), this made it easier to loop through and move every other section of the snake to the last position of the one in front of it. There were a few bugs that came along with this as my code was made for the constant updating of the position but I changed my code to work along with this more effective method.

#### Moving On
Once I had the movement working correctly, it meant I could start refining some of the aspects of the game and work towards having the full core game completed. I started by fixing the collision of the collectables to work with the new movement system and I adding in a game over screen for when the player either hits a wall or themselves. I made very quick progress after sorting the movement, it was very clear that this was what was holding me back for the past week or so and now that it was sorted, getting the other aspects of the game working proved to be mostly easy in comparison. One part I did have a little trouble with was adding the score, this was because I wanted the score stored as an integer and then printed as a string. I was not familiar with converting integers to strings so did some research around this and found there were multiple different ways I could go about doing it, I found the one I could most effectively add into my code and then created a simple function using this method to create my score.

#### Almost There
After the weekend I have the finished basic snake game with movement, score, menu and win/lose conditions all working correctly. The screenshot below shows where the game currently is. In order to actually finish the game to where I want it to be, I still have a couple of things I need to do. I need to create a level/difficulty system where you can choose what difficulty you want and the level will be different according to this, I hope to have the difficulty option in a separate settings menu. The final thing I will do, is find some nicer assets and art to make the game look more polished as apposed to how it currently looks. That is where I hope to be for next time.

[![https://gyazo.com/a1c548387a6d2581d747b1bd3ba64e40](https://i.gyazo.com/a1c548387a6d2581d747b1bd3ba64e40.png)](https://gyazo.com/a1c548387a6d2581d747b1bd3ba64e40)
