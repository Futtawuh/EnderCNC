# EnderCNC

# Currently undergoing a facelift to all printed parts and additional QOL features. MGN rails version will also be released after the orginal version with facelift is out of beta. 

# Always check out the [Changelog](https://github.com/Futtawuh/EnderCNC/blob/main/Changelog.md) for any updates done to the CAD. 

## VERY VERY BETA project. 
(image of the new facelift version, check [Changelog](https://github.com/Futtawuh/EnderCNC/blob/main/Changelog.md) for info)
![image](https://github.com/user-attachments/assets/7ce10dc6-d56f-4962-9f77-364592733cd6)






https://github.com/user-attachments/assets/92859aa1-7ed4-4385-81ab-ec51dbf1d837

https://github.com/user-attachments/assets/d6dc1093-e1e1-4dbe-b1f9-021c9d8749b4

# (Residue on the bit is just sticky-tape from doing the holes)

https://github.com/user-attachments/assets/a4f48e41-3836-4eb9-8406-88c55c8b1824

![part](https://github.com/user-attachments/assets/84995a64-6b96-4889-8dd5-63da7fdcb275)




### Got too many Enders laying around? Dont need a [5th Trident?](https://github.com/yell3D/Ender3dent) Well! Try the EnderCNC, born from a lack of sleep, a wish to learn more CAD and too many spare parts floating around.

Mostly based on the Ender 3 PRO 3D printer. If you have an old Ender 3 PRO or find one dirt cheap it might be a worthwhile build and a cheap CNC. Please dont go out buying a new Ender 3 PRO for this.

Its running Klipper, not the best for CNC but good enough for basic milling/engraving etc.

In my testing it had no issues with wood as to be expected. No issues cutting and engraving acrylics. Biggest surprise was that it could do aluminium with ease on a 150w 20$ dremel. More testing to be done.

## Things you can salvage from the Ender 3 PRO:

* Frame
* Steppers
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
* some wires


## What you probably need to buy:

* 2x 8MM ID bearings (8x22x7)
* 4x F695 ZZ bearings (could use 2x GT2 non-teeth pulleys)
* 2x 400mm Ø10mm rods
* 2x LMK10LUU (55mm long bearings) 
* 400mm V SLOT 2040 for x axis
* 2x 8mm ID 20teeth pulleys
* some length of 6mm belt (to be updated, but not much needed)
* assortment of nuts and bolts (to be updated)
* m5 T-nuts or m5 roll'ins.
* MGN9H - 2x blocks, 2x 120mm rails, accoring to CAD you can get away with 2x 100mm rails but this is NOT tested.  
* a Dremel higher w the better.(500+w spindel ~Ø55 would be sick tho anything bigger would eat too much cutting area)
* Maybe a limit switch or two? ( X - YY - Z)
* 5mm id 20teeth pulleys
* GT2 Belt Loop (6mm wide) - 188mm
* Heat inserts M3x5x4
* Raspberry pi. (If you can find an old laptop for free/cheap, install Ubuntu on that and install klipper/mainsail etc on that as a cheap Rpi) 
* ### (I had all these parts laying around from older projects)

## Printed parts:

* All parts are PLA, printed with voron recommend walls/infill. 
* X plates are 100% infill.
* Dremel holder is designed for my spesific one. so unless you have a Biltema store near you , youll have to test fit yours or edit the dimensions. (if you have a biltema near get the MG150) its a clamp/screw mechanism, so might fit more types of dremels.
* Only part that needs support is the z motor mount, but its not much.

## Weakpoints: (so far)
 
* 10mm rods are probably not the best
* v wheels on x axis
* Obviously the Dremel, locked into 3.1mm shaft bits, but still good enough for aluminium.
* x plates are printed ( see more info lower) 

## X carriage plates: 

X plates are printed, front one is mounted to mgn9 rails and stiff enough, back x plate is not stiff enough and should be the first part you mill out of aluminum once its up and running and found your feeds/speeds. Or you could print out a 1:1 scale of the x_back_plate.dxf on a sheet of paper, glue it to a piece of aluminium and do it by hand/bandsaw/drillpress etc. (See DXF folder for .dxf or .pdf)
Dont have any aluminium? well thats why the x plate is 4mm, and so is your enders bed carriage! Just be sure to use the correct holes during assembly. You can go for a thicker back plate, but youll need longer flathead screws for the wheels.
![image](https://github.com/user-attachments/assets/c4f19946-c595-4232-bdd7-9e3ad63d106a)


## Whats to come?
* (no promises, please help me with mods lol) 
* Basic build guide?
* Vacuum attachment.
* Basic FW for SKR pico, Creality 4.2.2/4.2.7
* Basic Macros for Klipper
* Slimmer Z carriage.
* MCU case for the Creality 4.2.2/4.2.7 boards. (I used a SKR pico)
* PSU case for Ender 3 PSU. (i used another spare)
* MGN12/15H for Y axis, 2 blocks pr side or thicker rods with 2x bearings on each side.
* MGN12/15H for X axis , pref 2 rails 4 blocks.
or any other types of beefy rails really.
* LED/RGB for max speed?

## Why all the random parts? 

This was never really ment to be shared as it was a personal pet project, it used 98% parts i had laying around and was made with those parts in mind, so thats why it has some
.. strange choices. My goal was to not spend a lot of money, it cost me around 20$ in nuts and bolts.

## Mods:

You are free to remix and mod as much as you want, just show me what you made and we'll add it to the Mods folder with full credit to the author of the mod.

## Closing words:

Any suggestions,help and feedback is greatly appreciated. Be safe, add an emergency stop and dont crash it too hard.
# Discord: ravenkeeper
