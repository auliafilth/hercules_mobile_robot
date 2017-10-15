# Hercules 4WD Mobile Platform

The mobile platform of choice is the Hercules 4WD from Seeed. [I got mine from Amazon](
https://www.amazon.com/Skeleton-Bot-Hercules-Robotic-Platform/dp/B01N4AGPTN/ref=sr_1_2?ie=UTF8&qid=1508102110&sr=8-2&keywords=hercules+4wd)

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

## Build Instructions with Pictures

I followed the given "Quick Start" assembly instructions. [The instructions on their wiki is more clear](http://wiki.seeed.cc/Skeleton_Bot-4WD_hercules_mobile_robotic_platform/). Nonetheless, I took some pictures to document my step-by-step process.

0. Peel off the protective sheets for the acrylic pieces. It allows them to be partially see-through which is nice for looking into the robot later

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7869.JPG" height="25%" width="25%">

1. Build the chasis

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7869.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7872.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7874.JPG" height="25%" width="25%">

2. Add the 4 motors. The two with encoders should be across from each other. Also note that you put in two screws per motor and there is a divot in each shaft.

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7878.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7880.JPG" height="25%" width="25%">

3. Make sure the hole in the motor shaft adapter is aligned with the divot and put the screw in.

<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7883.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7882.JPG" height="25%" width="25%">
<img src="https://raw.githubusercontent.com/johnny-wang/hercules_mobile_robot/master/images/IMG_7884.JPG" height="25%" width="25%">

* Flip motor wires 
 i.e. If M1 is the left 2 tires and M2 are the right 2 tires, commanding them forward the robot spins in place.
      This means you need to swap the wires on the M1 connector.
