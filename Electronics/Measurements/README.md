# VBUS measurements

## Thanks to Aypac

[LINK TO ORIGINAL](https://github.com/dirkvl/FairPhone/issues/2#issuecomment-179817946)

By Aypac:


Finally had time to do some measuring. All Bat-Voltages are taken by removing the bat from the phone.

Case a)
-No Charger connected
-Battery Voltage at 4.12V
-Phone turned on

    Charge is at 0V
    VBUS is at 3.90V

Case b)
-Charger (Laptop)
-Battery @ approx 4.1V
-Phone is "off"

    Charge pin @ 0V
    VBUS pin @ 3.99V

Case c)
-Charger (Laptop)
-Battery @ approx 4.1V
-Phone is "off"

    Charge pin @ 0V
    VBUS pin @ 3.94V

Case d)
-Bat fully charged (says Phone) @ 4.31V
-Almost no difference if FP is on/off and charger is dis-/connected

    VBUS @ 4.12V

My personal understanding of this is, that there is a Schottky diode (or something similar) between VBUS and Bat+ => You can not charge via VBUS, you won't get higher Voltages than ~4.15V.
Charge is always at 0V. With a conductivity test I get a reading of about 1.4V for the voltage drop between the Charge-pin and Bat+. This lets me believe, that there is some kind of regulator in between.

Surprisingly I got an almost perfect conductivity test between (GND)->(VBUS). This might be some kind of protection against wrong polarisation? But that would fry the PCB if enough power was connected, right? Nothing like that between (GND) and (Charge).

## Conclusions from measurements by dirkvl

To be added later.