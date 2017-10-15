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

I followed the given "Quick Start" assembly instructions. [The instructions on their wiki is more clear.](http://wiki.seeed.cc/Skeleton_Bot-4WD_hercules_mobile_robotic_platform/). Nonetheless, I took some pictures to document my step-by-step process.

1. Build the chasis
![alt text](https://github.com/johnny-wang/hercules_mobile_robot/tree/master/images/IMG_7869.JPG)
![alt text](https://github.com/johnny-wang/hercules_mobile_robot/tree/master/images/IMG_7870.JPG)

* Flip motor wires 
 i.e. If M1 is the left 2 tires and M2 are the right 2 tires, commanding them forward the robot spins in place.
      This means you need to swap the wires on the M1 connector.
