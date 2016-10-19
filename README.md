# Mobile-Robot-Arm, Mr A.
Robotics project. 5 DoF motor based arm on a dual motor wheel base. Arduino and Raspberry Pi control.

Currently implemented.
----------------------

Control - Forward and reverse motor control in variable burst times via the serial to Arduino.

There are 22 Comands. 8 for arm control, forward and reverse on 4 'joint' motors, affected by the burstTime variable. 2 for the gripper, forward and reverse at a set time to cover fully open to close and the inversion. 9 for driving and steering control covering a variety of maneuvers. 2 for incrementing the burstTime variable up or down 1/4s. 1 to toggle spotlight on or off.

Commands are recieved sequencially and each motors starts and stops on it's own timer.

Progression to MVP (Minimal viable product).
------------

Power - Distinguish what power is needed and define a sutible source that is untethered and rechargeable.

Control- Gain feedback for motor position. Refine controls to perform motor movement based on duration of input. Define functions to perform specfic maneuvers for the arm. Amend variable burstTime to hold specific milliseconds.

Awareness- Install camera and ultrasonic sensors to gain an awareness of area surrounding Mr. A.

GUI- Requirents: Buttons to toggle each motor or system on/off. A window for serial feedback from Arduino, and a method to send serial data back. A viewing window for the camera feed. 
