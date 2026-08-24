# DIY Arduino Robot Arm - Controlled by Hand Gestures - Project16
Arduino Robotic Arm - Controlled by Hand Gestures
This project is a tutorial on how to build a DIY Robotic Arm controlled by hand gestures. The Robotic arm is able to be controlled wirelessly from a distance as well as perform basic functions on its own.
Robot Arm: Thingiverse 3D Printed Robotic Arm - https://www.thingiverse.com/thing:1748596
### Part 1: Gripper Parts
### Part 2: Base and Turntable
### Part 3: Robotic Core Arm

Robotic Glove: Thingyverse Robotic Glove/ Gauntlet - https://www.thingiverse.com/thing:1982745
### Robotic Glove

# Mark One Robotic Arm
Mark One is an Arduino-powered robotic arm prototype designed for object manipulation, gesture-based control, and wireless operation. It features a claw for gripping objects, six servo motors for multi-axis movement, and a stepper motor for base rotation.

This project also includes a robotic glove controller, allowing the arm to be operated through natural hand gestures using flex sensors and an accelerometer over Bluetooth.

# Project Overview
Mark One is a first-generation robotic arm built as a flexible and expandable prototype. The system is composed of two main parts: https://smartbuilds.io/

A robotic arm that performs movement and gripping tasks.

A robotic glove that sends gesture-based commands wirelessly.

The goal of the project is to create a practical robotics platform that can automate tasks such as object picking, arm positioning, and simple verification or interaction workflows.

# Features
Arduino-based robotic arm control.

Six servo motors for joint movement.

Stepper motor for smooth base rotation.

Claw/gripper mechanism for object handling.

Wireless communication using Bluetooth.

Gesture-based control using a robotic glove.

3D-printed mechanical structure.

Modular design for future upgrades and improvements.

# How It Works
The robotic arm works as a coordinated system of motors, where each motor controls a specific movement of the arm. The Arduino sends commands to the servo driver and stepper motor driver to control rotation, lifting, bending, and gripping.

The robotic glove acts as the input device. Flex sensors detect finger bending, while the accelerometer tracks hand motion. When a gesture crosses a defined threshold, the glove sends a command through Bluetooth to the robotic arm, which then performs the corresponding movement.

In short:

Sensors in the glove detect movement.

Bluetooth transmits the command.

Arduino on the arm receives the command.

Motors execute the action.

### Robot Arm: Thingiverse 3D Printed Robotic Arm 
•	Part 1: Gripper Parts
•	Part 2: Base and Turntable
•	Part 3: Robotic Core Arm
Robotic Glove: Thingyverse Robotic Glove/ Gauntlet - (credits: Roman 13)
•	Robotic Glove


The project involves creating a robotic arm, referred to as "Mark One," powered by Arduino. This robotic arm features a claw for object manipulation and is equipped with six motors to enhance its movement capabilities. It can be programmed to automate various tasks, such as completing verification forms or picking up objects.
The arm operates through coordinated movements of its motors, and it can be controlled using hand gestures, allowing for a more intuitive interaction. The wireless and portable design enables control from a distance without the need to program each action individually. The project includes building both the robotic arm and a corresponding robotic glove. The arm requires components such as an Arduino, six servo motors, a stepper motor, a servo driver, a battery, a Bluetooth module, jumper wires, and a breadboard. The glove is made using a smaller Arduino Nano, a breadboard, a flex sensor, an accelerometer, and another Bluetooth module for communication.

The project described involves the development of a robotic arm, referred to as "Mark One," which is powered by Arduino and designed for various automation tasks, including object manipulation and gesture control. Here are the key conclusions and results from the project:

## Project Overview
- **Robotic Arm Features**: The robotic arm consists of six servo motors that provide enhanced movement capabilities and a claw mechanism for picking up objects. It is programmable via Arduino, enabling automation of tasks like filling out capture forms and picking up items.
- **Gesture Control**: A significant feature of this prototype is its ability to be controlled using hand gestures through a robotic glove equipped with sensors, allowing for a more intuitive interaction with the arm.

## Technical Implementation
- **Components Used**: The assembly includes an Arduino board, six servo motors for joint movement, a stepper motor for base rotation, Bluetooth modules for wireless communication, and various sensors (flex sensors and accelerometers) for the glove.
- **3D Printing**: The arm was constructed using 3D printing technology, which allowed for customization of parts and facilitated the integration of components such as LED indicators in the gripper.

# Hardware Requirements
Robotic Arm
Arduino board

6 servo motors

1 stepper motor

Servo driver board

Battery for servo driver

Bluetooth module

Jumper wires

Breadboard

3D-printed robotic arm parts

# Robotic Glove
Arduino Nano

Breadboard

Flex sensor

Accelerometer

Bluetooth module

10K ohm resistor

Jumper wires

3D-printed glove parts or standard glove base

## Performance and Functionality
- **Operational Testing**: Upon assembly, the robotic arm demonstrated responsiveness to hand gestures, although initial tests indicated that sensitivity adjustments were necessary to prevent unintended movements. The programming involved creating functions that allowed the arm to perform specific tasks based on sensor input from the glove.
- **Future Improvements**: The project noted that while the current prototype is functional, there is room for enhancements in terms of programming accuracy and fluidity of motion. Future iterations may include additional sensors or refined control algorithms to improve performance.

## Conclusion
The "Mark One" robotic arm project successfully achieved its primary goals of creating a programmable robotic arm capable of gesture-based control. It showcases the potential of Arduino in robotics and opens avenues for further development, potentially leading to more sophisticated versions in future iterations (e.g., "Mark Two"). The project emphasizes both educational applications and practical uses in automation tasks, illustrating the interdisciplinary nature of robotics development.

### In summary, 
the robotic arm is designed to work collaboratively with the glove, allowing users to control it through gestures. The project serves as a prototype with potential for further development, and detailed instructions, including a part list and code, are provided for those interested in replicating the build.

### Robotic Arm
The robotic arm is assembled from 3D-printed components and mounted with six servo motors for each joint. A stepper motor is used at the base to improve rotational movement. The claw is attached at the end of the arm for gripping and releasing objects.

### Robotic Glove
The glove is built around motion sensors that track finger bending and hand movement. Flex sensors are mapped to individual fingers, while the accelerometer helps detect directional movement. The glove can be worn comfortably and communicates with the robotic arm wirelessly.

# Programming Logic
The project uses two main Arduino programs:

1. Robotic Arm Code
Initializes servo and stepper motor control.

Uses a servo driver library to control multiple servos.

Listens for Bluetooth commands from the glove.

Executes movements such as claw opening, wrist rotation, arm lifting, and base rotation.

2. Robotic Glove Code
Reads values from flex sensors and accelerometer.

Detects when a gesture exceeds a defined threshold.

Sends commands over Bluetooth to the arm.

Works as a wireless controller for the robotic system.

# Performance
The prototype demonstrates responsive gesture-based control and functional movement across multiple joints. It successfully performs tasks such as claw movement, arm rotation, and gesture-driven interaction.

During testing, some sensitivity tuning was required to avoid false triggers, but overall the system proved effective and stable for a first prototype.

## Possible Applications
Robotics learning and prototyping.

Gesture-controlled automation.

Object picking and movement tasks.

Human-robot interaction experiments.

DIY mechatronics and embedded systems projects.

## Future Improvements
Add more sensors for finer gesture detection.

Improve motion smoothness and response accuracy.

Enhance the control algorithm to reduce false positives.

Expand the glove to support more fingers and gestures.

Develop a second-generation version: Mark Two.

# Project Structure

mark-one-robotic-arm/
├── arm_code/
├── glove_code/
├── models/
├── docs/
├── images/
├── README.md
