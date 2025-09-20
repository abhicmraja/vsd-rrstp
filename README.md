# RISC-V Reference SoC Tapeout Program by VSD

This repository documents my journey through **VSD's RISC-V Reference SoC Tapeout Program**, featuring week-to-week task submissions along the way.  
The aim of the project is to **design, implement, and tape out a System on Chip (SoC)** using open-source VLSI methodologies — providing practical exposure to the complete digital design flow from **specification to GDSII for fabrication**.

---

## SoC Tapeout Pipeline

The SoC development pipeline can be broken down into six key stages:

---

### 1. <span style="color:#2E86C1">Specification and Modeling</span>
- Define functionality, target performance, and design constraints.  
- Develop a high-level **C/C++ behavioral model**.  
- Use a testbench to verify requirements.

---

### 2. <span style="color:#28B463">RTL Design</span>
- Translate the behavioral model into **Verilog/VHDL**.  
- Capture data flows, control paths, and functional blocks.  
- Verify RTL correctness by comparing with the initial model.

---

### 3. <span style="color:#CA6F1E">Synthesis</span>
- Employ synthesis tools to transform RTL into a **gate-level netlist**.  
- Map functions to digital gates.  
- Integrate pre-designed IP blocks (digital + analog).

---

### 4. <span style="color:#8E44AD">SoC Integration</span>
- Assemble processor, memory, macros, IPs, and peripherals.  
- Interconnect data, control, clock, and I/O domains.  
- Build a cohesive SoC architecture.

---

### 5. <span style="color:#D35400">Physical Design (RTL → GDSII)</span>
- Convert the logical design into a manufacturable **physical layout**.  
- Floorplanning → Placement → Clock Tree Synthesis → Routing.  
- Leverage standard cell + IP libraries to generate the final mask layout.

---

### 6. <span style="color:#C0392B">Verification & Sign-off</span>
- Run **Design Rule Checks (DRC)** for manufacturability.  
- Perform **Layout Versus Schematic (LVS)** for correctness.  
- Export final chip as a **GDSII file** ready for tapeout.

---

## Project Organization

The repository is structured into the following directories:

