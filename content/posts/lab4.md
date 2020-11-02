---
title: "Lab4: VR another step towards complexity"
date: 2020-11-02T16:32:48+01:00
draft: false
description: VR development is way more complex because of the particularity of inputs and cameras, but following tutorials can, as always, help you to get it done quite fast, the question that remains is: did you get any of that? (yes the exact same question you get at the end of a Rick & Morty episode...)
---

I managed to make things work as this footage shows:

{{< youtube J4mPBWyfWgA >}}



Unfortunately, I had few access to the VR lab because of the COVID so I could not fix some issues: mainly the offset of the object when you grab it in VR.

But the main issue with this is that I followed the guidelines with interest but couldn't come up with any critical vision on what I was doing because I had so few experience in what I was doing, it was the first I coded anything in VR but it felt way more magical than everything I had done on Unity before, the main reason is that you import many packages because building everything from scratch must be a nightmare. It was a long process but it ended up working by following closely every step so that's my best advice when you work on something you don't know well technically : follow each steps carefully.
Still I think the integration of my game to the VR environment went smoother than expected and I thought it would be the other way around (importing VR controls to the game) so that shows how VR is compatible with unity development. However, the simplicity of roll a ball definitely helps there. 


Some issues I encoutered:
Camera offset issue: I couldn't change the main camera position in the beginning so I had to move back 1m de have the board in front of me.

Grabbing Offset Issue: As we see in the gameplay footage, there is a snap offset when you grab the board,
https://forum.unity.com/threadsvr-oculus-sdk-touch-controller-snap-position-snap-offset-grab-a-gun.512853/

I tried to fix it by following this thread but the result was not there and I couldn't access the lab anymore but I think the solution is there.




