# DS4-Type-C
Hate microUSB? Looking to decrease cable clutter? This is the PS4 mod for you. This repo aims to host mostly drop-in USB Type C replacement boards for all revisions of PS4 controller. The goal for each board is to follow the USB Type C standard, and to include pads for those who wish to impedance match the USB data lines. Either solder in resistors here to compensate, or simply use a solder/wire bridge. The overall project goal is to keep all possible parts the same between boards, and to make it reasonablly easy for a person of moderate skill to populate these boards as they are with no modifications necessary. This is an open source project though, so you're free to download [KiCad](https://www.kicad.org/download/) and start making modifications to these boards so that you can more easily populate them.

I used a 0.8mm PCB when I originally made these, and found it worked quite well. Gives a little more room to work inside the controller. Cost will likely depend on which board house you choose to go through.

## JDS-001
Work for this board was done [here](https://github.com/HDR/DualShock4-USB-C) by Martin Refseth. I reworked his board to create kicad and schematic files for it. I also added compensation resistors as discussed above.

## JDS-011
This board has not been started. Feel free to fork this project and make a PR if you own this board and wish to contribute. If all you can provide is schematics and dimensions, someone should be able to get a board made pretty quickly.

## JDS-030
As with JDS-011.

## JDS-040, JDS-050, and JDS-055
Work for this board is complete. I verified that 040 functions the same as stock. This board is special in that it features connectors and compensation resistors for JDS-040, JDS-050, JDS-055. The JDS-05X side is presently untested, but according to reddit user [u/Mcorgano](https://www.reddit.com/r/PS4Mods/comments/p2q3da/selling_dropin_replacement_type_c_charge_boards/h8oozja/) the pinout is supposedly the same between JDS-040 and JDS-055. The [idea](https://www.reddit.com/r/PS4Mods/comments/p2q3da/selling_dropin_replacement_type_c_charge_boards/h8os8rh/) for this dual board also comes from the same user.

## Universal
The idea here is to create one "panelized" board which contains all above boards (JDS 001, 011, 030, 040, 050, 055). This means that someone could easily acquire a board for all controllers, then populate the one they need.


# Parts
The goal with parts is to stay as consistent as possible between boards. Unfortunately, we have to use two types of RGB LED between the older and newer boards, but the goal is for this to be the only difference. Resistors are standardized to 0603 using the kicad hand_solder pads. We use USB type C connector C-31-M-12 to make soldering easy. Additionally, we use the Molex 530480 line of FPC connectors on all boards.  

Footprints or symbols which do not come with kicad by default are to be declared as project libraries, and included in the board directory as .pretty files. See 040 055 for as a reference.  

- New RGB LED:          [MSL0601RGBU1](https://www.mouser.com/ProductDetail/ROHM-Semiconductor/MSL0601RGBU1?qs=F5EMLAvA7IAg0rK0mfHa6w%3D%3D)
- Old RGB LED:          [MSL0104RGB](https://www.mouser.com/ProductDetail/ROHM-Semiconductor/MSL0104RGBU1?qs=%2Fha2pyFaduhThMWGX8bFHltJ8rIVfHrbMpgQU1T0g7RvDKWc6HIiGQ%3D%3D)
- USB Type C:           [Type-C-31-M-12]()
- FPC Connector - 12:   [503480-1200](https://www.mouser.com/ProductDetail/Molex/503480-1200?qs=%2Fha2pyFaduiit5JSGz5lsv1U%252BbZL3U56cNxg7eoCvCy3Ie8rHq3SFA%3D%3D)
- FPC Connector - 14:   [503480-1400](https://www.mouser.com/ProductDetail/Molex/503480-1400?qs=%2Fha2pyFadujj30aImGpM0ckpak%252BVtmx2aY5U9nBD5Hh2NWtQuUTDBg%3D%3D)
- Resistors:            [0603](https://www.mouser.com/Passive-Components/Resistors/Film-Resistors/Thin-Film-Resistors-SMD/_/N-7gz44?Keyword=0603&FS=True)