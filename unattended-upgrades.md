---
title: "Unattended Upgrades"
date: 2023-01-22T19:52:00-04:00
tags: [Raspberry Pi, apt-get unattended-upgrades]
---
To keep the Raspberry Pi (RPI) Operating System (OS) up-to-date, without performing the update/upgrade manual steps, the system can be configured to perform the upgrades itself.

## Prerequisites

- RPI
- [Raspberry Pi OS setup]( {{< ref "content/how-to/raspberry-pi/operating-system" >}})

## Steps

1. Login to the RPI.
1. Setup *Unattended Upgrades*.

   ```
   sudo apt-get install unattended-upgrades
   ```