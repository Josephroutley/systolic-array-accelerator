# Systolic Array Matrix Accelerator

## Project Overview
This project implements a **Systolic Array** architecture to perform high-speed matrix multiplication ($C = A \times B$), the core operation behind modern AI/ML workloads (similar to NVIDIA Tensor Cores).

The focus is on "Power, Performance, and Area" (PPA) trade-offs and computer arithmetic optimization.

## Learning Objectives
* **Computer Arithmetic:** Designing efficient Multiply-Accumulate (MAC) units.
* **Parallel Processing:** managing data flow through a grid of processing elements.
* **PPA Optimization:** Analyzing the trade-offs between a high-performance design vs. a low-area design.

## Architecture
* **Processing Element (PE):** A single unit capable of multiplication and accumulation.
* **Systolic Grid:** A 4x4 (or larger) grid of PEs connected for data streaming.
* **Memory Interface:** Buffers to feed rows/columns into the array.

## Tools & Tech Stack
* **Language:** SystemVerilog
* **Synthesis:** Yosys (for Area/Gate count analysis)

## Roadmap
- [ ] Design the Processing Element (MAC unit).
- [ ] Connect PEs into a 2D Systolic Array.
- [ ] Implement the control logic to "pulse" data through the array.
- [ ] **Analysis:** Synthesize the design targeting maximum speed.
- [ ] **Analysis:** Synthesize the design targeting minimum area.
- [ ] **Report:** Document PPA results in the Wiki/Docs.
