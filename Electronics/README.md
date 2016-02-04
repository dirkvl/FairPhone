# FairPhone

### Back connector

When you are looking from the back of the phone you see 5 pogo pins. With a multimeter and some trial&error you can find the following info:

```
(1) (2)
  (3)
(4) (5)

1) vbus
2) charge
3) gnd
4) d+
5) d-
```
#### VBUS
5V power out, always on. <LINK TO MEASUMENTS>
#### CHRG
Dedicated power input. Will love some 5V.
#### GND
Ground. (thank you captain obvious!)
#### D+/D-
Data lines for USB. Use some nice series resistors to limit current.

It has the following dimensions:

<img src="https://github.com/dirkvl/FairPhone/blob/master/Drawings/back-connector.JPG" width="300">

### Behind the back connector

<Assumptions>
- It has a separate step-up circuit to 5V
- There is a 5.5V zener diode behind both pin1 and pin2 connected to ground to protect for overvoltage.
- VBUS will not accept power in (since there is a dedicated charge pin)
- Charge pin will accept anything between 4.5V and 5.5V up to 1A
- There is no MPPT, making solar panels practically impossible.
</Assumptions>

<Confirmed>
- USB2.0
- 500ma
</Confirmed>

### Available space

When designing a hardware extension, there are some places to use and some places to definitely stay away.

All antennas should definitely be avoided as far as possible. If you cover an antenna, the reception of that antenna will be gone and the phone will push a lot of extra power to that antenna to try to get a connection anyway. This will result in a lot of power use, a lot of radiation and still no reception. Don't go there.

Some parts on the back of the phone show bare metal (sd card slot) or are slightly extruded (speaker and vibrator), these are to be avoided too. Covering the sd card slot with a PCB is a bad plan, it increases the risk of shorts if you have none-ground vias or tracks in that area. Some goes for the vibrator, it slightly extends from the surface, which will push the PCB away from the pogo pins, making for a bad connection. So, stay away.

The area above the battery however you can totally use.

![Available space](https://github.com/dirkvl/FairPhone/blob/master/Drawings/availablespace.png "Available space")

### Behind regular USB port
<insert info>

### Behind 3.5mm Jack
<insert info>