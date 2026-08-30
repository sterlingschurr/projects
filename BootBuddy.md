# Boot Buddy
Intermediary controller to handle booting a HTPC from a controller

# The Problem
Many people create home theater PCs (HTPCs) for gaming purposes. A small PC connected to a TV can play the same games as an Xbox or a Playstation with better performance per dollar and a more open ecosystem. However, these PCs often have integration challenges preventing a seamless experience.
One such challenge is the ability to control the entire experience from a controller. Windows OS is made primarily as desktop-first, and Microsoft has no tools for using a PC in this context. The Boot Buddy intends to bridge this gap 

# The Solution
## Decided features
The Boot Buddy will be a hardware solution. It will have a small microcontroller (likely an ESP32) that is always on. When someone turns on their controller an presses the guide button, the microcontroller will be able to send a signal to the front panel header of the host PC telling it to boot up. Once the boot is detected, the BB will drop the connection to the game controller, which will then be free to connect to the HTPCs Bluetooth. 

## Undecided Features
- Keeping the bluetooth connection to the BB and forwarding controller signals via USB. This will allow for mouse and keyboard emulation, for navigation. But this might better be solved with software.
- Smart home integration, boot from your Alexa or whatever.

# The Execution
This Project is not yet done. Stay tuned!

# Next Steps
This Project is not yet done. Stay tuned!
