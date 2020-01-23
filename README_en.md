# Chidori build guide

Please refer to [here](https://github.com/ka2hiro/chidori_expansion_build_guide/blob/master/README_en.md) for the Chidori expansion kit build guide.





## Before build

* Please be aware of injuries with soldering irons, tools, parts etc.
* When you leave your seat during work, please confirm that the soldering iron is turned off.
* Very small parts are included, so be careful not to lose.




## Confirm contents
The following parts are included in the kit. Please check whether there is any shortage before work.

![kit contents](images/IMG_4410.jpg)

Number | Image | Name   | Value | Qty | Remarks         | Place(Master) | Place(Slave) 
:----|:------|:--------|:-----|:----|:-----------------|:-------|:-------
1 |![PCB](images/IMG_4411.jpg)| PCB      |       | 2    | 1 for master, 1 for slave. | |
2 |![Top  Plate](images/IMG_4414.jpg)| Top plate |  | 2 |           | | 
3 |![Bottom Plate](images/IMG_4412.jpg)| Bottom plate |     | 2 |        | | 
4 |![Acryl Plate](images/IMG_4415.jpg)| Acrylic  plate |  | 2 |        | | 
5 |![MPU](images/IMG_4425.jpg)| MPU | ATMEGA3280-PU | 1 |    | U1 | 
6 |![I2C IO Expander](images/IMG_4424.jpg)| I2C IO Expander | MCP23017 | 1 |  |  | U1 
7 |![IC Socket](images/IMG_4426.jpg)| IC Sockets |  | 2 |   | | 
8 |![Crystal](images/IMG_4428.jpg)| Crystal oscillator | 16 MHz | 1 |    | Y1 | 
9 |![Polyswitch](images/IMG_4429.jpg)| Resettable fuse | RXEF005 | 1 |    | F1 | 
10 |![Tact Swtich (W)](images/IMG_4431.jpg)| Tactile switch(wh) | TVBP06-B043CW-B | 1 |   | RESET | 
11 |![Tact Switch (B)](images/IMG_4433.jpg)| Tactile switch(bl) | TVBP06-B043CB-B | 1 |   | BOOT | 
12 |![TRRS Jack](images/IMG_4435.jpg)| TRRS Jack | MJ-4PP-9 | 4 | | J2, J3 | J1, J2 
13 |![DIP Switch](images/IMG_4438.jpg)| DIP Switch | KSD42 | 1 | | | SW28 
14 |![USB Connector](images/IMG_4440.jpg)| USB Connector | 54819-0519 | 1 |    | J1 | 
15 |![LED Green](images/IMG_4442.jpg)| LED(gr) | OSG8HA3Z74A | 2 |   | LED1 | LED1 
16 |![LED Yellow](images/IMG_4444.jpg)| LED(yl) | OSY5JA3Z74A | 2 |   | LED1 | LED1 
17 |![ZenerDiode](images/IMG_4446.jpg)| Zener diode | GDZJ3.6B | 2 | Be careful as it is difficult to distinguish from 1N4148. | D25, D26 | 
18 |![Capacitor10u](images/IMG_4449.jpg)| Electrolytic capacitor | 10μF | 1 |   | C1 | 
19 |![Capacitor1u](images/IMG_4463.jpg)| Capacitor | 1μF | 3 | Marked "105" on the package. | C2 | C1, C2 
20 |![Capacitor0.1u](images/IMG_4460.jpg)| Capacitor | 0.1μF | 2 | Marked  "104" on the package. | C3 | C3 
21 |![Capacitor22p](images/IMG_4458.jpg)| Capacitor | 22pF | 2 | Marked "22" on the package. | C4, C5 | 
22 |![Resistor10k](images/IMG_4465.jpg)| Resistor | 10kΩ | 5 | The color code is brown,  black,  orange,  gold. | R1 | R3, R4, R5, R6 
23 |![Resistor5.1k](images/IMG_4467.jpg)| Resistor | 5.1kΩ | 4 | The color code is green, brown, red, gold. | R7, R8 | R1, R2 
24 |![Resistor2.2k](images/IMG_4469.jpg)| Resistor | 2.2kΩ | 2 | The color code is red, red, red, gold. | R5, R6 | 
25 |![Resistor1.5k](images/IMG_4470.jpg)| Resistor | 1.5kΩ | 1 | The color code is brown, green, red, gold. | R2 | 
26 |![Resistor68](images/IMG_4473.jpg)| Resistor | 68Ω | 2 | The color code is blue, gray, black, gold. | R3, R4 | 
27 |![Diode](images/IMG_4477.jpg)| Diode | 1N4148 | 48 |Be careful as they are difficult to distinguish from Zener diodes. | D1 - D24 | D1 - D24 
28 |![M2 Standoff 10mm](images/IMG_4478.jpg)| M2 standoff | 10mm | 4 |                   | | 
29 |![M2 Standoff 7mm](images/IMG_4480.jpg)| M2 standoff | 7mm | 8 |                   | | 
30 |![M2 Screw](images/IMG_4483.jpg)| M2 screw | 4mm | 24 |                   | | 
31 |![RubberFeet](images/IMG_4485.jpg)| Rubber feet |      | 8 |                | | 
32 |![TRRS Cable](images/IMG_4486.jpg)| TRRS cable |       | 1 |     | | 
33 |![USB MiniB Cable](images/IMG_4490.jpg)| USB MiniB cable |       | 1 |     | | 




## Other required items
* In order to complete the kit, the following parts must be prepared separately.

  * Key switch (Cherry MX compatible only support)
  * Key caps




## Required tools
In order to build, the following tools are required at minimum.

* Soldering iron (preferred temperature controllable)
* Lead solder
* Tweezers
* Phillips head screwdriver
* Magnifier
* Flux
* Multimeter

In addition, you may also prepare the following as necessary.

* Flux remover
* Solder wick



## Precautions when assembling

* The parts used for the master and the slave are different. Note that each step in the procedure may be labeled "master only" or "slave only."
* In the following procedure, it is assumed that both the master and the slave are assembled at the same time, but it is of course possible to assemble them separately. Assemble the way you like. If you are assembling separately, skip the steps that are not required for each step.
* Some components require attention in the mounting direction. If this is indicated in the procedure, check the orientation of the parts carefully before working.




## Solder resistors
1. Solder the resistors R1 to R8 on the master side.

![Resistor master](images/IMG_4235.jpg "Master side")

2. Solder the resistors R1 to R6 on the slave side.

![Resistor slave](images/IMG_4240.jpg "Slave side")



## Solder Zener diode (Master only)

**Note that the diode has a direction. **

1. Solder the Zener diodes D25 and D26 on the master side.

![Zener diode](images/IMG_4247.jpg)



## Solder the crystal oscillator (Master only)

1. Solder the crystal oscillator Y1 on the master side.

![Crystal](images/IMG_4254.jpg)



## Solder the capacitor

1. Solder the capacitors C2 to C5 on the master side.

![Capacitor master](images/IMG_4258.jpg)

2. Solder the capacitors C1 to C3 on the slave side.

![Capacitor slave](images/IMG_4260.jpg)



## Solder electrolytic capacitor (Master only)

**Note that electrolytic capacitors have a direction. **

1. Solder the electrolytic capacitor C1 on the master side. Attach it so that the longer lead is facing (+).

![Capacitor master](images/IMG_4269.jpg)



## Solder resettable fuse (Master only)

1. Solder the resettable fuse F1 on the master side.


![Resettable fuse](images/IMG_4276.jpg)



## Solder diode

**Note that the diode has a direction. **

1. Since the diode is mounted vertically, bend the cathode (the side with the black bar) lead in advance as shown in the following image.

![Bend lead](images/IMG_4277.jpg)

2. When mounting the diode on the PCB, insert it so that the body is on the round land.

![place diode](images/IMG_4283.jpg)

3. Solder the diodes D1 to D24 on the master side.
4. Solder the slave diodes D1 to D24.

![solder diode](images/IMG_4287.jpg)




## Solder LED
**Note that LED has a direction.**

1. Solder LED1 (green) and LED2 (yellow) on the master side. Make sure that the longer lead faces the round pad.

![led master](images/IMG_4296.jpg)

2. Solder LED1 (green) and LED2 (yellow) on the slave side. Make sure that the longer lead faces the round pad.

![led slave](images/IMG_4300.jpg)




## Solder the tactile switch (Master only)
1. Solder the tactile switches (black) and (white) on the master side.

![tact switch](images/IMG_4304.jpg)




## Solder the DIP switch (Slave only)
1. Solder the DIP switch on the slave side.

![dip switch](images/IMG_4307.jpg)

2. Set the DIP switches as follows, setting 1 to Off (down) and 2 to 4 to On (up).

![dip switch2](images/IMG_4570.jpg)




## Solder the USB connector (Master only)
1. Solder the USB connector on the master side.

![usb connector](images/IMG_4312.jpg)




## Solder the TRRS jack
1. Solder the TRRS jack on the master side.

![trrs jack](images/IMG_4314.jpg)

2. Solder the slave side in the same way.

![trrs jack](images/IMG_4320.jpg)

  


## Solder IC socket
**Note that the IC socket has a direction.**

1. Solder the IC socket on the master side. Attach the notch of the IC socket to the right side.

![ic socket master](images/IMG_4324.jpg)

2. Solder the slave side in the same way.

![ic socket slave](images/IMG_4329.jpg)



## Insert ATMEGA328P and MCP23017
**Note that the IC has a direction.**

1. Insert ATMEGA328P into the IC socket on the master side and MCP23017 into the IC socket on the slave side.
2. Since the IC pins are wider than the IC socket, bend them slightly inward before inserting.
3. Align the notch on the IC with the IC socket so that the direction of the IC is correct.

![mark](images/IMG_4500.jpg)




## Check whether the soldering is properly done
Refer to the schematic ([master side](files/chidori_master.pdf), [slave side](files/chidori_slave.pdf)) and check whether soldering is correctly done.

Before connecting to the computer, at least check the followings.

1. Check that there is no short circuit between UVCC - GND and VCC - GND.
2. Make sure the MPU pins are not bridged.
3. Make sure the USB connector pins are not bridged.




## Verify that it is recognized as a USB device
When you connect the keyboard to the computer, check that the **green LED lights up**.

Next, perform the following operations to enter the boot loader mode and confirm that the device is recognized as a USB device.

1. Hold down the BOOT switch (black)
2. Press and release the RESET switch (white)
3. Release the BOOT switch (black)

When you enter bootloader mode, the **yellow LED will flash**. If it doesn't, try repeating the above steps slowly.

* For Mac, start "System Information" and check whether the device named "USBasp" is visible.

![system info](images/system-info.png)

* For Windows, the libusbK driver must be installed. Download the installation tool from the following site and set it up.
	* [Zadig - Installing tool](https://zadig.akeo.ie/)
	* [Setup](https://electronics.stackexchange.com/questions/416714/avrdude-does-not-recognize-usbasp-device/417509#417509)
* Start "Device Manager", check whether the device named "USBasp" is visible.

![device manager](images/device-manager.png)

If it is not recognized as a USB device or does not enter the boot loader mode, please double check the schematic to see if all parts are properly soldered.




## Attach the key switches to the top plate
1. Attach the key switches to the top plate.

![switch insert to plate](images/IMG_4337.jpg)

2. Combine the PCB and the top plate. 
3. Press the key switches firmly into the PCB and check that the bottom of the key switches are in contact with the PCB.
4. Solder the key switches.

![combine top plate and pcb](images/IMG_4354.jpg)




## Attache the stand off for acrylic plate
1. Attache the stand off M2x10mm for the acrylic plate to the screw hole near the TRRS jack. 

![standoff for acryl plate](images/IMG_4362.jpg)




## Attache the bottom plate
1. Insert the M2x4mm screw into the bottom plate and attach the stand off.

![bottom plate](images/IMG_4369.jpg)

2. Combine the top plate and PCB on the bottom plate and screw them with M2x4mm.

![combine  all](images/IMG_4373.jpg)




## Attach the rubber feet
1. Attach the rubber feet to the bottom plate.

![rubber feet](images/IMG_4495.jpg)




## Attach the keycaps
1. Attach your favorite keycaps.



## Write firmware
The firmware uses QMK. Since it has not been merged into QMK itself, clone the following repository, check out the "chidori_support" branch, and build.

[qmk_firmware](https://github.com/ka2hiro/qmk_firmware)

After checking out, go to the directory of your local repository.

Then connect the keyboard to the computer and enter boot loader mode.

Execute the following command to start writing the firmware. If writing fails, try running the command again.

~~~
$ make chidori:default:usbasp
~~~

When writing is completed, press the RESET switch (white) to exit the boot loader mode.

Refer to [this document](https://docs.qmk.fm/#/getting_started_build_tools) for how to build the environment for building firmware.




## Completed!
Attach the acrylic cover and you're done. Congrarulation!
![Done](images/IMG_4491.jpg)



