# Chipathon Proposal: Development of a 4-Input Multiplexer Standard Cell

## Project Overview

In this project, our team, Digimon, proposes the development of a **4-input multiplexer (MUX)** standard cell as part of the IEEE SSCS Chipathon 2025. The goal is to design, implement, and verify a robust and reusable MUX cell that can be integrated into larger digital logic designs, contributing to an open-source standard cell library for academic and prototyping use. This work will be conducted from June, 2025 to September, 2025 and will consist of 5 stages:

- Proposal Creation
- Schematic Design and Simulation
- Layout Design and Post-layout verificiation
- Standard Cell Characterization
- Manufacturing & Testing
---

## Team Overview

### Team Name: Digimon
### Institution: Brown University
#### **Members**:
  - Derek Truong
  - Joseph Nwoso
  - Shayaan Chaudhary 
  - Wilson Vo
  - TBD
  
#### All members will participate in cross-functional roles.


## Background

### Gate-Level Design
Below is a gate level schematic of our 4 input multiplexer.

![4-to-1 MUX Block Diagram](images/4_MUX_GL.jpg)

### Function-Level Description

*(To be developed: Describe the functional behavior, select lines usage, and block diagram here.)*

---

## Functional Description

The **4-to-1 Multiplexer** has 4 data inputs (D0, D1, D2, D3), 2 select lines (S1, S0), and 1 output (Y).

| S1 | S0 | Y   |
|----|----|-----|
| 0  | 0  | D0  |
| 0  | 1  | D1  |
| 1  | 0  | D2  |
| 1  | 1  | D3  |

### Function:
Depending on the combination of select lines S1 and S0, the output Y will reflect the corresponding data input.

---

## Specifications

- **Cell Type:** 4-input multiplexer standard cell
- **Inputs:** D0, D1, D2, D3, S0, S1
- **Output:** Y
- **Supply:** VDD, GND
- **Target Technology:** [e.g., SKY130 / Nangate45 / other PDK]
- **Design Goals:**
  - Minimal propagation delay
  - Optimized area for integration into standard cell libraries
  - DRC-clean layout
  - LVS match between schematic and layout
  - Verified functional simulation using standard testbenches

---

## Licenses Overview

We plan to release the design under the **Apache License 2.0**, ensuring:

- Open-source availability
- Freedom to use, modify, and distribute with proper attribution
- Compatibility with common silicon and EDA tool workflows

---

## Future Work (Planned Extensions)

- Development of additional logic cells (AND, OR, XOR, flip-flops)
- Timing characterization for library integration
- Automated verification and layout generation scripts

---

### 📂 Repository Structure (Tentative)

