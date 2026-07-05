# LED Dot-Matrix Display Driver

A perfboard-built **8×8 LED dot-matrix display** driven through driver ICs, controlled externally via a wired connection (from a microcontroller / driver board).

![LED dot-matrix display lit up](./images/dot-matrix-display.png)

## Overview

- An 8×8 dot-matrix LED module mounted on perfboard
- Two DIP-package driver/decoder ICs (one on each side of the matrix) — likely row/column drivers such as shift registers (`74HC595`) or a driver+decoder pair (e.g. `ULN2803` + `74HC154`)
- A 2-pin screw terminal for power input (bottom-left)
- A small blue component near the power input (possibly a capacitor or trimmer — confirm)
- A status LED (bottom, lit red)
- A multi-conductor cable bundle carrying control signals in from an external controller board

> Note: confirm and fill in the exact IC part numbers, pinout, and the row/column scan scheme (static drive vs multiplexed) once verified — this README currently describes the board from visual inspection.

## Bill of Materials (as identified from the board)

| Component | Value / Part | Notes |
|---|---|---|
| Dot-matrix LED module | 8×8, common row/column | Yellow/orange LEDs |
| Driver IC | *TBD* (DIP package) | Left side of matrix |
| Driver IC | *TBD* (DIP package) | Right side of matrix |
| Terminal block | 2-pin screw terminal | Power input |
| LED | Red, indicator | Status/power |
| Capacitor/trimmer | *TBD* | Near power input |
| Cable bundle | Multi-conductor | Control signals from external board |

## Design Files

Add schematics, control code, or the multiplexing/scan logic here, e.g.:

```
03-led-dot-matrix-display/
├── schematic/
├── firmware/          # if driven by a microcontroller
└── images/
```

## Status

✅ Prototyped on perfboard — confirmed lighting up rows as shown in the photo above.
