---
title: "3D Printer (name tbd)"
author: "Kristofer P"
description: "A fast and sturdy cantilever 3D printer"
created_at: "2025-07-07"
---

**Write a story here**

# July 7th, 2025: Initial research and frame design.


## Research
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

## Modelling the frame

I started off by searching for some 2020 and 2040 extrusion. Eyeballed the lengths to be 350mm for the Z, 150mm and 300mm for the bed, 400mm for the X-axis.

The extrusions will be joint together with joining plates. Maybe I will add some other joints, tbd.

Then I added the linear rails. The grabcad model was only 100mm long, so I had to extend it to 250mm. 

![image](https://github.com/user-attachments/assets/ab50a9eb-805e-49bb-9279-829c70bc4f63)

I do not know why, but Autodesk Fusion was playing tricks on me the entire time.

For the life of me, I couldn't understand why Fusion was chopping off parts of the entirely different bodies from different compontents.
When I tried splitting the 100mm rail to 50mm, it would split every single rail part and then when I went to delete the extra 50mm, the rail would suddenly have holes in them.

It happend in other areas too, like the extrusions. When I went to extend or cut an extrusion, the other extrusions would cut themself too.
I ended up somehow forcing myself through the problem, so if anyone has some ideas, let me know.

### Time spent on that day: 5h

# July 8th, 2025

## Research
Did some searching and came to the conclusion, that 2040 extrusion is too flimsy and decided to swap out the extrusions for 3060.
I also searched where I can buy the extrusions and found a polish shop that sells custom lenghts for a really reasonable price.

3060 for €0.30/cm and 2020 for €0.12/cm.



## CAD
![image](https://github.com/user-attachments/assets/bdf5d816-22e4-4b29-aa4c-e2eab1726dfe)



