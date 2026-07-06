# Muller C-Element RTL-to-GDSII Implementation

## Overview

The **Muller C-element** is a fundamental asynchronous logic element used in asynchronous digital circuits. Unlike conventional logic gates, the Muller C-element changes its output only when **all inputs agree**. If the inputs differ, it holds its previous output state. This makes it an essential component for synchronization and handshaking in asynchronous systems.

This project demonstrates the complete **RTL-to-GDSII ASIC design flow** of a Muller C-element using **Verilog HDL** and Cadence EDA tools. The design was functionally verified, synthesized, physically implemented, and converted into a GDSII layout.

---

## Project Objectives

- Design the Muller C-element using Verilog HDL.
- Verify the functionality using a testbench.
- Perform RTL synthesis using Cadence Genus.
- Analyze area, timing, and power reports.
- Complete physical implementation using Cadence Innovus.
- Generate the final GDSII layout.

---

## Working Principle

The Muller C-element follows the logic below:

| Input A | Input B | Output Q |
|---------|---------|----------|
| 0 | 0 | 0 |
| 1 | 1 | 1 |
| 0 | 1 | Holds Previous State |
| 1 | 0 | Holds Previous State |

This behavior enables reliable synchronization in asynchronous circuits.

---

## Project Flow

```text
Verilog RTL
      │
      ▼
RTL Simulation
(NCLAUNCH / SimVision)
      │
      ▼
RTL Synthesis
(Cadence Genus)
      │
      ▼
Gate-Level Netlist
      │
      ▼
Physical Design
(Cadence Innovus)
      │
      ▼
Floorplanning
      │
      ▼
Placement & Routing
      │
      ▼
GDSII Layout
```

---

## Tools Used

- Verilog HDL
- Cadence NCLAUNCH
- SimVision
- Cadence Genus
- Cadence Innovus

---

## Project Files

| File | Description |
|------|-------------|
| `muller.v` | RTL implementation |
| `muller_tb.v` | Testbench |
| `constraints.sdc` | Timing constraints |
| `genus.tcl` | Genus synthesis script |
| `muller_netlist.v` | Synthesized netlist |
| `area.rpt` | Area report |
| `timing.rpt` | Timing report |
| `power.rpt` | Power report |
| `muller.gds` | Final GDSII layout |

---

## Results

✔ Functional simulation completed successfully.

✔ RTL synthesis completed using Cadence Genus.

✔ Area, timing, and power reports generated.

✔ Physical implementation completed using Cadence Innovus.

✔ Placement and routing successfully performed.

✔ Final GDSII layout generated.

---

# RTL Simulation

The RTL design was verified using **Cadence NCLAUNCH (SimVision)**. The simulation confirms that the Muller C-element updates its output only when both inputs are equal and retains the previous output otherwise.

<img width="1600" height="900" alt="nclaunch muller capacitance" src="https://github.com/user-attachments/assets/207282fd-964d-43e6-9189-773ddaade1e7" />


---

# Physical Layout (Innovus)

The synthesized netlist was imported into **Cadence Innovus** for floorplanning, placement, routing, and physical implementation. The final routed layout represents the physical realization of the Muller C-element.

<img width="1600" height="900" alt="muller view" src="https://github.com/user-attachments/assets/8e2ee234-7731-431b-b49a-0a0da8ca33d5" />


---

# GDSII Generation

The final layout was exported as a **GDSII** file, which is the standard format used for IC fabrication. Since GDSII is a binary file, it cannot be viewed in a text editor and should be opened using layout viewers such as Cadence Virtuoso or KLayout.

<img width="1600" height="900" alt="muller gds" src="https://github.com/user-attachments/assets/2d7757f4-8440-4d89-a79b-965c5cef1a18" />

---

## Future Enhancements

- Perform post-layout timing analysis.
- Implement the design using a smaller technology node.
- Extend the design to larger asynchronous circuits.

---

## Author

**Surjini R**

Electronics and Communication Engineering

Interested in VLSI Design • ASIC Design • Physical Design • Digital IC Design
