# BOM

There's an interactive BOM [here](https://djtersteegc.github.io/fujinet-adam-hardware/ibom-devkit-smd.html), I find them super useful when placing the SMD parts. 

I buy pretty much everthing from AliExpress suppliers with the exception of the tantalum capacitors (whatever is on clearance at Newark) and the ESP32 board (cheaper shipped from Amazon). If you are bulding in the "tall" configuration, you will also need some 2.54mm female headers.  I buy the 1x40p models and break when down into two 19 pin headers required by the devkit board.

C2 is a bulk storage cap for the 5V input from the ADAMNet line.  I speced it at 100uF, but anything from 22uF and up will probably be fine.  You may not even really need it.

C1 is to handle inrush and prevent sag and MCU reboots on the 3.3V rail if you are hot swapping your SD card.  Mozzwald's original design went without, so not strictly needed, especially if you don't plan on hot swapping the card.

# Assembly

Lay down all the SMD components first.  When complete, your board shoud look like this.

![devkit-smd-no-through-hole](../docs/devkit-smd-no-through-hole.jpg)

Next decide if you are building it on female headers or soldering the devkit directly to the board.  If the latter, there are some 3mm spacers and support blocks in the "short" 3D directory you can print out to space the devkit board correctly and keep the board level when you flip it over to solder it together.

![devkit-smd-spacers-support-blocks](../docs/devkit-smd-spacers-support-blocks.jpg)

![devkit-smd-level](../docs/devkit-smd-level.jpg)

Next solder on the two RJ12 jacks.  For the LED's, I first insert them in the PCB, then the PCB in the case, flip it over and support the case ~1mm off the surface for the LED's to just poke through the top and get a nice reveal. Solder one leg on the LED's, flip it over to check your spacing again, and then solder the other leg.

# Case

If built on female headers, print the files in the "tall" directory.  Make sure to print three buttons.  If soldering directly to the board spaced 3mm above it, use the case file in the "short" directory.  Assemble with two M2.5x10mm screws.

![devkit-smd-tall-designspark](../docs/devkit-smd-tall-designspark.png)

![devkit-smd-designspark](../docs/devkit-smd-designspark.png)