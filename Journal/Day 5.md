# Day 5 - Battery and Power Consumption Investigation

Date: June 15, 2026

## Objective

Investigate poor battery life and determine whether the issue was caused by battery degradation, hardware configuration, or excessive power consumption.

## Background

I accidentally left my laptop unplugged overnight and the battery completely discharged. After restoring the system, I decided to investigate my battery health and overall power consumption.

## Accomplishments

Installed the following tools using Pacman:

* Powertop
* Inxi

Used Linux power management and hardware diagnostic tools to gather information about the system.

## Findings

### Battery Health

Using Upower, I determined:

* Design Capacity: 48 Wh
* Current Capacity: 37.1 Wh
* Battery Health: 77%

The battery has lost approximately 23% of its original capacity but is still considered functional.

### Power Consumption

Initial testing showed approximately:

* 40 W power draw while charging

Additional testing while running on battery showed:

* Approximately 21 W power draw

This indicated that the earlier 40 W reading was not representative of normal battery usage.

### Graphics Investigation

Using Inxi and NVIDIA-SMI, I discovered:

* Intel UHD Graphics is rendering the desktop environment.
* The NVIDIA RTX 3050 Ti Mobile GPU is installed and available.
* The NVIDIA GPU was consuming approximately 16 W while idle.

Further investigation showed:

* Runtime Power Management was enabled.
* Runtime Status was "suspended."
* Power Control was set to "auto."

This indicates that Linux is already managing the dedicated GPU correctly and placing it into a low-power state when not actively being used.

## Conclusion

The battery is degraded but not severely damaged. The laptop appears to be operating normally for its hardware configuration, and Linux power management is functioning correctly.
