# EnderCNC

## VERY VERY BETA project.

### Got too many Enders laying around? Dont need a 5th Trident? Well! Try the EnderCNC, born from a lack of sleep, a wish to learn more CAD and too many spare parts floating around.

Based on the Ender 3 Pro frame, but if you buy extrusions you could scale it up without issues.(why would you even do that) If you have an old Ender or find one dirt cheap it might be a worthwhile build and a cheap CNC. Please dont go out buying a new Ender for this.

Its running Klipper, not the best for CNC but good enough for basic milling/engraving etc. And i cba learning another OS atm.

In my testing it had no issues with wood as to be expected. No issues cutting and engraving acrylics. Biggest surprise was that it could do aluminium with ease on a 150w 20$ dremel. More testing to be done.

## Things you can salvage from the Ender 3:

* Frame
* Motors
* PSU
* MCU
* Leadscrew
* leadscrew thread nut
* 1 length of belt
* handfull of screws
* limit switches (depin from their pcb)
* ptfe tube
* v wheels
* aluminium spacers from v wheels
* bed carriage ( see why lower down)


## What you probably need to buy:

* 2x 8MM ID bearings (correct dimensions to be added)
* 2x 400mm 10mm rods
* 2x lmu10 something bearings to be updated
* 400mm 2040 for x axis
* 2x 8mm ID 20t pulleys
* some length of 6mm belt
* assortment of screws
* cheap mgn9h (will update correct length)
* a Dremel higher w the better.(500+w spindel ~Ø55 would be sick tho anything bigger would eat too much cutting area)
* maybe a limit switch or two?
* 5mm id 20t pulleys
* closed loop belt to be updated, same as the M4 extruder 

## Printed parts:

* All parts are PLA, printed with voron recommend walls/infill. 
* X plates are 100% infill.

Dremel holder is designed for my spesific one. so unless you have a Biltema store near you , youll have to test fit yours or edit the dimensions. (if you have a biltema near get the MG150) its a clamp/screw mechanisms tho so might fit more types.

* only part that needs support is the z motor mount, but its not much.
* you should print out the lmu bearing test print to see that they fit snug. 



## Why all the random parts? 

This was never really ment to be shared as it was a personal pet project, it used 98% parts i had laying around and was made with those parts in mind, so thats why it has some
.. strange choices. 

## Weakpoints: (so far)

* Youll have to extend stepper wires. 
* 10mm rods are probably not the best
* v wheels on x axis
* x plates are printed ( see more info lower)
* x/z carriage homes "over" the y extrusions, causing you to crash into the side of the extrusion when z is low. In my "beta" one i have X0 10mm away from the limit switch and 10mm less max travel on X max, this means Z will always have to home first, see my home overwrite macro. This will be fixed in a V2 when that time comes.

## X carriage plates: 

X plates are printed, front one is mounted to mgn9 rails and stiff enough, back x plate is not stiff enough and should be the first part you mill out of aluminum once its up and running and found your feeds/speeds. Or you could print out a 1:1 scale of the x_back_plate.dxf on a sheet of paper, glue it to a piece of aluminium and do it by hand/bandsaw/drillpress etc.
Dont have any aluminium? well thats why the x plates are 4mm, and so is your enders bed carriage! 


## Whats to come?
* (no promise, please help me with mods lol) 

* MNG12/15H for Y axis, 2 blocks pr side or thicker rods with 2x bearings on each side.
* MGN12/15H for X axis , pref 2 rails 4 blocks.
or any other types of beefy rails really.

My plan is to add 2 more versions, one using only v wheels from the ender on all axis for a super cheap build, and one for mgn rails on all axis as a "i hate my money" option. 


## Closing words:

My first real project in fusion, so there might be issues here and there. Any suggestions and help is greatly appreciated. You are free to remix and mod as much as you want, just show me what you made \o/ Be safe, dont crash it too hard.
