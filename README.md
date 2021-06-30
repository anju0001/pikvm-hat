
# PIKVM HAT

This repo contains all the files you need to produce your own super cheap pikvm hat.
Originally, the pikvm creators used  ORMOM G3VM-61A1 solid state relays for connection to the ATX header. They are very good, but also very expensive. 
I created this pikvm hat for the Rapsberry Pi with focus on price and dimensions, that is why I replaced the OMROM parts with super cheap 4N33 optocouplers.
The PCB is small enough to fit in this pikvm case from thingiverse:
https://www.thingiverse.com/thing:4704821

## Files

In the **gerber** directory you will find all files that are needed for production by a PCB factory.
The directory contains all the single files but as well a ZIP file that you can upload to whatever PCB manufacturer you like. Most factories want you to upload the files as a ZIP archive.

The file **assembly.jpg** in the root directory shows how to assemble the finished PCB.

## Assembly/BOM

What you need to assemble this project:

 - 1x PCB
 - 1x double row 9 pin (2x9) pin header
 - 4x 4N33 optocoupler
 - 4x single row 2 pin (1x2) pin header
 - 4x 220R resistor (R1-R4)
 - 2x 4k7 resistor (R5+R6)
 
That is all. Be aware, the 2x9 pin header has to be soldered in from **the bottom**, this has to be a Raspberry hat after all :) Also check for short circuits, expecially if you use heat sinks on the Raspberry! The hat might touch the heat sinks if they are too high.

## Connecting

The 1x2 pin headers are for connecting the PCB to the ATX headers of your mainboard.

    PWR -> Power button
    RST -> Reset button
    PLD -> Power LED
    IDL -> IDE/HDD LED

Be careful to not mix up the positive/negative terminals, so + on the PCB has to be connected to + on the mainboard.

## Problems

Nothing is working? Get a magnifier and check for solder bridges, short circuits, etc. This PCB has been produced and assembled many times and works very nicely.

## License

Free for **non-commercial** use only. If you want to use this commercially or sell this PCB, you **must** contact me first for clarification of terms!
In this case write an email to info@aj.de

