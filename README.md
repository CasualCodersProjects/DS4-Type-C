# DS4-Type-C
Hate microUSB? Looking to decrease cable clutter? This is the PS4 mod for you. This repo aims to host replacement boards for all models of PS4 controller using USB type C.

## JDS-001
Work for this board was done [here](https://github.com/HDR/DualShock4-USB-C) by Martain Refseth. 12ian3 reworked his board, and created kicad and schematic files for it.

## JDS-011
Work on this bard will begin shortly. The plan is for 12brendan3 to get the pinout and make schematics and a board which features type C.

## JDS-030
Work for this board will begin shortly. The plan is for 12brendan3 to get the pinout and make schematics and a board which features type C.

## JDS-040 and JDS-055
Work for this board is complete. 12ian3 verified that 040 functions as intended. This board is special in that it features connectors and resistors for both JDS-040 and JDS-055. JDS-055 side is presently untested, as no contributors currently own a DS4 controller which uses JDS-055. The pinout is supposedly the same between JDS-040 and JDS-055, but this is untested, and comes from reddit user [u/Mcorgano](https://www.reddit.com/r/PS4Mods/comments/p2q3da/selling_dropin_replacement_type_c_charge_boards/h8oozja/) on reddit. The [idea](https://www.reddit.com/r/PS4Mods/comments/p2q3da/selling_dropin_replacement_type_c_charge_boards/h8os8rh/) for this dual board comes from the same user.


# Parts
The goal with parts is to stay as consistent as possible between boards. Unfortunately, we have to use two types of RGB LED between the older and newer boards, but the goal is for this to be the only difference. Resistors are standardized to 0603 using the kicad hand_solder pads. We use USB type C connector C-31-M-12 to make soldering easy. Additionally, we use the Molex 530480 line of FPC connectors on all boards.  

Schematics which do not come with kicad by default are declared as project libraries, and included in the root project directory as .pretty files. See 040 055 for as a reference.  

- New RGB LED:          [MSL0601RGBU1](https://www.mouser.com/ProductDetail/ROHM-Semiconductor/MSL0601RGBU1?qs=F5EMLAvA7IAg0rK0mfHa6w%3D%3D)
- Old RGB LED:          [MSL0104RGB](https://www.mouser.com/ProductDetail/ROHM-Semiconductor/MSL0104RGBU1?qs=%2Fha2pyFaduhThMWGX8bFHltJ8rIVfHrbMpgQU1T0g7RvDKWc6HIiGQ%3D%3D)
- USB Type C:           [Type-C-31-M-12]()
- FPC Connector - 12:   [503480-1200](https://www.mouser.com/ProductDetail/Molex/503480-1200?qs=%2Fha2pyFaduiit5JSGz5lsv1U%252BbZL3U56cNxg7eoCvCy3Ie8rHq3SFA%3D%3D)
- FPC Connector - 14:   [503480-1400](https://www.mouser.com/ProductDetail/Molex/503480-1400?qs=%2Fha2pyFadujj30aImGpM0ckpak%252BVtmx2aY5U9nBD5Hh2NWtQuUTDBg%3D%3D)
- Resistors:            [0603](https://www.mouser.com/Passive-Components/Resistors/Film-Resistors/Thin-Film-Resistors-SMD/_/N-7gz44?Keyword=0603&FS=True)