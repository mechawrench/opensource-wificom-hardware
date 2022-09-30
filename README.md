# Open Source WiFiCom Hardware - Build your own!

![WiFiCom, Assembled](/images/wificom_1.jpg)

This repository provides the needed files to make a THT(Through Hole Technology) PCB for the WiFiCom Hardware.  THT was chosen to make this more accessible, SMT (Surface Mount Technology) is quite the step up.  Also included are basic 3d models for the enclosure.  You are free to use these files for any purpose but attribution is required.

## Credits
This project was made possible by the incredible work of BladeSabre.  I request that you provide credits to both BladeSabre and myself if you use this project.  Do note "BrassBolt" is on the PCB silkscreen bottom (users should never see this unless removing hot glue from the PCB).

## TODO
- [ ] Add STL files for enclosure
- [ ] Add editable files for enclosure
- [ ] Add editable files for PCBs

## Supported Toys
- Digimon Pronged (2 Prong/3 Prong)
- Digimon IR
- Digimon Barcodes (D-Scanner)
- Legendz (Talispod/Talisdam)

## Parts List

### General
- Hot Glue Gun
- Hot Glue Sticks
- 3d Printer (or have someone print the enclosure for you)
- Double sided tape (industrial strength)
- Soldering equipment
    - Solder
    - Flux
    - Soldering Iron

### Components
**NOTE** A link will be added soon to quickly add all parts to your cart
- Arduino Nano RP2040 Connect (With Headers)
- Resistors 1/4 watt
    - 1.2K (1%)
    - 3.3K (1%)
    - 220 ohm (1%)
    - 4.7K
    - 100K
    - 470K
    - 1K
- 2x 1nf capacitor
- IR Receiver 58000
- IR Receiver 4838
- IR 950nm LED
- 2x 15 pin socket header
- 1x 2 pin socket header (for Legendz use)
- 1x Button (of appropriate size)
    - **Note**:  This button is smaller than normal buttons, compare sizes.  I will provide a parts list here soon with links to the parts I used.
    - **Note**:  If your button only has two pins, use the two pins on the far right.  The two on the left are not actually connected to anything.
- Two wires to connect board base to interface

## Build Instructions
### PCB
1. Find the GERBER file for the PCBs in the `PCB` folder.
2. Upload the files (board base and pronged interface) to your favorite PCB manufacturer.
3. Order the PCB.

### Case
1. Find the STEP file for the case in the `Case` folder.
2. Ensure you load the STL file into your slicer with proper placement, by default you may see bad alignment when importing the STL file.
3. Slice the STL file for your 3d printer.
4. Print the case.

### Assembly
1. Solder the components to the PCB.
2. Get the board base ready, place hot glue in the corners and set the assembled board inside.  Hold down for approximately 30 seconds.
3. Slide the pronged interface wires through both the case lid and the interface base to prepare for soldering the interface on.
4. Solder the interface to the board.  Be sure to place SIG/GND properly.
5. Use (strong) double sided tape to affix the interface board to the interface base.  Again, use double sided tape to affix the interface board to the case lid.  You should now have a solid interface and top section of the case.
6. Once your electronic board is glued to the base, you can now glue the top section on.  Ensure you leave room on both sides (see picture), you want to be able to access the button as-well as the LEDs on the side of the USB-MICRO port.

### Important Notes
- All components are required, do not skip any.
- The button is smaller than normal buttons, compare sizes.  I will provide a parts list here soon with links to the parts I used.
- Triple check that SIG/GND are hooked up properly.
- Program the Arduino Nano RP2040 Connect BEFORE gluing together the unit.
