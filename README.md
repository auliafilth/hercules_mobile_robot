# Hercules 4WD Mobile Platform

The mobile platform of choice is the Hercules 4WD from Seeed. [I got mine from Amazon](
https://www.amazon.com/Skeleton-Bot-Hercules-Robotic-Platform/dp/B01N4AGPTN/ref=sr_1_2?ie=UTF8&qid=1508102110&sr=8-2&keywords=hercules+4wd)

## Table of Contents

[Build Instructions with Pictures](https://github.com/johnny-wang/hercules_mobile_robot#build-instructions-with-pictures)

[Code Instructions](https://github.com/johnny-wang/hercules_mobile_robot#code-instructions)

## Build Instructions with Pictures

I followed the given "Quick Start" assembly instructions. [The instructions on their wiki is more clear](http://wiki.seeed.cc/Skeleton_Bot-4WD_hercules_mobile_robotic_platform/). Nonetheless, I took some pictures to document my step-by-step process.

**0. Peel off the protective sheets for the acrylic pieces. It allows them to be partially see-through which is nice for looking into the robot later**

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7873.JPG" height="25%" width="25%">

**1. Build the chasis**

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7869.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7872.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7874.JPG" height="25%" width="25%">

**2. Add the 4 motors. The two with encoders should be across from each other. Also note that you put in two screws per motor and there is a divot in each shaft**

Note: Here I installed the encoder motors at different end than specified in the instructions. This is due to the location of the switch that is to be installed later. I opt-ed for the hole of the switch to be at the bottom than the top. See step 6 for more details.

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7878.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7880.JPG" height="25%" width="25%">

**3. Make sure the hole in the motor shaft adapter is aligned with the divot and put the screw in**

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7883.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7882.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7884.JPG" height="25%" width="25%">

**4. Add the wheels**

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7886.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7890.JPG" height="25%" width="25%">

**5. Install the motor controller**

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7891.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7893.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7894.JPG" height="25%" width="25%">

**6. Install the battery and switch**

NOTE: I originally installed the small acrylic piece to hold the battery in place. This is also why I installed the switch at the bottom because the acrylic blocked the top hole. However, I ended up removing the acrylic to give the battery, switch, and wires more wiggle space.

This part requires a small bit of soldering to attach the leads to the switch.
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7903.JPG" height="25%" width="25%">

I decided to solder the leads to these two contacts for two reasons:
(a). The switch is 'on' when toggled away from the wheel so there is more clearance in case the wheel picks up and debris.
(b). There is more space and less precision is needed to hit the switch and kill power if needed. (Of course a large e-stop button is better. That will be future work.)
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7902.JPG" height="25%" width="25%">

**7. Plug in the wires**

Plug in the motor wires as shown in the diagram. The "left" wheels go to M1 and the "right" wheels go to M2. However, you will need to flip the contacts for either M1 or M2 wires because the "forward" command to the motor controller will spin the vehicle in place with the current setup. 

DO NOT cut the wires, you can pop out the contact with a small screw driver. Push down and pull the wire out.
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7907.JPG" height="25%" width="25%">

For me, the red wires went to M2B and M1A banks.
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7908.JPG" height="25%" width="25%">

**8. Plug in the UartSBee module**

This guy will allow you to send commands and read encoders to/from the motor controller board.
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7909.JPG" height="25%" width="25%">

## Code Instructions

The sample code from their website does not work.
* Use the github code: https://github.com/Seeed-Studio/Hercules_Motor_Driver
* Remove the "-master" from the directory name.
* Save directory to library folder of Arduino (in Documents of Mac)
* Note: "motorDriverDemo" code does not work
* "DC_motor" example works out of the box 
* Arduino IDE use "Atmega328" or "Pro / Mini"
* enocder_demo from https://github.com/blueeyedcharlie/Hercules_Motor_Driver/
  Revolution-counter (tachometer)
  Make sure to get latest Arduion IDE 

