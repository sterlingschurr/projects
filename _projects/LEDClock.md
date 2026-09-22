---
title: RGB LED Matrix Wall Clock
skills: [3D Printing, 3D Modeling, Embedded Systems, I2C, Arduino, C]
date: 2024-09-09
---

![Project Cover Photo](assets/images/LEDClockcoverimage.jpg)
Digital wall clock featuring slim design, user configuration, custom color generation, and light sensitivity for automatic dark mode.

## The Idea
Addressable LEDs are cheap and easy to use. I wanted to use this technology to may advantage and make a 2-dimensional LED array and use it to display the time.

## The Plan
![Concept diagram](assets/images/LEDClockconceptdiagram.jpg)
Using a zig-zaggin pattern, I would be able to align the strip of LEDs in a grid. Using a lookup table I could then display numbers fairly easily through the matrix. In a custom 3D printed case, the clock would be able to diffuse the lights and make them appear as square pixels. An arduino with a RTC module could handle the time keeping and color coordination.

## The Execution
![Wiring diagram](assets/images/LEDClockwiringdiagram.jpg)
How the actual construction went, and how it differed from expectations
![Actual photo of the thing](assets/images/LEDClockactualphoto.jpg)

## Next Steps
what I didn't have time to do, how I could improve on this in the future
