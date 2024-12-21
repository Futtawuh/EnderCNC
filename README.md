# EnderCNC

## VERY VERY BETA project.

![image](https://github.com/user-attachments/assets/de257c63-5e4d-4829-91a2-60f41d26e5db)




https://github.com/user-attachments/assets/d6dc1093-e1e1-4dbe-b1f9-021c9d8749b4


### Got too many Enders laying around? Dont need a [5th Trident?](https://github.com/yell3D/Ender3dent) Well! Try the EnderCNC, born from a lack of sleep, a wish to learn more CAD and too many spare parts floating around.

Based on the Ender 3 Pro frame, but if you buy extrusions you could scale it up without issues.(why would you even do that) If you have an old Ender or find one dirt cheap it might be a worthwhile build and a cheap CNC. Please dont go out buying a new Ender for this.

Its running Klipper, not the best for CNC but good enough for basic milling/engraving etc.

In my testing it had no issues with wood as to be expected. No issues cutting and engraving acrylics. Biggest surprise was that it could do aluminium with ease on a 150w 20$ dremel. More testing to be done.

## Things you can salvage from the Ender 3:

* Frame
* Motors
* PSU
* MCU
* Leadscrew
* leadscrew thread nut
* 1 length of belt (just buy new for all axis)
* handfull of screws
* limit switches (depin from their pcb)
* ptfe tube (used as "dragchain")
* v wheels
* aluminium spacers from v wheels
* bed carriage ( see why lower down)


## What you probably need to buy:

* 2x 8MM ID bearings (8x22x7)
* 4x F695 ZZ bearings
* 2x 400mm Ø10mm rods
* 2x LMK10L (55mm long bearings) 
* 400mm 2040 for x axis
* 2x 8mm ID 20t pulleys
* some length of 6mm belt (to be updated, but not much needed)
* assortment of nuts and bolts (to be updated)
* MGN9H - 2x blocks, 2x 120mm rails, accoring to CAD you can get away with 2x 100mm rails but this is NOT tested.  
* a Dremel higher w the better.(500+w spindel ~Ø55 would be sick tho anything bigger would eat too much cutting area)
* Maybe a limit switch or two? ( X - YY - Z)
* 5mm id 20t pulleys
* GT2 Belt Loop (6mm wide) - 188mm
* Heat inserts M3x5x4
* Raspberry pi. (If you can find an old laptop for free/cheap, install Ubuntu on that and install klipper/mainsail etc on that as a cheap Rpi) 
  (I had all these parts laying around from older projects)

## Printed parts:

* All parts are PLA, printed with voron recommend walls/infill. 
* X plates are 100% infill.
* Dremel holder is designed for my spesific one. so unless you have a Biltema store near you , youll have to test fit yours or edit the dimensions. (if you have a biltema near get the MG150) its a clamp/screw mechanisms tho so might fit more types.
* Only part that needs support is the z motor mount, but its not much.
* You should print out the lmu bearing test print to see that they fit snug. (to be added)



## Why all the random parts? 

This was never really ment to be shared as it was a personal pet project, it used 98% parts i had laying around and was made with those parts in mind, so thats why it has some
.. strange choices. My goal was to not spend a lot of money, it cost me around 20$ in nuts, bolts and 8mm ID bearings/pulleys.  (not counting price for parts i had on hand)

## Weakpoints: (so far)

* Youll have to extend stepper wires. 
* 10mm rods are probably not the best
* v wheels on x axis
* x plates are printed ( see more info lower)
* x/z carriage homes "over" the y extrusions, causing you to crash into the side of the extrusion when z is low. In my "beta" one i have X0 10mm away from the limit switch and 10mm less max travel on X max, this means Z will always have to home first, see my home overwrite macro. This should be fixed in a CAD but not tested with new parts. 

## X carriage plates: 

X plates are printed, front one is mounted to mgn9 rails and stiff enough, back x plate is not stiff enough and should be the first part you mill out of aluminum once its up and running and found your feeds/speeds. Or you could print out a 1:1 scale of the x_back_plate.dxf on a sheet of paper, glue it to a piece of aluminium and do it by hand/bandsaw/drillpress etc.
Dont have any aluminium? well thats why the x plate is 4mm, and so is your enders bed carriage! Just be sure to only use the correct holes during assembly. 
![image](https://github.com/user-attachments/assets/c4f19946-c595-4232-bdd7-9e3ad63d106a)



## Whats to come?
* (no promises, please help me with mods lol) 
* Vacuum attachment.
* Slimmer Z carriage.
* MCU case for the Creality 4.2.2/4.2.7 boards. (I used a SKR pico)
* PSU case for Ender 3 PSU. (i used another spare)
* MNG12/15H for Y axis, 2 blocks pr side or thicker rods with 2x bearings on each side.
* MGN12/15H for X axis , pref 2 rails 4 blocks.
or any other types of beefy rails really.
* LED/RGB for max speed.


My plan is to add 2 more versions, one using only v wheels from the Ender on all axis for a super cheap build, and one for MGN rails on all axis as a "i hate my money" option. 


## Closing words:

My first real project in fusion, so there might be issues here and there. Any suggestions and help is greatly appreciated. You are free to remix and mod as much as you want, just show me what you made \o/ Be safe, add an emergency stop and dont crash it too hard.
