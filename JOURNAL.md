---
title: "Kiloan P1M"
author: "Kian Lorenz"
description: "Custom CoreXY printer with changeable toolheads for 3D printing and laser engraving or cutting."
created_at: "2025-06-15"
---

**Total time spent: 28.5hrs**

# June 15th - Planning the concept (0.5hrs)

After I had a rough idea of ​​what I wanted to build, I wrote down my ideas. The goal is to design an inexpensive and simple CoreXY printer and construct it so that the print head can be replaced with a laser. I've had this idea for a few months now and am now taking this opportunity to implement it. The printer should be usable with and without an enclosure.

- Aluminum frame (2020)
- CoreXY
- should be easily scalable
- swapable toolheads (FDM and Laser)
- autoleveling
- emergency stop
- full enclosure
- Nema 17 Motors if possible

![Frame Idea](images/frame.jpeg)

# June 15th - Frame and Z-Axis (10hrs)

I learned from YouTube how a typical CoreXY printer is constructed. Then I started designing in Fusion360. After the frame, I continued with the Z-axis. In my mind, this design should work well and print semi-well (i am learning cad with this project). The system uses a trapezoidal lead screw and the corresponding TR8x4 trapezoidal lead nut to move the Z-axis up and down, attached to linear guides. Nema 17 motors are used because they are inexpensive in my area.

![z-axis](images/z-axis.jpeg)

A 3D printed holder is screwed into the aluminum extrusion at all three points at the top. The linear rail is then attached to this holder. Another holder is screwed on and fitted with a ball bearing so that the trapezoidal lead screw is held and can rotate freely.

![z-axis-top](images/z-axis-top.jpeg)

Below, a 3D-printed holder is screwed to the aluminum extrusion where the linear rail and motor are attached. The trapezoidal lead screw is attached to the motor via a 5mm to 8mm coupling, and the weight is distributed across the motor housing via a ball bearing with a washer to prevent excessive strain on the shaft. On the carriage, which sits on the linear rail, there is another 3D-printed holder that holds the trapezoidal lead screw nut and onto which the aluminum extrusion frame is screwed, upon which the print bed is then placed.

![z-axis-buttom](images/z-axis-buttom.jpeg)

The aluminum extrusion frame for the print bed is held together with simple 3D printed plates.

![BedFrame](images/bedMountConnectors.jpeg)

# June 18th - XY-Axis (6.5hrs)

After a few school exams, I was finally able to move on to the remaining axes. The Y-axis already has two linear rails, and I've finished the 3D-printed mounts. These include space for screwing the two idler pulleys at two different heights for the two belt loops. I also learned today how the corexy system works exactly; YouTube was my best source of help.

![xy-axis-1](images/xy-axis-1.jpeg)

The entire CAD project looks like this so far.

![so-far1](images/so-far1.jpeg)

# June 22th - XY-Axis finis, learning and PrintHead (11.5hrs)

I've finally finished the end pieces for the XY axis. The middle plate holder is only loosely attached and, as mentioned, serves only as an intermediate piece to adjust the two idler pulleys to the correct distance. They've become a bit bulkier, but I think that gives the whole thing more stability and hopefully they will be easy to 3D print.

![xy-endthings](images/xy-endthings.jpeg)

Next come the motor mounts, which are very simply made. You screw the NEMA 17 motor to the upper U-shaped part and attach it to the base plate. Now, with a bit of fiddling, you need to attach the base plate to the aluminum extrusions. Finally, you can screw the pulley to the motor shaft.

![xy-motors](images/xy-motors.jpeg)

And now the XY axis looks like this. The Y axis needs to be adjusted because I didn't make any provision for leveling the print bed. So, I'll make the previously designed guides with linear rails at all four corners and add joints at all four corners to level the bed. Similar to a 5-axis 3D printer design.

![so-far2](images/so-far2.jpeg)

I've decided against the simple Creality CR10S extruder or the similar Ender 3 extruder. For direct extrusion, I'll use the dual gear BMG extruder or a cheap clone to minimize overall costs. I'll attach any NEMA 17 motor that's no longer than 48 centimeters to it, so I can enclose the printer later. With a small adapter, I can use the Bambu X1C hotend. For the electronics, I'd like to use a small control board on the print head, but I don't yet know how complicated that would be.

![printhead-components](images/printhead-components.jpeg)