# Moteino/MoteinoMEGA Arduino core files for Atmega328P/ATmega1284P based Moteinos

## What is it?
Everything you need to run a ATmega1284P based Moteino MEGA from the Arduino IDE.
Added regular Moteino variant based on the prolific ATmega328p.

## Status
This Arduino core contains the ATmega1284P MoteinoMEGA variant and the ATmega328p Moteino variant (added Nov 2014) along with the DualOptiboot bootloaders.
The platform now includes Dualoptiboot for ATmega1284P and ATmega328p which support [wireless programming](http://lowpowerlab.com/blog/category/moteino/wireless-programming/) (C) by Felix Rusu of LowPowerLab.com

## License
This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details. View full license text at: http://www.gnu.org/licenses/gpl-3.0.txt

## Installation
0. Ensure you are running Arduino 1.6.0 or greater (this was tested on Arduino 1.6.1)
1. Download the whole repository ZIP, then extract the Moteino core [ZIP File](https://github.com/LowPowerLab/Moteino/blob/master/MEGA/Core/Moteino.zip) from that. 
2. From the Moteino.zip archive unzip and copy the Moteino folder in the Arduino 'Hardware' directory, e.g. /Arduino/hardware/Moteino
1. Download the [root of this repository](https://github.com/LowPowerLab/Moteino) (find the "Download ZIP" button), then find this [ZIP File](https://github.com/LowPowerLab/Moteino/blob/master/MEGA/Core/Moteino.zip) in that master ZIP archive. You will need to 
2. Unzip the content of the Moteino.zip into a folder called 'hardware' located in your sketches directory, e.g. /Users/felix/Arduino/hardware/Moteino. Some users report that they can only make this work by copying it directly in the hardware folder under their Arduino installation folder.
3. Restart the IDE
4. Select Tools > Board > Moteino or MoteinoMEGA
5. To burn the bootloader, follow the Arduino [Bootloader](http://arduino.cc/en/Hacking/Bootloader) instructions.

## Requirements
* Tested on stable Arduino 1.6.1
* According to maniacbug the bootloader cannot be burned using [USBtinyISP](http://www.ladyada.net/make/usbtinyisp/). That programmer cannot flash to chips with >64k flash size. I recommend using a true AVR programmer like the AVR ISP MKii.

## MISC - See also
ManiacBug's older [mighty-1284p arduino core](http://maniacbug.wordpress.com/2011/11/27/arduino-on-atmega1284p-4/) and 
Leonardo Milliani's [mods to mighty-1284p](http://www.leonardomiliani.com/2014/core-per-atmega644p1284p-aggiornato-per-lide-1-5-6-r2/).