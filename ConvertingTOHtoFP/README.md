# JollaTOH to Fairphone casings

## Que?

The Jolla phone -LINK- introduced the OtherHalf concept. Casings with extending functionality can be added on the back of the phone and have the possibilty to connect directly to the phone over I2C. Additionally there is a power in and out.

Fairphone has a similar concept (how very original!) but instead uses USB. This opens up some doors, but makes some other doors a little harder to open.

## I2C on Jolla TOH

-LINK to JollaTOH page-

I2C -LINK- is a protocol developed in Holland (Whoop Whoop!) by Philips and is intended for embedded electronics (chips on the same PCB) to speak with each other. 

## USB on Fairphone

USB is a protocol intended for the use of peripherals, like a mouse/keyboard/touchpad/memorystick. The data tranfer speed is a lot higher and a lot of application will be plug&play (otherwise you are not allowed to call it USB), but the circuits can be a bit more complex and expensive.

## Bridging

If one has developed a JollaTOH and wants to convert this to a Fairphone casing, the most straightforward way to do this is using an FTDI bridge <LINK>. 

FTDI makes a lot of very fancy microcontrollers, of which we will need a USB-I2C bridge. This is a ic that has the USB protocol built in and has an I2C line out to connect the rest of the electronics. 

## Commands

-moar info later-