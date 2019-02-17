# Blink for Blue Pill using Platformio & ST-Link

The Blue Pill & ST-Link V2 can be found on [eBay](https://www.ebay.com/sch/i.html?_nkw=STM32+st-link) for < $10

Just Clone this repository, open in VSCode with the Plafoirmio IDE prefiously installed, connect your ST-Link to your Blue Pill, plug in your ST-Link to your PC via USB and upload.  If you get errors, make sure you have the STM32 Platform installed in Platformio (STM32 4.6.0 used to compile and test on 2019-02-17)...see references below.  You can DM me if you get stuck [@PiercePrimm](https://twitter.com/PiercePrimm).

## References
- [Platformio](https://platformio.org)
- [STM32 Patform for Platformio](https://platformio.org/platforms/ststm32)
- [BluePill Board for Platformio](https://docs.platformio.org/en/latest/boards/ststm32/bluepill_f103c8.html)
- [STM32Duino]()
- [Blue Pill Board for STM32Duino](https://wiki.stm32duino.com/index.php?title=Blue_Pill) - This page has most of the information you need to work with the Blue Pill.  Note that, many times, the USB will not work because or the incorrect D+ resistor.  I have not changed any of my boards because I just use the ST-Link and therefore I don't have to update the bootloader to work with Arduino.
- [ST-Link V2 Driver for Windows](https://www.st.com/content/st_com/en/products/development-tools/software-development-tools/stm32-software-development-tools/stm32-utilities/stsw-link009.html)