# 4-bit Adder Interface Board

> **AI-generated README**: This README was generated with AI from the repository contents and may contain mistakes or omissions. Please verify hardware details, part numbers, and wiring against the KiCad source files before using it as authoritative documentation.

## Overview

This repository contains KiCad design files for a custom PCB titled **4 Bit - Seven Seg Interface**. The project appears to be a discrete-logic interface board built around a 4-bit adder and related support circuitry, intended to drive or interface with a seven-segment display.

The repository description indicates it is:

> “A custom PCB designed to mimic the function of a CPU. Entirely made from discrete logic ICs.”

## What is in the repository

The project is organized as a KiCad hardware design with schematic sheets and board/layout files, including:

- **PCB layout**: `4 Bit - Seven Seg Interface.kicad_pcb`
- **KiCad project**: `4 Bit - Seven Seg Interface.kicad_pro`
- **Main schematic**: `4 Bit - Seven Seg Interface.kicad_sch`
- **Supporting schematics**:
  - `Adders.kicad_sch`
  - `Registers.kicad_sch`
  - `Decoder.kicad_sch`
  - `Hex.kicad_sch`
  - `A.kicad_sch`
  - `C&D.kicad_sch`
  - `G.kicad_sch`
  - `555Timer.kicad_sch`
  - `untitled.kicad_sch`
- **Footprint libraries**:
  - `Components.pretty/`
  - `15000LED.pretty/`
- **Backup files**:
  - `4 Bit - Seven Seg Interface-backups/`

## Project structure and inferred function

From the schematic names and symbols used in the design, the board likely includes:

- **4-bit adder stage** using a `CD74HC283M96` 4-bit binary adder
- **Register / storage logic** using flip-flops and DIP switch inputs
- **Decoder / inverter logic** for signal conditioning and display control
- **Seven-segment display interface** using an `LSHD-7503` display component
- **Clock/timing circuitry** using a `555Timer` schematic section
- **Discrete logic gates** such as AND, OR, and NOT devices from the SN74LVC and CD4000 families

## Notable components seen in the schematics

A few parts are visible in the schematic source:

- `CD74HC283M96` — 4-bit binary adder
- `SN74LVC1G08DBVR` — 2-input AND gate
- `SN74LVC1G11DBVR` — 3-input AND gate
- `SN74LVC1G32DCKR` — 2-input OR gate
- `SN74LVC1G14DCKR` — inverter / Schmitt trigger
- `SN74LVC1G175DCKR` — D flip-flop with async clear
- `CD4072BM96` — dual 4-input OR gate
- `LSHD-7503` — seven-segment display
- `CFS-0102TB` — DIP switch component
- `219-8MST` — switch component
- LEDs, resistors, and capacitors for support circuitry

## Likely purpose

Based on the file names and symbols, this board seems intended to:

- accept switch inputs
- store or route 4-bit values
- perform addition with a 4-bit adder
- decode or condition signals
- display results on a seven-segment display

## Getting started

To work with this repository:

1. Install a compatible version of **KiCad 8**.
2. Open `4 Bit - Seven Seg Interface.kicad_pro` in KiCad.
3. Inspect the schematic sheets and PCB layout.
4. Review footprints and part choices before fabrication.

## Manufacturing / fabrication notes

This repository appears to be a hardware design project, so you will likely need to:

- verify all footprints
- confirm net connectivity and board rules in KiCad
- generate Gerbers, drill files, and BOM from the project
- review backups and autosave files before committing to fabrication

## Caveats

Because this README was generated automatically:

- component roles may be inferred incorrectly
- sheet names may not perfectly describe their actual logic
- some file names may represent work-in-progress or unused sheets
- exact electrical behavior should be confirmed in KiCad

## License

No license file was found in the repository contents examined here. If you plan to reuse or distribute the design, check with the repository owner or add an explicit license.
