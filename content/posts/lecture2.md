+++
title = "History of HCI, Input Devices and User Interfaces"
date = "05/10/2020"
author = "Milan"
authorTwitter = "" #do not include @
cover = ""
tags = ["", ""]
keywords = ["", ""]
description = ""
showFullContent = false
+++

google scholar link: https://scholar.google.com/citations?user=BXCGQXwAAAAJ&hl=en
A great researcher in HCI is HRVOJE BENKO, his work revolves around haptics, VR and AR, projection room interaction and input devices. He is the current director of research in Facebook Reality labs Research.
He is very active in many fields of VR and HCI as he publishes regularly over the years. 
The paper I want to present is about weight perception in VR using pseudo haptics techniques to simulate weight for the user: http://www.hbenko.com/#PseudoHapticWeight .

The reason why I chose this paper is because the weight issue was a bummer for me in VR games (skyrim for instance or even throwing stuff to enemies in superhot) because each time I felt no weight, I experienced instant dissonance and the environment definitely felt like a simulation despite the fact that I was sweating to dodge a bullet 3 seconds before as if my life was at stake. This is the basic pipeline of how a specific bad immersion affects the overall presence of a VR game.
 From a more general standpoint, pseudo haptics could potentially enhance results of medical use of VR as in reeducation sessions for instance.
I think the idea to tackle the issue with pseudo haptics (an illusory perception of feedback) instead of grounded haptic devices is relevant as better computed simulation is always more convenient to deploy than real world devices such as real haptics (another idea Benko managed to test in this 2018 paper which quite confirms how all around this scientist is in this field: http://www.hbenko.com/publications/2018/Strasnik_Haptic%20Links_2018.pdf)


The paper revolves around finding the perception of weight through the control to display  (C/D) ratio seeking the most accurate C/D ratio which was made possible by transferring the weight perception to a true physical work estimation problem. Then they experimented on the problem to extract a predictive model of weight perception.
The first experiment’s goal was to leverage the user’s sensation of weight for two identical cubes but with different C/D ratios in the simulation. The participants concluded that the cube with the C/D ratio inferior to 1 was heavier, whereas the C/D>1 ratio cube felt lighter. 

![CDratio](/blog/CDratio.jpg)	

This graph shows how the C/D ratio was changed and the offset of movement that was accordingly applied to the cube. (a.u. stands for arbitrary units).

Then they ask participants to adjust the weight of a cube according to their perception, as they created a model of the relation between C/D ratio and perceived mass.

![CDratio2](/blog/CDratioandoffset.jpg)

Their data fits the model quite well.

What can we conclude?

Applying this model to games such as skyrim VR could enhance the simulation and doesn’t require any specific hardware. It’s just a matter of finding a correct model and correctly implementing it in order to trick the user. Therefore I hope to see a general use of pseudo haptics in VR games as poor weight perception has always been an immersion killer.


the Ultimate Display by Ivan Sutherland, 1965
link: http://citeseer.ist.psu.edu/viewdoc/summary?doi=10.1.1.136.3720

The now basic area-filling capability is done by every display device we have since macintosh 128K (1984)
The interaction with a computer through a typewriter (which became a keyboard) comes from the same era.
The idea to use the UI described as “point to the first and "drag" it over to the second” is one of the key elements of WIMP and has been established around the macintosh era too.  
Stylus are now fingers on smartphones/tablets
voice input: here in every smartphone/alexa but not that much used 
coordinates are now easy to handle for computers and WIMP programming is all about coordinates. So the Rand Stylus with its signal has been obsolete since then.
Every display equipment now perfectly handles the recursion of memory between the interface and every layer of the program.

Therefore, we can assume that we’ve already reached what Ivan Sutherland considered as the perfect display. However, something is lacking to reach the idea of ultimate display.

He considers for instance senses (smell, taste) which are not part of our current displays.
It is therefore interesting to look into what he named kinesthetic display as its application to VR is at the core of current research in the field.
For instance, the depletion of the force modelized in VR to a real world interaction with the user is one of the main current challenges of VR immersion. (playing skyrim with a 50 grams Long sword quickly gives away the simulation. We must look into the haptic feedback field to find answers to this idea (http://www.hbenko.com/)

“make the display presentation depend on where we look.” This relates to VR as the headset monitors movement and position but it can also refers to more diverse devices such as pure eye tracking without a VR headset which is a current research field in VR.


Another point he makes is the ability for computers to display mathematics law that we can’t grasp in reality as they go beyond our perception of the world (mostly for dimensions reasons) To follow his idea of computer being the window of fundamental physics and maths for human beings, we can think of programs that could display non euclidian worlds as it could serve research. But wait it does exist: https://www.youtube.com/watch?v=P6sB00nkoeM&ab_channel=Creslex there’s a non euclidian minecraft mod that I must look into in order to analyse it. This type of displays could be a great tool for education and in a broader way, enable our capacity to think outside the box and beyond our common senses.
![noneuclidian](/blog/noneuclidian.jpg)	

Finally, the true ultimate display is one that interferes in the real world as it controls the matter in the room, such display has never been released as of today and we can’t possibly think of it in the near future. Although the elementary bricks are quite present with the combination of VR and 3D printers we could imagine a room where the user can create and interact with matter such as a real life minecraft version but how dangerous would that be? 



TIPTEXT: An Input Device for the future

TipText is the best paper award winner of 2019 UIST, I thought it was interesting to analyse the paper receiving the award as it can be a synonym for trend or at least direction of the current research. On top of that, this input device combines mobility and a VR compatible input which can explain its importance in the near future. We can directly see why by looking to its presentation:
https://www.youtube.com/watch?v=i3YPZsiHEKM&ab_channel=HCIResearch%40Dartmouth

We can define it as a compact touch input device.
Pros:
 -As I mentioned, the best asset of this device is about it’s perfect compatibility with every challenging input compatibility with new tech such as VR,AR and smartphones. It’s definitely a device that we could consider as problem solving for many compatibility issues as it requires no particular surface except for the fingers we all have, there’s almost no movement required so it basically adds no constraint at all for its use.
-The eyes-free aspect is also quite rare in the input device field and add another layer of simplicity and compatibility in our everyday life which could mean its extension to daily user input for smartphones, tablets, cars and any possible IOT device we could think of.


Cons:
-The first con we can think of is the time required to handle such input (especially with the eyes-free parameters that makes it tough to really assess. Although their prototypes results look quite promising.

-Moreover, the fat finger problem (clarity issue) is definitely the main issue to consider regarding this input device so it must be widely tested before judging its true capacity. 


-Their data comes from relatively constrained study with 3d models of the finger of each tester. Applying the 3d model to a broader solution can be tricky.
I can’t see other possible issues but we can presume that daily use could eventually show issues that couldn't be grasped prior to it’s launch. 

-Last but not least, the WPM factor is at the core of new input devices, they achieve results up to 13.3 WPM which is a third of what we currently achieve on smartphones and a fourth of average computer typing speed according to this review: https://businesstech.co.za/news/mobile/344078/can-you-type-faster-than-a-teenager-on-your-mobile-phone-take-this-test-to-find-out/#:~:text=On%20average%2C%20mobile%20users%20were,both%20desktop%20and%20mobile%20devices.
We can imagine further improvements in the sensing technique to address this issue but it could potentially be the dead weight of this solution as it seems hard to go beyond this cap. 

Solutions?
To address these issues they considered several keyboard layouts on the fingertip: 
Basic QWERTY with statistical decoder
Multi Letter keys which comes with auto word-candidates such as those implemented in  older phones but a more statistical/ IA approach could improve this solution.
The best solution seems to be the multi letter keys with custom assignation of letters:

Time to handle: their evaluation seems to demonstrate increasing speed in typing over time so it now has to be tested by the public in order to truly demonstrate its suitability to a broad market solution.
Longer presentation of the solution: https://www.youtube.com/watch?v=e4-tANkReyw&ab_channel=ACMSIGCHI


