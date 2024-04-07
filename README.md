# Lunar Rover Software for MARCIE

## Overview
This repository houses the software developed for the MARCIE Lunar Rover. The software encompasses the architecture and flow essential for the rover's operation on the lunar surface, focusing on mission-critical processes such as power management, navigation, and data transmission.

### Key Components
- **Software Architecture**: Utilizes the RAD5545 processor for its reliability and robust memory alongside Single Board Computers (SBCs) for enhanced functionality.
- **Communication**: Employs wireless communication between the Mission Operator System, the base system, and the rover, with Ethernet for software communications.
- **Software Framework**: The Core Flight Executive (cFE) provides a stable software framework, facilitating reliable component communication.
- **Instrument Interface**: Software interfaces with various instruments (indicated in green) to gather and transmit data effectively.

![Software Architecture](https://imgur.com/zJLUnpS.png "Software Architecture Diagram")

## Software Flow
Outlined in the provided flowchart, the software decision-making process initiates with a power assessment. Insufficient power levels engage a charging phase, followed by antenna deployment and landing site evaluation. The rover then calibrates its instruments, updates mission control, and initiates autonomous navigation to avoid obstacles and perform scientific tasks.

![Rover/Software Flow](https://imgur.com/x5V7S9U.png "Rover/Software Flow Diagram")

## Repository Structure
- `RoverFlow.cpp`: Implements the rover's mission operations in C++, including power checks, antenna deployment, instrument calibration, and autonomous navigation.
- `SoftwareArchitecture.png`: Illustrates the software architecture, highlighting developed applications and supporting software components.
- `SoftwareFlow.png`: Depicts the rover's software decision-making process from mission start through navigation to data transmission.

## Getting Started
To run the rover simulation:
1. Ensure C++17 or later is installed on your system.
2. Compile `RoverFlow.cpp` using your preferred C++ compiler, e.g., `g++ -std=c++17 RoverFlow.cpp -o RoverFlow`.
3. Execute the compiled program: `./RoverFlow`.

## Dependencies
- C++17 or later for compiling the simulation code.
- No external libraries are required for the basic simulation.

## Acknowledgments
This software leverages the Core Flight Executive (cFE) and AutoNav, components previously utilized in notable missions like VIPER and Perseverance. This reusability significantly reduces the risk factor by incorporating tested and proven software elements.

## Contact
Harlan Phillips - harlanphillips74@gmail.com

Project Link: [https://github.com/yourusername/yourrepositoryname](https://github.com/yourusername/yourrepositoryname)
