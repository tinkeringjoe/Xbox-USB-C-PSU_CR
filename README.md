This fork is for the following:

1) Reducing cost by using a cheap single IC that requires barely any supporting passives for USB-PD negotiating.
2) Updating power good signal to be an AND of the 4 power rails rather than a wired OR for power good.
3) Move components from back to front to simplify manufacturing.
4) Change from solder pads to through holes for power cabling; add enough holes for all XBOX revisions cabling.

Goals 1-4 completed. Additionally changed the following.
Inductor/output capacitors for all power rails have been updated per datasheet equations to minimize ripple.
Cost reduced components (BOM will remain hidden until testing is completed.)


This board supports the following power on the rails with an expected ripple of around 1%
5V - 15A
12V - 1.5A
3.3V - 5A
3.3VSB - 700mA

5 turn-key boards have been ordered to test. The following testing is to occur before even touching an XBOX.


1.) Power supply ripple is to be measured under the following conditions (1%, 25%, 50%, 100% of peak load). Should not exeed 5%.
2.) Load removal testing; 100% to 0% load. Should not exceed 10% of voltage rail.

Once these requirements have been satisfied real-hardware testing can occur.

# Xbox-USB-C-PSU
The first ever USB C PSU for the original Xbox

# NOTE:
This board currently supports all 3 Xbox motherboard revisions, but requires a different BOM for 009 and 012 than 121.
If you don't know what revision your Xbox is, you can find out with this guide: [https://www.herringhardware.com/xboxrevisions](https://www.herringhardware.com/XboxRevisions.html)

# REPO STRUCTURE:
All source files for the PCB are contained within the respective folder for each of the 3 official Xbox PCB revions,
-121 to start with, and -009 and -012 will be added soon.
Production files to manufacture the PCBs are located in [Releases](https://github.com/Redherring32/Xbox-USB-C-PSU/releases)

# PCB SPECS:
* 4 layers
* 151.739x39.78mm
* 1oz copper (all layers), heat issues may result from skimping on this
* filled vias (VIPPO) for assembly reasons due to via in pad

![kicad_rvZLV58yR5](https://github.com/user-attachments/assets/5e256504-aa61-479c-9c4e-d7f61f2c38fe)


## LICENSE:
Licensed under
the TAPR Open hardware license (www.tapr.org/OHL)

©Redherring32 2025

## DISCLAIMER:
I offer this with no warranty, express or implied, and I am NOT responsible for anything that may happen as a result of misuse of this PCB.
You have been warned.
