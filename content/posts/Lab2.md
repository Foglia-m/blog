+++
title = "Lab2: roll-a-ball, or the best tutorial you've ever seen"
date = 2020-11-02T16:32:42+01:00
draft = false
description = "Unity somehow managed to make the harsh world of game development a joyful and rewarding experience"
showFullContent = false
+++

The Unity community is known to be  new user friendly and its tutorials are the quintessence of this idea as they explain slowly but surely what you can figure out by yourself but instead of building it in a messy way, you follow logical and methodical steps. 
Generally, I'm not into following tutorials as I prefer to keep the reasoning on my side only so I propose a 2 step approach that definitely looks like what my granny used to do to teach us (her grand children) to ride bikes. She would show the way going first and let us mimic her way of doing so in order to learn. But of course my brother and I were more about racing so we'd not follow her advises so the solution she came up with was my grandpa driving what she called a "broom car", if we could not go further exhausted by our racing pace we would end up getting grandpa's advices comfortably seating in the "broom-car".
 This slow unity tutorial pace is definitely a "broom-car" that won't fit the bold racer dev type but can definitely help you up if you're stuck on something obvious that you could not get by yourself. Their design is made this way: very clear milestones so that you know exactly what is done within and can keep going your way and eventually merge your work with how they do it.


About my work, I followed the tutorial and implemented the same basic version of the game.
 As a portal fan I want to add portals to it but I'm not sure they'll be completed at time when I upload this blog. 
I also want to implement a techno mode where the music and the visual effects make the game look like a huge party => this would be perfect as a VR implementation ( subcounscious Tetris Effect inspiration all the way here).
Another great inspiration in my life is Zelda's game design so I want to add a triggered wind effect to the game.

I have not encountered any issues making the basic game. 

Here is the gampeplay of the game so far, in order to add the bounciness that gives the game some more energy, I added a physic material with te following settings: 
dynamic friction: 0.1
static friction: 0.2
Bounciness: 1
Friction combine : multiply (multiplies both frictions between the ball and the other material)
Bounciness combine : maximum => few energy loss so that the ball bounces all the time with 1 (no matter what other material it bounces on)

The Death and portal share the same script (although I built two different in order to link the portals in the future)
They use trigger collider and are linked to a platform that gives its position in order to spawn the ball back in the game.

gameplay: 
{{< youtube IDzou4Z75Nc >}}