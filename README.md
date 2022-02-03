# V0.1 Nema17 A/B Drive
**Not Compatible with the tophat**
This mod edits the A/B drives on the Voron V0.1 to allow for top-mounted nema17 motors.

## Why you should use nema17s instead of nema14s
TLDR: You shouldn't.
There is only one reason to run this mod and that is if you are trying to speed boat race. If that is not something that interests you this mod should not be installed on your machine. There will be no performance and/or quality increase from this mod under normal printing conditions. The stock nema14s will get you to speeds that will outperform the stock extrusion rate and stock cooling ability of the V0. This mod should only be considered if the motors are the bottleneck in your system and you need/want to go faster. Please see my list of reasons why to use/not use the mod below. If you decide you do not want to install this mod I also provided some alternative methods to increase the max speed of your system. 

### When to use this mod
- Your machine can extruder at a faster rate than your printer can run at
- Your cooling solution is outperforming my current speeds you print at
- I fit the above two conditions and I still want to go faster

### When not to use this mod
- Your machine can't extrude fast enough at the max speed with nema14s
- Your machine has problems with cooling at the max speed with nema14s
- You have not reached the limits with your current setup
- You use this machine for abs and need it to be fully enclosed (Tophat is not compatible with this mod)

## Other ways to reach faster speeds
- Increase the current on your motors
    - Please be aware of the currents your motors and stepper drivers are rated to. However, this is not the current that you will actually be able to use; it does not tell the whole story. You will run into overheating issues well before you hit the rated current. You can find more info elsewhere online if you want to learn more.
- Increase voltage of your motors
    - Please be aware of the voltage your components are rated to. Both your stepper drivers and controller boards need to be rated to the voltage you are running. The most common HV setup is 48v which will require 48v steppers drivers, a board with 48v sockets and a 48v psu. If your board/drivers are not up to spec they will instantly fry when you power on the machine and may start a fire. Additionally 48v is deadly and should be handled with the same precaution as mains power. Do not use 48v if you are not comfortable with it.  
- Decrease the weight of the moving mass
    - Since the V0 is a corexy machine this means decreasing the weight of the gantry. The first main way of doing this is replacing the aluminum extrusion with a carbon fiber one. Please be aware that cutting carbon fiber will release dangerous particulates into the air and proper protection must be used (your covid mask won't do anything). Also sufficient testing has not been done to fully understand the impact that this will have on rigidity and thermal warp due to heating the bimaterial gantry. It is believed that it will worsen both of these but there is not sufficient data to fully understand the degree it will do so. The second way to decrease weight is to move from a direct drive to a bowden system. However, this will obviously impact print quality negatively.

## BOM
##### Motors
The motors are the only additional parts that need to be bought as the hardware is the same as the stock V0. You can find the recommended motors below. I also recommend replacing your stepper drivers with something that can handle the current of larger motors. TMC2209s are only rated to 2 amps(can't go above 1.4 without cooling). I use 5160s for my stepper drivers.
##### Recommended Motors
- LDO-42STH47-2504AC
- NOC-17N18261A48MM-SJ

##### Printed Parts
You just need the six printed parts from the repo. You can use the normal tensioner nobs from the V0. The parts should be printed with the normal Voron part settings.

## Installation
The first thing you will need to do is remove the supports from the screw slots on the lower parts of the printed parts. After that the manual instructions can be followed for the most part. The only difference is that the motors will sit on top of the drives instead of the bottom.  Also the four screws that secure the drive to the frame should be put in place before attaching the motor. The motor will slightly block you from inserting them once it is attached.

## FAQ
Q: This is stupid nema14s provide more than enough power for such a small machine.
A: First of all thats not a question. Second of all I completely agree as I outlined multiple times above. This mod is only for speedboat racing. This mod will do nothing for you in normal printing conditions.

Q: Why are the motors on top of the a/b drives?
A: It was the only way to get them to fit without having a major overhaul to the frame/belt path. It also gives you more room for motor coolers and for extra/larger electronics on the back of the machine. The downside is that the tophat will no longer fit.