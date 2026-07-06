# LED Dot-Matrix Display Driver

A perfboard-built **8×8 LED dot-matrix display** driven through driver ICs and Controlled by 8 bit DIP Switch.

<img width="768" height="744" alt="PROJECT_Board" src="https://github.com/user-attachments/assets/6c2bea16-8c47-4873-9d73-864e3fbead4e" />

## Overview

- An 8×8 dot-matrix LED module mounted on perfboard
- Two DIP-package driver/decoder ICs (one on each side of the matrix) — likely row/column drivers such as shift registers (`74HC595`) or a driver+decoder pair (e.g. `ULN2803` + `74HC154`)
- A 2-pin screw terminal for power input (bottom-left)
- A small blue component near the power input (possibly a capacitor or trimmer — confirm)
- A status LED (bottom, lit red)
- A multi-conductor cable bundle carrying control signals in from an external controller board

> Note: confirm and fill in the exact IC part numbers, pinout, and the row/column scan scheme (static drive vs multiplexed) once verified — this README currently describes the board from visual inspection.

## Bill of Materials


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

[Exp3.pdf](https://github.com/user-attachments/files/29689474/Exp3.pdf)

## Status

Prototyped on perfboard — confirmed lighting up rows as shown in the photo above.

<img width="201" height="154" alt="image" src="https://github.com/user-attachments/assets/a6872312-aa38-408b-aee1-5bc574645392" />
