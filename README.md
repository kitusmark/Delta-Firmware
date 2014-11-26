Delta-Firmware
==============

###Introduction 

I've forked the Marlin Firmware of the [BCN3DR](http://www.reprapbcn.com/es/catalog/bcn3dr) Delta printer from [RepRapBCN](http://www.reprapbcn.com) in order to work in some improvements:

1. Auto Bed Leveling with FSR (Force Sensing Resistors).
2. Out Of Filament Detector. Just an endstop detecting if there's filament or not and triggering M600 to be able to change the Spool.
3. Cool Pause function with parking functionalities.

These functionalies are implemented thinking in the future where I'll be adding some remote host server to the printer like [Octoprint](http://www.octoprint.org).

###Auto Bed Leveling

This implementation is based on some work by @jcrocholl in his Marlin fork and in the [Kossel branch](https://github.com/jcrocholl/Marlin/tree/kossel)


###Out of Filament Detector

This is even simpler. Guiding the filament through an Endstop, if the endstop is not triggered it means we ran out of filament. This function uses M600 to be able to change the Spool and keep on going with your print.


