# Frequency-Meter

## Overview

The **Frequency Meter** is a digital circuit designed to measure an unknown input frequency in the range of **0.00 Hz to 99.99 Hz**. It operates using a **100 Hz Time Base Frequency** as a reference for measurement accuracy.

This project includes both the schematic and PCB design created using **KiCad**. The design is compact and intended for educational or experimental use in lab environments or as a standalone frequency counter module.

---

## Features

- Measures frequency in the range **0.00 Hz to 99.99 Hz**
- **100 Hz Time Base** for accurate measurement
- Dual-digit decimal output display
- Optimized for simplicity and low component count
- Designed in KiCad (open-source EDA)

---

## How It Works

The working principle is based on frequency counting using a time gate. The **unknown signal** is counted over a **fixed time window of 1 second** (derived from a 100 Hz time base using a divider circuit). The counted pulses are then scaled and displayed on a 2-digit 7-segment display, showing values in the format XX.XX.

### Major Blocks:

- **Time Base Generator**: Generates 100 Hz from a crystal oscillator or other stable reference.
- **Frequency Counter Logic**: Counts the number of pulses from the unknown frequency source during the gate time.
- **Display Driver**: Converts the counted value into a human-readable format using 7-segment displays.

---

## Schematic and PCB

- **Schematic File**: `0682.kicad_sch`
- **PCB Layout File**: `0682.kicad_pcb`

These files can be opened using [KiCad](https://www.kicad.org/) (version 6 or later recommended).

---

## Components Used (Typical)

- Crystal Oscillator or Timer IC (for 100 Hz base)
- Flip-flops / Logic ICs (74-series or CD4000)
- Counters (e.g., CD4017, 74LS90)
- 7-Segment Display Drivers
- 7-Segment Displays (2-digit)
- Resistors, Capacitors, and other passive components
- Optional: Microcontroller (if using software counter)

---

## Applications

- Frequency counter for waveform generators
- Educational kits and demonstrations
- DIY electronics lab equipment
- Signal analysis and debugging tools

---
