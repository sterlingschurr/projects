---
title: Superfan
skills: [3D Modeling, 3D Printing, Arduino, Lithium Batteries, Circuit Design]
date: 2022-06-06
---

![Project Cover Photo](assets/images/superfancover.jpg)

Superior personal comfort using a brushless motor and a custom controller.

## The Problem
Personal fans are weak. They don't move enough air beyond providing a slight comfort, and they aren't useful for any other sort of application. I wanted something stronger.

## The Solution
![Concept diagram](assets/images/superfanconceptdiagram.jpg)

The general idea is just to add more power to a handheld fan. I planned to create a fan powered by a brushless motor and ESC from a drone, as those are designed to move the most air possible. To generate throttle signals to the ESC I would have a small microcontroller providing the PWM on a circuit board. It should be reasonably ergonomic and have variable throttle. 

## The Execution
![Wiring diagram](assets/images/superfanwiringdiagram.jpg)

I wanted the throttle to be a spring-loaded potentiometer, but those were much harder to source than I thought and I wasn't willing to make my own for safety concerns. I decided to use 3 buttons on the circuit board for low/medium/high throttle. I also added a step-up function so the motor could get up to speed.

The housing, while functional, isn't perfect. The assembly and printing is a little difficult, and it only screws in on one side, leading to flex in the body.

![Actual photo of the thing](assets/images/superfanactualphoto.jpg)

## Next Steps
- Strenghten housing design
- Change to usb-rechargable power delivery
- Folding propeller
- Spring-loaded throttle for finer control 