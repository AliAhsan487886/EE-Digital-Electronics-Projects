# AHSAN Name Display PCB

A custom-designed and etched PCB that lights up to spell out **"A.H.S.A.N."** — five characters, each built from individually addressable LED segments rather than off-the-shelf 7-segment packages.
<img width="619" height="376" alt="PCB_Name" src="https://github.com/user-attachments/assets/8162202a-3e36-4d5d-8814-627aba52742f" />

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

## Altium Design for PCB

<img width="877" height="257" alt="Alitium_Design_01" src="https://github.com/user-attachments/assets/733eccbd-d095-4765-bd14-3a5e2e40dba1" />

## Status

Board etched, populated, and tested — confirmed lighting up as shown in the photo above.
