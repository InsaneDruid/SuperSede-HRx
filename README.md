# SuperSede-HRx - a HRx clone family
A 100% compatible replica of the HR40, HR40B &amp; HR80 graphics boards for the CBM PET lineup.


The SuperSede HRx are 100% compatible clones of the HR40, HR40B and HR80 graphics boards for the PET/CBM series computers from 1982, beginning with the dynamic board.
They implements all the features, including the high 320*200 pixel high resolution graphics that can be mixed standard text output on a per character base, the availability of the 8k of onboard RAM for Data usage and the possibility to use existing ROM expansion on the graphics board.

## The HR40 board for the non CRTC 40column dynamic PET lineup
![HR40 render](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40/images/hr40_render.png)

[Schematic](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40/hr40.pdf "Schematic")  

[Bill of Materials](https://htmlpreview.github.io/?https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40/bom/hr40_bom.html "Bill of Materials")

[Wire connections](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40/hr40_connections.pdf "Wire connections" )

* The connection to the Character ROM can be made with a standard DIP24 to ribbon cable adapter.

* The connection to UF8 can be made with the provided breakout adapter found in [adapter_uf8](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/adapter_uf8/ "adapter_uf8").

## The HR40b board for the CRTC based 40column PET/CBM lineup
![HR40B render](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40b/images/hr40b_render.png)

[Schematic](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40b/hr40b.pdf "Schematic")  

[Bill of Materials](https://htmlpreview.github.io/?https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40b/bom/hr40b_bom.html "Bill of Materials")

[Wire connections](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr40b/hr40b_connections.pdf "Wire connections" )

* The connection to the CRTC can be made with the provided breakout adapter found in [adapter_crtc](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/adapter_crtc/ "adapter_crtc").

## The HR80 board for the 80column CBM lineup (8032, 8032SK*, 8096)
![HR80 render](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr80/images/hr80_render.png)

[Schematic](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr80/hr80.pdf "Schematic")  

[Bill of Materials](https://htmlpreview.github.io/?https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr80/bom/hr80_bom.html "Bill of Materials")

[Wire connections](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/hr80/hr80_connections.pdf "Wire connections" )

* The connection to the CRTC can be made with the provided breakout adapter found in [adapter_crtc](https://github.com/InsaneDruid/SuperSede-HRx/blob/main/adapter_crtc/ "adapter_crtc").

## The SuperSede cards and Expansion ROMs
The SuperSede boards hav 8k of their own RAM which occupies memory locations 36864 to 45055 ($9000 to $AFFF). This is the Rom Expansion area, normally represented by sockets UD11 and UD12 (UD3 and UD4 for 9-inch PETs). 

When you power-up your computer the ROM sockets are enabled and the high resolution memory disabled. Thus Rom expansions can be used in standard text mode like normal.

## The Firmware
The firmware needed for the SuperSede cards consist of

* A modified CharRom (with inverted characters).
* A 4k ROM containing the EditorROM followed by the GRAPHIX software in the E900-EFFF area.

The Firmware and supporting tools are available on their own repository: [SuperSede-HRx-Software](https://github.com/InsaneDruid/SuperSede-HRx-Software/ "Firmware and tools for the SuperSede HRx boards ")

## The License
This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.   
See https://creativecommons.org/licenses/by-sa/4.0/.

## The Credits
This work would not have been possible without the help from a bunch of amazing people from [VzEkC e. V. forums](https://forum.classic-computing.de/forum/ "forum.classic-computing.de"). Many thanks go out to:

* *Andy Grady* - for the scans of a blank board that formed the backbone for this project, the construction of the first prototypes as well as writing the print routines and assembling the firmware for the cards.
* *Steve Gray* - for collecting a ton of information about the cards
* *CBM_Ba* and *Richy* - for prototyping, testing, feedback and general positive retrocomputing craziness
