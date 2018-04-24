---
layout: post
title: Project Horde 03
date: 20-04-2018
author: Brad Moss
categories:
  - Blog
  - Low-Level Programming
  - Networking Game
img: Networking.png
thumb: horde_thumb.png
published: true
---
#### Getting Behind

Unfortunately, since the last post about the game here, we haven’t made a huge progress on our game yet. There are a couple of reasons for this, including having to manage three different group projects with deadlines all within days of each other and in each group there is at least one member not pulling their weight, which obviously is causing some timing issues as we’re having to cover the extra work they should be doing. This took my focus away from our game as other deadlines were sooner and it was more crucial for me to focus on them and attempt to finish them before coming back to our RTS game. 

<!--more-->

#### Progress

But enough about the reasons why we’re not exactly on track with our game and now more about where we have gotten to and what development changes we have made. 

As our deadline draws closer, we decided that some of the features we initially had planned for our game would have to be scrapped and instead simplified in order for us to be able to hopefully finish the game in time. We initially wanted a basic crafting system which would involve collecting metal around the map and crafting new weapons with them. For this, I was going to create a basic weapon class which would handle all of the damage and range of weapons, instead I have built the damage functions into the units class which works off of a singular base value which limits us to one or two basic attacks unfortunately. We decided to cut the crafting system in its entirety to create less work for ourselves.

We also wanted to have boss fights scattered throughout our level which would be harder to kill and would perhaps play dynamic dramatic music in order to increase tension. Again unfortunately, this had to be scrapped due to timing reasons. Instead I’ve limited the unit class to only be able to create base zombies as well as different types of survivors/humans. 

#### Grid

I had some issues creating a grid to the exact standards another team member expected of me, this led to me spending too much time trying to get it working the way they thought it should, so they were happy, rather than doing it a way I was more comfortable with. Because of this, I’m not overly happy with the grid system in the game, it relies too heavily on position of the grid squares rather than a more simplistic row-col method which is how I would have liked to create it. It was functional however and did print out the squares as intended. 

The grid now just needed some extra functionality for the units, so I created some functionality that would allow, when a unit is selected, the tiles around said unit to be lit up to see available movement. The units currently just glide towards their target rather than smoothly walking towards it and their attack functionality is what I will be implementing next. 

It would be nice if we had all team members working on our game rather than just two of us, I did make this issue with our other teammate known but nothing was done about it, therefore leaving us in a similar situation as with our previous group game. Nevertheless, I will continue working as hard as I can, however my work over the last few days has been somewhat limited due to multiple pieces of coursework and I’ve been dealing with constant head pains for the past week which somewhat effects my ability to focus and code effectively. A gif of our current game state can be seen below.

[![https://gyazo.com/8da024dd67c1044bdd8b13b04329694a](https://i.gyazo.com/8da024dd67c1044bdd8b13b04329694a.gif)](https://gyazo.com/8da024dd67c1044bdd8b13b04329694a)
