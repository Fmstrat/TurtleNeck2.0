# This is a legacy project - you do NOT need it -
# TN Pro V2.0
![TN2_Render](https://github.com/user-attachments/assets/04dee60e-6889-46bf-8f6b-388c52244336)
TurtleNeck Pro - The smart toolhead buffer.

AT Discord:

[![Join me on Discord](https://discord.com/api/guilds/1229586267671629945/widget.png?style=banner2)](https://discord.gg/armoredturtle)

TurtleNeck Pro (TNP) Is a toolhead buffer for klipper printers designed to work with the [AFC Klipper Add-on](https://github.com/ArmoredTurtle/AFC-Klipper-Add-On).
It ustilizes an STM32G0B1 MCU over usb-c to operate. Making it a single cable addition to your klipper machine.

TNP utilizes two hall effect sensors to dectect movement of the buffer before hitting a hard stop in either direction. Adiddtionally on the PCB are 5 endstops ports that can be utilized for filament combiners or "hubs".
The purpose of a toolhead buffer such as TNP is to compensate for mismatched rotation distances between a toolheads extruder and a direct drive AFC ("type 2 MMU" if you like calling them that...)
TN2.0 MCU uses JST-PH connectors for all of its expansion.

[Build manual HERE](https://armoredturtle.xyz).

#BOM#
| Part  | QTY |
| ------------- | ------------- |
| TN2.0 PCB | 1  |
| 3x2mm magnet  | 1  |
| M2.5x10 FHCS  | 1  |
| ECAS04 bowden collet | 2  |
| M3x8 SHCS | 4  |
| M3x10 FHCS | 2 |
| M3 Heatset insters | 4  |
| 1mm Felt adhesive backed |~1x10mm X4 |


![TN2 0 Pins](https://github.com/user-attachments/assets/540bb77b-cc90-49a5-84fc-ba7ac245fbd7)


#Pins of note#
| Device | Pin |
| ---------------- | ----- |
| USB coms | PA11/PA12 |
| Trailing hall effect sensor | PB1 |
| Advance hall effect sensor | PB2 |
| Endstop 1 | PB5 |
| Endstop 2 | PB6 |
| Endstop 3 | PB7 |
| Endstop 4 | PB8 |
| Endstop 5 | PB9 |
| RGB (neopixel) | PD3 |

#Schematic
![Schematic_TurtleNeck_2024-10-13](https://github.com/user-attachments/assets/c11a8c29-cd33-466f-b604-7e2d9ea658bc)
