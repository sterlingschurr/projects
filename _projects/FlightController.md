---
title: Custom Autonomous Drone Flight Controller - for Hill Air Force Base
skills: [NuttX RTOS, C++, PX4 Autopilot, SPI, I2C, USB, PCB Design, SI/PI, Altium, Keysight ADS, STM32]
date: 2026-07-24
---

![Project Cover Photo](/assets/images/FlightControllercoverimage.png)
As part of a team of 4, created a custom drone flight controller capable of running PX4 autopilot software

****This project has a completed report in PDF format that is more thorough than this page will be. [Click Here](/assets/documents/flightcontrollerreport.pdf) to access that report.**

## The Problem
The United States is heavily reliant on China for the production of electronics. For applications of defense, it is better to own one's intent and to control the design and production of devices. One emerging technology in defense is drones. A vast majority of drone controllers and the components that go into them are produced overseas. This opens the door for other people to influence our defense strategies in ways we don't want.

## The Solution
![Concept diagram](/assets/images/FlightControllerconceptdiagram.png)
Hill Air Force Base asked if we could produce a domestically-designed flight controller capable of autonomous flight. We inherited a half-completed project from another team that needed to be redesigned, manufactured, and tested. This project came with two sets of requirements: The required outcome of the project, and the required actions to be taken based on the previous team's work to get there.

### Base Requirements
These are the base vision of the project.
- NDAA-Compliant
- Running custom or open-source firmware
- Compatible with common off-the-shelf solutions for ESCs, Controllers, Telemetry, etc.
- Future compatibility with a drone swarm configuration

### Relative Requirements
These are the things we had to do to relative to our starting point to achieve the desired product.
- Verify and manufacture PDB (Power Distribution Board)
- Select new processor and reroute PCB for it
- While rerouting PCB, reduce design from 6 to 4 layers
- Solve firmware issues that previous teams couldn't

## The Execution
![Wiring diagram](/assets/images/FlightControllerwiringdiagram.png)

Part of the construction on the board was interfacing it with a PDB (power distibution board, seen above). We were provided almost-finished but outdated schematics for this board. We had to update these, manufacture the PDB, and then make sure it interfaced with our flight controller design.

We completed all of our hardware objectives. We were able to make both boards and they interfaced as they should. 

Our software goals were unfortunately derailed by poor support from the PX4 project. While they claimed they could handle the STM32 processor we had installed, there were a few glaring issues. The largest was not supporting the SDMMC port that the controller used, which meant we could not save settings, and therefore couldn't operate the drone fully. We were working on a solution for this until the end of the project.

This is a quick summary of the execution, refer to the [original fulll report](/assets/documents/flightcontrollerreport.pdf) to see everything we did.

![Actual photo of the thing](/assets/images/FlightControlleractualphoto.jpg)

## Next Steps
The next steps for this design is to align the system with reference designs provided by PX4. This will give frictionless software support and allow for more time using the drone rather than creating custom software fixes. Our hardware was solid but the software prevented us from seeing full functionality. 

The original project definition wanted there to be room for integrating this design into a swarm configuration. That's beyond my part of the project, but that would be the big-picture next steps after this controller is complete.