---
title: "Operating System"
date: 2022-01-22T16:53:00-04:00
tags: [Raspberry Pi, Operating System, apt-get update, apt-get upgrade]
---
The Raspberry Pi OS is the default operating system for an RPI SBC.  It is based on a Debian linux and configured for usage with the RPI.

## Prerequisites

- Acquire an RPI SBC
  - [PiShop.ca](https://www.pishop.ca/)
  - [CanaKit](https://www.canakit.com/)
  - [ThePiHut](https://thepihut.com/)
  - [Pimoroni](https://shop.pimoroni.com/)
- Acquire a micro-SD card

## Steps

1. Download the Raspberry Pi Imager from [Raspberry Pi OS](https://www.raspberrypi.com/software/) onto a computer that will prepare the mirco-SD card.
1. Insert the micro-SD card.
1. Run the Raspberry Pi Imager software.
1. Choose the version of the OS:

   - Raspberry Pi OS with Desktop for a GUI experience
   - Raspberry Pi OS Lite for a terminal/headless experience

   And either 32 bit, for any RPI board, or 64 bit, for RPI version 3 (or more recent) boards, option.
1. Under settings, specify the user and password, network information, and enable SSH.
1. Write the OS to the micro-SD.
1. Insert the micro-SD into the RPI.
1. Turn on the computer.
1. Wait for system to configure on first boot.
1. Login to the computer.
1. Update the repositories.
   ```
   sudo apt-get update
   ```
1. Upgrade the applications.
   ```
   sudo apt-get upgrade
   ```
      
## References

- [Raspberry Pi OS](https://www.raspberrypi.com/software/)

*[GUI]: Graphical User Interface
*[OS]: Operating System
*[RPI]: Raspberry Pi
*[SBC]: Single Board Computer
*[SD]: Secure Digital
*[SSH]: Secure Shell