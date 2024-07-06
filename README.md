# Electrical-week-1
week 1 in smart methods internship 


## Robot Walking Algorithm
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
