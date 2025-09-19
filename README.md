RISC-V Reference SoC Tapeout Program by VSD
===========================================

This repository documents my journey through VSD's RISC-V Reference SoC Tapeout Program, featuring week-to-week task submissions along the way. The aim of the project is to design, implement, and tape out a System on Chip (SoC) using robust open-source VLSI methodologies, providing practical exposure to the complete digital design flow from specification to GDSII for fabrication.

## SoC Tapeout Pipeline

**Specification and Modeling:**  
Begin by defining the chip’s functionality, target performance, and design constraints. Develop a high-level behavioral model in C/C++ and use a testbench to verify that the initial idea meets the requirements.

**RTL Design:**  
Convert the behavioral model into Register Transfer Level (RTL) hardware code using Verilog or VHDL. This captures all data flows, control paths, and major functional blocks while ensuring correctness by comparing it to the initial model.

**Synthesis:**  
Employ synthesis tools to transform the RTL into a technology-specific gate-level netlist, mapping functions to digital gates and integrating essential pre-designed IP blocks for both digital and analog features.

**SoC Integration:**  
Assemble the synthesized processor, memory, macros, IPs, and essential peripherals into a unified chip architecture. This involves interconnecting data, control, clock, and I/O domains for a cohesive SoC.

**Physical Design (RTL to GDSII):**  
Transform the chip’s logical representation into a manufacturable physical layout. This phase includes floorplanning, placement, clock tree synthesis, routing, and utilization of standard cell and IP libraries to create the final mask layout.

**Verification and Sign-off:**  
Perform comprehensive verification to ensure successful silicon fabrication. This includes running Design Rule Checks (DRC) for manufacturability, Layout Versus Schematic (LVS) checks for circuit correctness, and finally exporting the chip as a GDSII file ready for tapeout.


# Project Organization
