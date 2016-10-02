# Mobile-Robot-Arm, Mr A.
Arduino robotics project. 5 motor arm on a dual motor wheel base.

Currently implemented.
----------------------

Control - Forward and reverse motor control via the serial to Arduino in variable burst times.

There are 22 Comands. 8 for arm control, forward and reverse on 4 'joint' motors, affected by the burstTime variable. 2 for the gripper, forward and reverse at a set time to cover fully open to close and the inversion. 9 for driving and steering control covering a variety of maneuvers. 2 for incrementing the burstTime variable up or down 1/4s. 1 to blink spotlight for a variable duration.

Commands are recieved sequencially and each motors starts and stops its own timer.
