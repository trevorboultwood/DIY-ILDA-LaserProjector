# DIY-ILDA-LaserProjector
A fully DIY laser projector system ILDA* compatible

Do you like:
Playing with Lasers?
Writing code?
Dangerous electronics?

Then you'll love this project.


This Git contains 3 folders, Hardware, Firmware & Software.

Introduction

Insert here.


The hardware folder contains the system overview as well as the schematic used to connect the various parts together.

The firmware folder contains the very basic ESP32 arduino project used to sample the DAC and produce PWM signals based on its readings. Why not do this over serial? One day I hope to do exactly this.


The software folder contains the Visual Studio C# project used to import and playback .ilda / .ild files to the laser projector. Essentially this is a 5.1 surround sound audio generator and playback and requires NAudio. The software decodes .ilda files and generates an xyRGB array which is then converted to analog world and playedback. Sadly I never managed to discover a way of doing this real time and therefore each file is decoded/encoded and then played.

