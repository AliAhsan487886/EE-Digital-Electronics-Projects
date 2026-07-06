# DIP-Switch Controlled 7-Segment Display Board

A perfboard-prototyped digital logic circuit that uses **DIP switches** as inputs and drives a **single 7-segment display** to Display binnary numbers in decimal form o seven segment, built through an IC.

<img width="3658" height="1716" alt="PROJECT_Board" src="https://github.com/user-attachments/assets/d2536aed-ead8-453f-8740-f308dd9f4b76" />

## Overview

- Power input via a 2-pin screw terminal, with a smoothing/reservoir capacitor
- An indicator LED on the input side
- A bank of 4 DIP switches (with two earlier revisions using an 8-position DIP switch bank instead)
- A DIP-package IC decoding the switch inputs to segment outputs
- Series resistors on each segment line for current limiting
- Single common 7-segment display as output

## Bill of Materials 

| Component | Value / Part | Notes |
|---|---|---|
| DIP switch | 4-way (final version) / 8-way ×2 (earlier version) | Input selection |
| IC | *TBD* (DIP package) | Decoder / logic |
| Resistors | Mixed values (color-band, ~4 visible on segment lines + a few on switch lines) | Current limiting / pull-up-down |
| 7-segment display | Common cathode/anode, single digit | Output |
| LED | Red, 3mm | Power/status indicator |
| Capacitor | Electrolytic, near terminal block | Power smoothing |
| Terminal block | 2-pin screw terminal | Power input |

## Status

Prototyped and tested on perfboard — confirmed displaying output as shown in the photo above.
