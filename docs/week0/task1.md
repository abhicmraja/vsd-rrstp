# Task 1 - Summarise Video on VLSI SoC Design and Planning Process 

Designing a System on Chip (SoC) using VLSI methodologies involves a series of structured steps, transforming an abstract idea into a manufacturable silicon chip. Here’s a concise, descriptive overview suitable for a GitHub repository main page:

## 1. Specification and Modeling

- Clearly define the intended functionality, performance targets, and constraints for the chip.
- Use a high-level language (like C/C++) to create a behavioral model of the chip.
- Develop a corresponding testbench to simulate and verify that the model behaves as desired.

## 2. RTL Design

- Elaborate the high-level model into a hardware-specific description at the Register-Transfer Level (RTL) using Verilog or VHDL.
- The RTL code specifies how data moves and gets processed, defining control logic, datapaths, and key functional units (e.g., processor cores, peripherals).
- Verify that the RTL design matches the original model’s intent.

## 3. Synthesis

- Use synthesis tools to automatically translate the RTL code into a gate-level netlist (interconnected standard logic cells suited to a target fabrication tech).
- Integrate pre-designed functional blocks (macros and IPs), which may include both digital and analog components, provided as either soft (flexible) or hard (fixed) blocks.

## 4. SoC Integration

- Integrate all synthesized components: processors, macros, analog/digital IPs, and peripherals.
- Connect data, control, clock domains, and I/Os to form a unified SoC architecture.

## 5. Physical Design (RTL to GDSII)

- Transform the logical design into a manufacturable chip layout.
- Key steps:
  - **Floorplanning**: Arranging and sizing main blocks on the chip.
  - **Placement**: Physically positioning all logic cells.
  - **Clock Tree Synthesis (CTS)**: Creating a robust clock network.
  - **Routing**: Laying down metal wires to interconnect all cells and blocks.
- Employ physical libraries for IPs/macros, which may be “hardened” (fixed) or “soft” (flexible).

## 6. Verification and Sign-off

- Perform rigorous final checks:
  - **Design Rule Checks (DRC)**: Ensure layout follows manufacturability and reliability rules.
  - **Layout Versus Schematic (LVS)**: Confirm layout matches the intended circuit structure.
- Once verified, export the final layout as a GDSII file, ready for semiconductor fabrication.

