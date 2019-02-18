# Blink for Blue Pill using Platformio & ST-Link
## Why is this here
I created this repository to help quickly bootstrap a project using the Blue Pill with Platformio & ST-Link.  It's meant to be used by those not familiar with the Blue Pill, ST-Link, Platformio or the platformio.ini settings and those migrating from the Arduino IDE to Platformio.  Many times I get stuck on things like:
- “what are the minimum platform settings I need to get a successful compile?”
- “what’s the base code I can use to prove a valid compile and program execution?”
- “do I use the pin number or other ID for accessing GPIO?”

This project is meant to provide confirmation of these basic things.  That being said, to get better at working with new hardware, I would suggest you try and create a minimal “blinky” program yourself and refer to this only if you get stuck.  Platformio has progressed to a level that most folks can get a new program running in a matter of minutes.

## Prerequisites
- The Blue Pill & ST-Link V2 can be found on [eBay](https://www.ebay.com/sch/i.html?_nkw=STM32+st-link) for < $10
- [VSCode installed](https://code.visualstudio.com/download)
- [Platformio IDE for VSCode installed](https://platformio.org/platformio-ide)
- [STM32 Platform installed in Platformio IDE](https://platformio.org/platforms/ststm32)
- [ST-Link V2 driver for Windows installed](https://www.st.com/content/st_com/en/products/development-tools/software-development-tools/stm32-software-development-tools/stm32-utilities/stsw-link009.html)


## How to use this repository
Just Clone this repository, open in VSCode with the Platformio IDE previously installed, connect your ST-Link to your Blue Pill, plug in your ST-Link to your PC via USB and upload.  If you get errors, make sure you have the STM32 Platform installed in Platformio (STM32 4.6.0 used to compile and test on 2019-02-17)...see links above.  You can DM me if you get stuck [@PiercePrimm](https://twitter.com/PiercePrimm).

## References
- [Blue Pill Board for Platformio](https://docs.platformio.org/en/latest/boards/ststm32/bluepill_f103c8.html)
- [Blue Pill Board for STM32Duino](https://wiki.stm32duino.com/index.php?title=Blue_Pill) - This page has most of the information you need to work with the Blue Pill.  Note that, many times, the USB will not work because or the incorrect D+ resistor.  I have not changed any of my boards because I just use the ST-Link and therefore I don't have to update the bootloader to work with Arduino.