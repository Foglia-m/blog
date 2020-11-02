+++
title = 'Lab 1: Setting up the blog with hugo and github'
date = 2020-11-02T16:32:38+01:00
draft = false
description = "the goal here is to describe how I managed to set up the blog by following tutorials"
showFullContent = false
+++

Building your local blog using hugo:

Hugo is really easy to handle (at least the basics) and makes the development of a blog so easy. I started working in local in order to see how things worked ( posts, config, image and so on)
It was all very smooth in local as I never encountered issues following the geting started tutorial from the hugo website https://gohugo.io/getting-started/
I'd advise using a WSL (windows Sub Linux) with linux to work on it but this is general to any command line based project. Perhaps you'll have to fix some local host path going this way but it's no big deal.

Hosting on a remote repository:
The troubles started when I had to go online:
I hosted it on GitHub following this tutorial: https://gohugo.io/hosting-and-deployment/hosting-on-github/ and everything was smooth if you're not a git noob, frankly I only know the basics(which are fast to learn but hard to master) and it was easy to do.
Unfortunately, I encountered issues with pictures because the paths wouldn't respect what I wrote in my code:
It turned /blog/N64.jpg into /N64.jpg for example and therefore the resource could not load.

Fix:


Unity setup:
It's so easy and user friendly at the beginning that you wonder how you never used it as a kid when you start, playing around with the pre-coded fps was a lot of fun and start to modify its code was also easy to do and a good "first grasp" learning approach. 
