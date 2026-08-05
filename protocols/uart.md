# UART (Universal Asynchronous Receiver-Transmitter)

Asynchronous serial communication protocol.

## Frame Format
- Start bit (1 bit, low)
- Data bits (usually 8 bits)
- Parity bit (optional)
- Stop bits (1 or 2 bits, high)

## Baud Rate
Tx and Rx must agree on the speed (e.g., 9600, 115200 baud).