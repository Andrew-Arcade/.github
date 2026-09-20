<img src="../logo/andrew-arcade-banner.png">

#

### About Andrew Arcade

Andrew Arcade is a custom game console built with a Raspberry Pi 5 running Linux. Its main purpose is to play video games that I (and others) have created.

Designed for makers who love both hardware and software.

Hardware:
The system is designed around the Raspberry Pi 5. A screen and and controller plug in and integrate seamlessly with the design of the device. The controller is a custom pcb holding a Waveshare Zero running [GP2040-CE](https://github.com/OpenStickCommunity/GP2040-CE) designed for buttons and joystick to be easily plugged in and swapped out via simple jst connections. It has a full gamepad setup with two joysticks and ten buttons for the normal Up/Down/Left/Right, A/B/X/Y, and Start/Option controller layout. Everything mounts to a 3d printed case which houses the system cleanly.

Software:
The Raspberry Pi 5 is running [DietPi](https://github.com/MichaIng/DietPi), a minimal Linux distribution designed for the Raspberry Pi 5. We have an application we call the Driver, it is effectively the home screen of the console and is loaded on startup. In the Driver you can run and manage your installed cabinets (games/apps) and shutdown/resetart/sleep the system. The driver installs cabinets from their repositories, using a standardized file to read metadata about the cabinet before installing/updating. The controller module/pcb runs [GP2040-CE](https://github.com/OpenStickCommunity/GP2040-CE), an opensource firmware for emulating controllers over hid. It may seem complicated to setup the software but it is very simple, we have a very detailed guide and once you get the os installed to the Raspberry Pi 5 all you need to do is run a single script to get everything setup (autostart/users/file structures, etc...).
