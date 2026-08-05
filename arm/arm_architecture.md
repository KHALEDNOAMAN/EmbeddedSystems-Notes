# ARM Cortex-M Architecture

## Overview
Cortex-M is a group of 32-bit RISC ARM processor cores optimized for low-cost and energy-efficient microcontrollers.

## Registers
- **R0-R12**: General Purpose Registers
- **R13 (SP)**: Stack Pointer (MSP/PSP)
- **R14 (LR)**: Link Register (stores return address)
- **R15 (PC)**: Program Counter

## Pipeline
Most Cortex-M processors use a 3-stage pipeline:
1. **Fetch**: Instruction fetched from memory.
2. **Decode**: Instruction decoded.
3. **Execute**: Instruction executed.