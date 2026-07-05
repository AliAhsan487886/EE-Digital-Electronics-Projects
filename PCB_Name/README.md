# AHSAN Name Display PCB

A custom-designed and etched PCB that lights up to spell out **"A.H.S.A.N."** — five characters, each built from individually addressable LED segments rather than off-the-shelf 7-segment packages.

![Lit PCB spelling AHSAN](./images/PCB.png)

## Overview

Each letter is formed by an array of surface-mounted LEDs, individually current-limited with **470Ω resistors**, laid out on custom copper traces to form the shape of the letter when lit. The board also includes:

- A small driver IC (visible near the first character)
- A 1kΩ resistor (marked `102`)
- A 33Ω resistor (marked `330`, near the far right)
- A connector/component near the top-left (power/control input)

> Note: fill in the exact IC part number and its role (e.g. driver, current source, blinking control) once confirmed — this README currently describes the board from visual inspection.

## PCB Layout

The routed board layout (front copper) is shown below:

![PCB routed layout](./images/pcb-layout.png)

- Board dimensions: **109.08 mm × 29.01 mm**
- Two-pin power header (Vcc / Gnd) on the left edge
- Silkscreen: `ALI AHSAN 2023-EE-173`

## Bill of Materials (as identified from the board)

| Component | Value / Part | Qty (approx.) | Notes |
|---|---|---|---|
| Resistor | 470Ω | ~35+ | LED current-limiting, one per segment/LED |
| Resistor | 1kΩ (`102`) | 1 | — |
| Resistor | 33Ω (`330`) | 1 | — |
| IC | *TBD* | 1 | Small black package, near first digit |
| LEDs | Red, SMD/segment style | Multiple | Form the letter shapes |

## Design Files

Add your KiCad project files (`.kicad_pcb`, `.kicad_sch`, schematic PDF, Gerbers) here, e.g.:

```
01-ahsan-name-display-pcb/
├── kicad/
│   ├── ahsan-display.kicad_pro
│   ├── ahsan-display.kicad_sch
│   └── ahsan-display.kicad_pcb
├── gerbers/
└── images/
```

## Status

✅ Board etched, populated, and tested — confirmed lighting up as shown in the photo above.
