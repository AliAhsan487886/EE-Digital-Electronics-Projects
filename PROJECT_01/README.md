# DIP-Switch Controlled 7-Segment Display Board

A perfboard-prototyped digital logic circuit that uses **DIP switches** as inputs and drives a **single 7-segment display**, built through an IC in a 14/16/18-pin DIP package (part number to be confirmed).

![Assembled board](./images/EX1.jpg)

## Overview

- Power input via a 2-pin screw terminal, with a smoothing/reservoir capacitor
- An indicator LED on the input side
- A bank of 4 DIP switches (with two earlier revisions using an 8-position DIP switch bank instead)
- A DIP-package IC decoding the switch inputs to segment outputs
- Series resistors on each segment line for current limiting
- Single common 7-segment display as output

An earlier/alternate revision of the board (below) used two 8-way DIP switch banks and additional header pins, likely for testing more input combinations or a wider bus:

![Earlier board revision](./images/Ex_2.jpg)

> Note: confirm and fill in the exact IC (e.g. 74LS47 / CD4511 / a microcontroller) and the switch-to-segment truth table once verified — this README currently describes the board from visual inspection.

## Bill of Materials (as identified from the board)

| Component | Value / Part | Notes |
|---|---|---|
| DIP switch | 4-way (final version) / 8-way ×2 (earlier version) | Input selection |
| IC | *TBD* (DIP package) | Decoder / logic |
| Resistors | Mixed values (color-band, ~4 visible on segment lines + a few on switch lines) | Current limiting / pull-up-down |
| 7-segment display | Common cathode/anode, single digit | Output |
| LED | Red, 3mm | Power/status indicator |
| Capacitor | Electrolytic, near terminal block | Power smoothing |
| Terminal block | 2-pin screw terminal | Power input |

## Design Files

Add schematics, truth tables, or firmware (if a microcontroller is used) here, e.g.:

```
02-dip-switch-7seg-decoder/
├── schematic/
├── truth-table.md
└── images/
```

## Status

✅ Prototyped and tested on perfboard — confirmed displaying output as shown in the photo above.
