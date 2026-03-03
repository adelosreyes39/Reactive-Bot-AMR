# Reactive-Bot-AMR
1. Project Objective
The goal of this project is to implement a fundamental reactive navigation system for a mobile robot. The robot autonomously navigates a 3D MuJoCo environment, identifying and avoiding static obstacles in real-time without requiring a pre-generated map. 
+1

2. Key Features
Reactive Logic: Uses a simple state machine (Forward, Turn, Recovery) to manage wheel velocities based on sensor data. 

Sensor Integration: C++ logic parses distance data from a simulated LiDAR/Range-finder. 

Physics-Based Simulation: Leverages MuJoCo's engine for realistic collisions and wheel friction. 

Sim-to-Real Path: Control logic is designed to be ported to physical hardware (Arduino or Raspberry Pi) using ultrasonic or infrared sensors. 

3. Software Components
Programming: C++ (Logic) and MJCF/XML (Robot and Environment Modeling). 

API: MuJoCo API for sensor processing and motor control. 

Model: A custom-developed differential-drive robot model. 

4. Repository Structure
Plaintext
├── docs/               # Weekly milestones and documentation 
├── model/              # MJCF (XML) robot and environment files [cite: 16, 24]
├── src/                # C++ source code for control and sensors [cite: 11, 24]
└── README.md
5. Development Roadmap
Weekly milestones, including video captures of simulation progress, are documented on the project website. 

[ ] Initialize custom MJCF robot model. 

[ ] Implement LiDAR data parsing in C++. 

[ ] Develop the "Forward, Turn, Recovery" state machine. 

[ ] Test 'Sim-to-Real' parity on physical hardware. 

6. License
This project is open-source. All C++ source code and the robot's XML model are available for use and modification.
