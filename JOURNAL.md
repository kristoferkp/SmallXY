---
title: "3D Printer (name tbd)"
author: "Kristofer P"
description: "A fast and sturdy cantilever 3D printer"
created_at: "2025-07-07"
---

**Write a story here**

# 1st entry: July 7th, 2025: Initial research and frame design.


Researching what parts to include in the 3D printer was a tough challenge to say the least.

First, I wanted to build a small coreXY printer, but after searching for the parts online (mainly AliExpress) and seeing what I already have on hand (basically nothing apart from a Raspberry Pi), I came to the conclusion that it will blow the $350USD budget.

So then, I decided to build a cantilever design for its simplicity and cost.
The main problem that seems to plague cantilever printers is instability.

As I wanted to build a fast machine, hopefully beating the Bambu Lab A1 mini, I decided to use 2040 aluminium extrusion as it is cheap and will probably give it the stability it needs.

I set my target to the Bambu Lab A1 mini. With its 180x180x180mm build volume, my machine would need to match that.

The heatbed options aren't very big on AliExpress (I found very little listings for 180mm heatbeds), so I decided to use a heatbed meant for the Micron+ printer.
There was a option of just using the Bambu Lab A1 mini heatbed unit as its price is very reasonable at €42, but with Bambu being so locked down, I couldn't find any information on it.
It probably is a 24V about 100W heater and some mystery thermistor. I would need to get my hands on one to find out.

I also searched for linear rails and landed on the MGN12H at 250mm long. They should be long enough for the 180mm bed and mounting stress. But I might swap them out for beefier rails down the line.

Found NEMA17 motors that should have enough torque to hold the X-axis up not during use. 17HS4401S.

Chose to use roll-in t-nuts for the linear rails. They are a bit more expensive than drop-in ones, but are way to save the hassle later on when building.

That was the end of the reasearch on that day.

---

I started off by searching for some 2020 and 2040 extrusion. Eyeballed the lengths to be 350mm for the Z, 150mm and 300mm for the bed, 400mm for the X-axis.

The extrusions will be joint together with joining plates. Maybe I will add some other joints, tbd.

Then I added the linear rails. The grabcad model was only 100mm long, so I had to extend it to 250mm. 

I do not know why, but Autodesk Fusion was playing tricks on me the entire time.

For the life of me, I couldn't understand why Fusion was chopping off parts of the entirely different bodies from different compontents.
When I tried splitting the 100mm rail to 50mm, it would split every single rail part and then when I went to delete the extra 50mm, the rail would suddenly have holes in them.

It happend in other areas too, like the extrusions. When I went to extend or cut an extrusion, the other extrusions would cut themself too.
I ended up somehow forcing myself through the problem, so if anyone has some ideas, let me know.

### Time spent on that day: 5h

![image1](/images/image1.png)

# 2nd entry: July 8th, 2025

Did some searching and came to the conclusion, that 2040 extrusion is too flimsy and decided to swap out the extrusions for 3060.
I also searched where I can buy the extrusions and found a polish shop that sells custom lenghts for a really reasonable price.

3060 for €0.30/cm and 2020 for €0.12/cm.

The bed has been a quite the headache. I can't really make my own bed as I do not have the equipment necessary, so I need to buy one pre-drilled and tapped.

I did find a Ratrig V-minion heatbed assembly, but noone has bought it so it is kinda risky.
The other option I found was the Micron180 heatbed assembly.

It has all the necessary things included for €60, but I might need to swap it out later when I optimize the BOM.

The Micron has a slight flaw for my use case, it is designed to be mounted fixed to the bottom of the printer. Which means, the mounting bracket that goes between the bed and the linear rail carriage has to be huge.

---

I started the day off with replacing the extrusions and fighting with Fusion a bit. I have managed to make sense of the problem a bit, but still kinda wonky.

The rails were next. They were less of an issue, but with the Fusion magic again, I am having a hard time categorizing the models into components. Please do not inspect the components too close.

The mounting brackets were next. I did several designs and L-shaped mounting brackets that I found on that polish website seems to be the best. I did add a T-shaped bracket to the bottom and normal corner brackets for reinforcment.

I found the CAD model for the Micron180 and just took the bed assembly out of the file. ;)

I did have to modify it, removing the extrusions, making a carrier plate for it, etc.

The carrier plate might actually not warp, I need to learn how the Fusion simulation works.
I have a feeling it will not hold up.

### Time spent on that day: 7h

![image2](/images/image2.png)

# 3rd entry: July 9th, 2025

I started the day researching again.

Looking over the BOM and the design, I think I can build an CoreXY for not a lot more and a lot faster and probably safer design wise.

The bed on the cantilever design is really suspicious.

I decided that I will make a flying bed and not a flying gantry.

The Z will use 4 linear rods and 2 Z-motors with screws.
This is because I only have 2 Z-motor drivers on the board and beacuse it is cheaper.

The Z will use 10mm linear rods, LM10UU and Nema17 motors with lead screws on them.

Hoping to find motors that aren't that expensive.

Found basically Prusa MK3 Z motors with built in 300mm lead screws, will use those.
They come on the printer in a 2 pack too, which is kinda amazing. The stars are slightly aligning.

There is a posibility of using some more Prusa motors. That makes the project a bit more accessable (if someone has MK3 motors lying around).

It is possible to use the MK3 bed and Y-carriage as well, but I don't have them and they are more expensive than the Micron180 bed I want to use.

The beds should be replaceable with a few design tweaks.

I also made the BOM a bit more complete and I am going to have to source a few parts myself beacuse the BOM is offically blown out of budget.

---

I started doing the CAD for the CoreXY printer.

I decided to use 2020 extrusion as there is more of it, so the rigidity shouldn't be a problem, and it is quite a lot cheaper.

The bottom of the printer is under review. I might make a skirt for the electronics or I house the electronics at the back of the printer.

I got the linear rods placed, the bed placed, the NEMA17 motor and its accompanying lead screw and the lead nut placed.
The second linear rods used to connect the lead screw and the Z-axis linear rods were also placed.

Next up I need to make the connecting piece that will be 3D printed.

I have realised that I really do like tinkering in Fusion and researching the parts. It is quite hard, but I like the challenge.

Aimlessly modeling is very time consuming, but when I achive the aim, it gets quite rapid.

### Time spent that day: 8h

![image3](/images/image3.png)