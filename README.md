# Quadrapod-spider-robo
An ardiuno microcontroller project along with sensor and servo controlling to build a four leg spider (Quadrapod robot) using C++ language

Arduino-Based Bluetooth Controlled Quadruped Robot
**1. Project Overview**
This project is a four-legged (quadruped) spider robot designed using an Arduino Uno. The robot uses twelve servo motors to control leg movement, an HC-05 Bluetooth module for wireless control, and an HC-SR04 ultrasonic sensor for obstacle detection. The system is powered through a buck converter with a common ground shared with the Arduino.
**2. Objectives**
- Design and build a stable quadruped robot.
- Implement coordinated walking gaits.
- Enable wireless control using Bluetooth.
- Detect obstacles using ultrasonic sensing.
- Demonstrate embedded systems, robotics, and servo control concepts.
**3. Hardware Components**
• Arduino Uno
• 12  MG90s Servo Motors (3 per leg)
• HC-05 Bluetooth Module
• HC-SR04 Ultrasonic Sensor
• XL-4016 Buck Converter Power Supply
• Chassis and Leg Assembly
• Connecting Wires and Power Distribution
**4. Leg Configuration**
L1 = Front Left
L2 = Front Right
L3 = Back Left
L4 = Back Right

Diagonal pair arrangement:
Pair A: L1 + L4
Pair B: L2 + L3
5. Pin Connections
Bluetooth:
TX -> D9
RX -> D10

Ultrasonic Sensor:
Echo -> A4
Trig -> A5

Servo Pins:
L1: D2, D3, D4
L2:  D5, D6, D7
L3: A0, A1, A2
L4: D11, D12, D13 

Unused Pin: D8
**6. Power Distribution**
All servos and modules are powered through a buck converter. The ground of the buck converter is connected to the Arduino ground to ensure proper signal referencing.
**7. Working Principle**
The Arduino generates PWM signals for the servos. Bluetooth commands received through the HC-05 control movement. The ultrasonic sensor measures distance to obstacles and can be used for collision avoidance. The robot walks using a diagonal-pair gait where L1/L4 and L2/L3 move alternately.
**8. Software Design**
Main functions include:
• Standing posture
• Forward walking
• Turning left/right
• Bluetooth command processing
• Obstacle detection
**9. Gait Description**
The robot uses a diagonal-pair gait. During movement, L1 and L4 move together while L2 and L3 support the body. The cycle then alternates, allowing continuous forward motion with improved speed and reasonable stability.
**10. Applications**
• Robotics education
• Embedded systems learning
• Motion control experiments
• Autonomous navigation research
• Demonstration and exhibition projects
**11. Future Improvements**
• Inverse kinematics implementation
• Camera integration
• Autonomous navigation
• Improved gait optimization
• Mobile application control
**12. Conclusion**
The quadruped spider robot demonstrates the integration of mechanics, electronics, and programming in a single system. The project successfully achieves wireless control, coordinated leg movement, and obstacle sensing, providing a practical platform for robotics development and experimentation.
