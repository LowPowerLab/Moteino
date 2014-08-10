# MoteinoMEGA Arduino core files for ATmega1284P based Moteinos

## What is it?
Everything you need to run a ATmega1284P based Moteino MEGA from the Arduino IDE.

## Status
This core was tested and modded from the original mighty-1284p core along with mods from Leonardo Milliani.
The platform now includes Dualoptiboot for atmega1284p which supports [wireless programming](http://lowpowerlab.com/blog/category/moteino/wireless-programming/) (R) by LowPowerLab.

## License
Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)
https://creativecommons.org/licenses/by-sa/4.0/

## Installation
1. Download the [ZIP File](https://github.com/LowPowerLab/Moteino/blob/master/MEGA/Core/MoteinoMEGA_Core.zip)
2. Unzip it a folder called 'hardware' off your sketches directory, e.g. /Users/felix/Arduino/hardware/MoteinoMEGA
3. Restart the IDE
4. Select Tools > Board > Moteino MEGA (1K DualOptiboot)
5. To burn the bootloader, follow the Arduino [Bootloader](http://arduino.cc/en/Hacking/Bootloader) instructions.

## Requirements

* Tested on stable Arduino 1.0.5
* According to maniacbug the bootloader cannot be burned using [USBtinyISP](http://www.ladyada.net/make/usbtinyisp/). That programmer cannot flash to chips with >64k flash size. I recommend using a true AVR programmer like the AVR ISP MKii.

## See also

Original creator of the mighty-1284p arduino core:
http://maniacbug.wordpress.com/2011/11/27/arduino-on-atmega1284p-4/

Leonardo Milliani's mods to mighty-1284p:
http://www.leonardomiliani.com/2014/core-per-atmega644p1284p-aggiornato-per-lide-1-5-6-r2/