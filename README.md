# Mobile-Robot-Arm, Mr A.
Arduino robotics project. 5 motor arm on a dual motor wheel base.

Currently implemented.
----------------------

Control - Forward and reverse motor control in variable burst tims via the serial to Arduino.

There are 22 Comands. 8 for arm control, forward and reverse on 4 'joint' motors, affected by the burstTime variable. 2 for the gripper, forward and reverse at a set time to cover fully open to close and the inversion. 9 for driving and steering control covering a variety of maneuvers. 2 for incrementing the burstTime variable up or down 1/4s. 1 to blink spotlight for a variable duration.

Commands are recieved sequencially and each motors starts and stops its own timer.

Progression to MVP (Minimal viable product).
------------

Power- Distinguish what power is needed and define a sutible source that is untethered and rechargeable.

Control/Commands- Gain feedback for motor position. Refine controls to tackle motor movement based on duration of input. Define functions to perform specfic maneuvers, i.e. move arm efficiently from current extended position to deposit area on wheelbase. Amend variable burstTime to hold specific milliseconds. 

Controller- Design and develop a tethered handheld device capable of sending commands to Mr A.
