# Electrical-week-1-task-1
week 1 in smart methods internship. 
task 1: Robot Walking Algorithm
task 2: electronic circuit connection and code


# task 1: Robot Walking Algorithm

This repository contains a code and a simulation that implements a simple algorithm for controlling the movement of a robot using six servo motors. Each servo motor controls a joint in the robot's legs: the left and right hips, knees, and ankles.

## Algorithm Overview
The walking algorithm moves the robot's legs through a sequence of four steps to simulate a walking motion:
1. Move the right leg forward:
   - The left hip is kept in a neutral position (90 degrees).
   - The right hip is moved forward (45 degrees).
   - The left knee is kept straight (90 degrees).
   - The right knee is bent (135 degrees).
   - The left ankle is kept in a neutral position (90 degrees).
   - The right ankle is adjusted (45 degrees).
   - The robot waits for 500 milliseconds to complete this step.
2. Move the right leg back to neutral:
   - The right hip is moved back to the neutral position (90 degrees).
   - The right knee is straightened (90 degrees).
   - The right ankle is moved back to the neutral position (90 degrees).
   - The robot waits for 500 milliseconds to complete this step.
3. Move the left leg forward:
   - The left hip is moved forward (45 degrees).
   - The right hip is kept in the neutral position (90 degrees).
   - The left knee is bent (135 degrees).
   - The right knee is kept straight (90 degrees).
   - The left ankle is adjusted (45 degrees).
   - The right ankle is kept in the neutral position (90 degrees).
   - The robot waits for 500 milliseconds to complete this step.
4. Move the left leg back to neutral:
   - The left hip is moved back to the neutral position (90 degrees).
   - The left knee is straightened (90 degrees).
   - The left ankle is moved back to the neutral position (90 degrees).
   - The robot waits for 500 milliseconds to complete this step.

## Explanation of Angles and Movement
1.	Hip Joints
    - Neutral Position (90 degrees): This angle keeps the leg aligned vertically under the body.
    - Forward Position (45 degrees): This angle moves the leg forward, simulating the forward step of the walk cycle.
2.	Knee Joints
    - Straight (90 degrees): This angle keeps the leg straight, providing stability and support.
    - Bent (135 degrees): This angle allows the leg to bend, lifting the foot off the ground to move forward.
3.	Ankle Joints
    - Neutral Position (90 degrees): This angle keeps the foot flat, providing stability.
    -Adjusted (45 degrees): This angle adjusts the foot position to facilitate the forward movement and prevent dragging.

## Movement Sequence Explanation 
1. Move the right leg forward:
    - The left hip remains neutral to support the body.
    - The right hip moves forward, bringing the right leg forward.
    - The left knee remains straight to provide stability.
    - The right knee bends to lift the foot off the ground.
    - The left ankle stays neutral to anchor the body.
    - The right ankle adjusts to help clear the ground as the leg moves forward.
    - The robot waits for 500 milliseconds to allow the movement to complete.
2. Move the right leg back to neutral:
    - The right hip moves back to the neutral position, aligning the right leg under the body.
    - The right knee straightens to support the body.
    - The right ankle adjusts back to the neutral position for stability.
    - The robot waits for 500 milliseconds to allow the movement to complete.
3. Move the left leg forward:
    - The left hip moves forward, bringing the left leg forward.
    - The right hip remains neutral to support the body.
    - The left knee bends to lift the foot off the ground.
    - The right knee remains straight to provide stability.
    - The left ankle adjusts to help clear the ground as the leg moves forward.
    - The right ankle stays neutral to anchor the body.
    - The robot waits for 500 milliseconds to allow the movement to complete.
4. Move the left leg back to neutral:
    - The left hip moves back to the neutral position, aligning the left leg under the body.
    - The left knee straightens to support the body.
    - The left ankle adjusts back to the neutral position for stability.
    - The robot waits for 500 milliseconds to allow the movement to complete.
    - By repeating this sequence, the robot alternates moving its legs forward and backward, simulating a walking

motion. The carefully chosen angles ensure that each leg moves smoothly and efficiently, providing stability and forward propulsion.



# task 2: electronic circuit connection and code


## Code and Hardware Explanation
The code is written in C++ and uses the Arduino Servo library to control the six servo motors. 
Using tinkercad the robot walking algorithm was prototyped and tested in Tinkercad, a free online collection of software tools. It’s particularly useful for simulating Arduino projects, allowing for virtual testing and debugging before applying the design to physical hardware. This helps in refining the code and ensuring that the servo movements are correctly calibrated.
All the servo motors are connected to digital pins that support PWM (Pulse Width Modulation) because of:
1. Precise Control: PWM allows for precise control of the servo motor positions by varying the duty cycle of the signal. This precision is necessary for accurately positioning the robot's joints.
2. Compatibility: The Arduino Servo library uses PWM signals to control the angle of the servo motors. 
3. Smooth Movement: PWM signals provide smoother transitions between positions, which is crucial for creating a realistic walking motion.
4. Frequency Requirements: Servos typically require a control signal at a frequency of around 50Hz, which can be achieved using PWM.

## Pin Configuration
The servo motors are connected to the following pins on the microcontroller:
- servo1 (Left Hip): Pin 3
- servo2 (Right Hip): Pin 5
- servo3 (Left Knee): Pin 6
- servo4 (Right Knee): Pin 9
- servo5 (Left Ankle): Pin 10
- servo6 (Right Ankle): Pin 11

## Code Explanation
- Setup:
Each servo is attached to its corresponding pin using the attach() method.
- Loop:
The loop() function executes the four-step walking sequence by sending the appropriate angle values to each servo motor.
The write() method is used to set the angle of each servo.
The delay() function is used to pause the execution of the code for 500 milliseconds between each step, allowing the servos to move and the robot to take a step.

## Hardware Setup
1.	Microcontroller: An Arduino board or any other microcontroller that supports the Servo library.
2.	Servo Motors: Six high-torque servo motors, one for each joint in the robot's legs.
3.	Power Supply: A power supply capable of providing sufficient current to power the microcontroller and the servo motors.
4.	Wiring: Wires to connect the servo motors to the microcontroller pins.
5.	Battery: A battery to power the entire setup. 

## Additional Notes
Ensure that the power supply can handle the current requirements of all six servos to avoid any power issues. 
Which is why an external battery is used, not the Arduino pins.

## link to the circuit simulation and code
[circuit simulation and code - tinkercad](https://www.tinkercad.com/things/lD6dzlsb2xt-6-servo-motor-for-robot-leg?sharecode=GoIJS240_Iz05Z_M5n-4MhHNNRy84VRbI7NH6hysV7I) 

