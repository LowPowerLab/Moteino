# Moteino/MoteinoMEGA Arduino core files for Atmega328P/ATmega1284P based Moteinos

# * ~~~ Obsolete ~~~ *
See new instructions to get Moteino Core in the [Moteino guide](https://lowpowerlab.com/guide/moteino/programming-libraries/).

## What is it?
Everything you need to run a ATmega1284P based Moteino MEGA from the Arduino IDE.
Added regular Moteino variant based on the prolific ATmega328p.

## Status
* This Arduino core contains the ATmega1284P MoteinoMEGA variant and the ATmega328p Moteino variant (added Nov 2014) along with the DualOptiboot bootloaders.
* The platform now includes Dualoptiboot for ATmega1284P and ATmega328p which support [wireless programming](https://lowpowerlab.com/guide/moteino/wireless-programming/) (C) by Felix Rusu of LowPowerLab.com
* Last updated: Aug 24, 2016.

## License
This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details. View full license text at: http://www.gnu.org/licenses/gpl-3.0.txt

##Install Update
* This guide and package is only relevant for manual installs on IDE 1.6+ or the older 1.0.6.
* Arduino IDE 1.6.4+ has a board manager that makes it really easy to add the board definitions, instead of using these ZIP files. For installing via BoardManager in IDE 1.6.4+, see [this guide](https://lowpowerlab.com/moteino/#programming).

## Installation
0. Ensure you are running Arduino 1.6.0 or greater (this was tested on Arduino 1.6.9). For Arduino 1.0.6 use the Moteino_1.0.6.zip instead, read below.
1. Download the root of this repository [from here](https://github.com/LowPowerLab/Moteino) (find the "Clone or Download" button), then extract the Moteino core [ZIP File](https://github.com/LowPowerLab/Moteino/blob/master/MEGA/Core/Moteino.zip) from that. If you run the 1.0.6 release get the Moteino_1.0.6.zip instead.
2. From the master ZIP archive of the whole repository, find the [corresponding Moteino.zip file](https://github.com/LowPowerLab/Moteino/blob/master/MEGA/Core/Moteino.zip)
3. Unzip the content of the Moteino.zip into a folder called 'hardware' located in your sketches directory, e.g. /Users/felix/Arduino/hardware/Moteino. Some users report that they can only make this work by copying it directly in the hardware folder under their Arduino installation folder.
4. Restart the IDE
5. Select Tools > Board > Moteino or MoteinoMEGA
6. To burn the bootloader, follow the Arduino [Bootloader](http://arduino.cc/en/Hacking/Bootloader) instructions.

## Requirements
* Tested on stable Arduino 1.6.9
* According to maniacbug the bootloader cannot be burned using [USBtinyISP](http://www.ladyada.net/make/usbtinyisp/). That programmer cannot flash to chips with >64k flash size. I recommend using a true AVR programmer like the AVR ISP MKii.

## MISC - See also
ManiacBug's older [mighty-1284p arduino core](http://maniacbug.wordpress.com/2011/11/27/arduino-on-atmega1284p-4/) and 
Leonardo Milliani's [mods to mighty-1284p](http://www.leonardomiliani.com/2014/core-per-atmega644p1284p-aggiornato-per-lide-1-5-6-r2/).
