# UART-RTL-TO-GDSII
UART transmitter and receiver design using Verilog HDL, functional verification, and the ASIC RTL-to-GDSII implementation flow.

# UART Transmitter and Receiver — RTL to GDSII

This project involved designing and implementing a UART transmitter and receiver using Verilog HDL and taking the design through the ASIC RTL-to-GDSII implementation flow.

## About the Project

UART (Universal Asynchronous Receiver Transmitter) enables serial communication between digital devices. The design uses a 50 MHz system clock and supports communication at 115200 baud.

The UART design consists of a transmitter, receiver, baud-rate timing logic, and a top-level module integrating the components.

## Tools and Technologies

- **HDL:** Verilog
- **Simulation:** Cadence SimVision
- **Logic Synthesis:** Cadence Genus
- **Physical Design:** Cadence Innovus
- **Design Flow:** RTL design, functional verification, synthesis, floorplanning, placement, clock tree synthesis, routing, and physical verification

## Functional Verification

The design was verified in loopback mode by connecting the transmitter output to the receiver input.

| Transmitted Data | Received Data | Result |
|---|---|---|
| `8'hA5` | `8'hA5` | Pass |
| `8'h3C` | `8'h3C` | Pass |

## Implementation Results

The project report documents the following synthesis results:

- **Synthesis cell area:** 2225.286 µm²
- **Total synthesis power:** 8.79 × 10⁻⁵ W
- **Worst Negative Slack (WNS):** 0 ns
- **Total Negative Slack (TNS):** 0 ns

The report also documents physical-design stages, DRC/LVS verification, timing analysis, and GDSII generation.

## What I Learned

This project gave me practical exposure to the ASIC design flow, from Verilog-based RTL design and functional verification to synthesis and physical implementation using Cadence EDA tools.

---

*Note: This repository currently documents the project based on my report. Verilog source files and other implementation artifacts are not included yet.*
