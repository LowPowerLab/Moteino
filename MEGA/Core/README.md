# Moteino/MoteinoMEGA Arduino core files for Atmega328P/ATmega1284P based Moteinos

## What is it?
Everything you need to run a ATmega1284P based Moteino MEGA from the Arduino IDE.
Added regular Moteino variant based on the prolific ATmega328p.

## Status
This Arduino core contains the ATmega1284P MoteinoMEGA variant and the ATmega328p Moteino variant (added Nov 2014) along with the DualOptiboot bootloaders.
The platform now includes Dualoptiboot for ATmega1284P and ATmega328p which support [wireless programming](http://lowpowerlab.com/blog/category/moteino/wireless-programming/) (R) by Felix Rusu of LowPowerLab.com

## License
This program is free software; you can redistribute it 
and/or modify it under the terms of the GNU General    
Public License as published by the Free Software       
Foundation; either version 3 of the License, or        
(at your option) any later version.
This program is distributed in the hope that it will   
be useful, but WITHOUT ANY WARRANTY; without even the  
implied warranty of MERCHANTABILITY or FITNESS FOR A   
PARTICULAR PURPOSE. See the GNU General Public        
License for more details. View full license text at: http://www.gnu.org/licenses/gpl-3.0.txt

## Installation
1. Download the [ZIP File](https://github.com/LowPowerLab/Moteino/blob/master/MEGA/Core/Moteino.zip)
2. Unzip it a folder called 'hardware' off your sketches directory, e.g. /Users/felix/Arduino/hardware/Moteino
3. Restart the IDE
4. Select Tools > Board > Moteino or MoteinoMEGA
5. To burn the bootloader, follow the Arduino [Bootloader](http://arduino.cc/en/Hacking/Bootloader) instructions.

## Requirements
* Tested on stable Arduino 1.0.6
* According to maniacbug the bootloader cannot be burned using [USBtinyISP](http://www.ladyada.net/make/usbtinyisp/). That programmer cannot flash to chips with >64k flash size. I recommend using a true AVR programmer like the AVR ISP MKii.

## See also
Original creator of the mighty-1284p arduino core:
http://maniacbug.wordpress.com/2011/11/27/arduino-on-atmega1284p-4/
Leonardo Milliani's mods to mighty-1284p:
http://www.leonardomiliani.com/2014/core-per-atmega644p1284p-aggiornato-per-lide-1-5-6-r2/