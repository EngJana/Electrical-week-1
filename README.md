# Electrical-week-2-task-2
‏week 2 in smart methods internship. 
‏task 2: electronic circuit connection and code


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

