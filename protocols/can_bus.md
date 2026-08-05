# CAN (Controller Area Network)

Standard for robust vehicle bus designed to allow microcontrollers and devices to communicate without a host computer.

## Features
- Message-based protocol (not address based)
- Differential signaling (CAN_H, CAN_L)
- Multi-master, CSMA/CR arbitration
- Dominant (0) and Recessive (1) bits

## Arbitration
Nodes with lower ID have higher priority (more dominant bits early on).