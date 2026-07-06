# Muller C-Element RTL-to-GDSII Flow #
## Overview ##
This project implements an Asynchronous Muller C-element using Verilog HDL and demonstrates the complete RTL-to-GDSII ASIC design flow using Cadence EDA tools.

## Project Flow ##
Verilog RTL
      │
      ▼
Functional Simulation
(NCLAUNCH / SimVision)
      │
      ▼
Logic Synthesis
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
Placement & Routing
      │
      ▼
GDSII Layout

## Project Files ##

muller.v – RTL design
muller_tb.v – Testbench
constraints.sdc – Synthesis constraints
genus.tcl – Genus synthesis script
muller_netlist.v – Synthesized netlist
area.rpt – Area report
timing.rpt – Timing report
power.rpt – Power report
muller.gds – Final GDSII layout

## Tools Used ##

Verilog HDL
Cadence NCLAUNCH
Cadence Genus
Cadence Innovus

## Flow Completed ##

✔ RTL Design

✔ Functional Simulation

✔ Synthesis

✔ Area Analysis

✔ Timing Analysis

✔ Power Analysis

✔ Floorplanning

✔ Placement

✔ Routing

✔ GDSII Generation


Timing report
Power report
Project Objective

To implement and verify an asynchronous Muller C-element while learning the complete ASIC implementation flow from RTL to GDSII using industry-standard Cadence tools.
