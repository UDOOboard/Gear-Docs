If you find any problem in the proper working of UDOO BOLT GEAR, please consult this section.

## My UDOO BOLT GEAR doesn't boot or restart itself continuously

If your UDOO BOLT GEAR does NOT boot or restarts all the time, please check the following points:

- When the power jack is inserted the board does not start automatically. The power status LED is *yellow/amber/orange* and the board is in the power off state. To turn on UDOO BOLT GEAR you have to press the small **power button** on the front of the board. The status LED turns green when the board is powered on. Check the power button position in the [Hardware Reference - Overview](!/Hardware_References/Overview) page.

- Check the **power source** you are applying to UDOO BOLT GEAR. Please, follow the [Power Sources](!/Hardware_References/Power_Sources) page or consult the [User Manual](https://udoo.org/download/files/Doc/UDOO_BOLT_MANUAL.pdf) to learn more about the power supply needed by the board for normal operation.

- Check that the restore factory configuration **switch** is in the right position for normal operation, otherwise the board will restart continuously. You can find info about that switch in the [BIOS-UEFI Firmware](!/BIOS-UEFI_and_Tools/BIOS-UEFI_Firmware) page or consulting the [User Manual](https://udoo.org/download/files//Doc/UDOO_BOLT_MANUAL.pdf).

- Try detaching all peripherals connected to UDOO BOLT GEAR except RAM and video cable. You should be able to see the UDOO LOGO and the first page of the BIOS.

- If you are using 2 RAM modules, try using only one RAM module at a time in the socket closest to the heatsink. If the card does not boot with either RAM modules, try using one RAM module at a time in the other socket, the one farthest from the heatsink. This is useful to rule out a problem with one of the RAM modules or one of the RAM sockets.

## I see an orange LED (D13) blinking

The D13 orange LED you see is the standard Arduino LED 13. The Arduino&reg; microcontroller (ATmega32U4) onboardM comes with an Arduino sketch (firmware) preinstalled that just blink the LED every 1 second. This is the standard Arduino first example and it is used in the board testing phase to check if the microcontroller side and communication works properly.

## The Fan on top of the heatsink has a strange behaviour

Please check the warnings in [Fan Settings](!/BIOS-UEFI_and_Tools/Fan_Settings) page to know how to configure the BIOS settings for your fan. An incorrect configuration can also cause the UDOO BOLT GEAR to shut down because it cannot dissipate heat properly.

## I can't upload sketches to Arduino Leonardo onboard

If you have any trouble uploading **Arduino sketches** running **Linux**, check the *Linux - known issues* section in the [Getting Started with Arduino Leonardo](!/Arduino_Leonardo-compatible(ATmega32U4)/Getting_Started_with_Arduino_Leonardo#page_Known-issues) page.  
Here you can find a procedure for trying to [restore the correct uploading state of sketches](!/Arduino_Leonardo-compatible(ATmega32U4)/Getting_Started_with_Arduino_Leonardo#page_How-to-restore-the-correct-uploading-state-of-sketches).
