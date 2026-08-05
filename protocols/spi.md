# SPI (Serial Peripheral Interface)

SPI is a synchronous serial communication interface specification used for short-distance communication, primarily in embedded systems.

## Pins
- **MOSI**: Master Out Slave In
- **MISO**: Master In Slave Out
- **SCLK**: Serial Clock
- **CS/SS**: Chip Select / Slave Select

## Modes
Determined by CPOL (Clock Polarity) and CPHA (Clock Phase).
- Mode 0: CPOL=0, CPHA=0
- Mode 1: CPOL=0, CPHA=1
- Mode 2: CPOL=1, CPHA=0
- Mode 3: CPOL=1, CPHA=1